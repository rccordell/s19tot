Technologies of Text  
Spring 2019

## Deciphering a Program

Below you'll find a snippet of some code that we will work with later this semester. Today I just want to look at the code together and work to decipher it. You'll be in groups and I want you to try and answer, to the best of your ability:

1. From what point does the code begin? In other words, what's its source data?
2. What does this code *do*? When it's run, what is the final product?
3. How does the code get from its source data to that final product? Which of the intervening steps can you separate out and understand?
4. This last step is more abstract, but how are the operations of this code *similar* to writing, and how are they *distinct*?

# Mystery Code

```{r, eval = FALSE, tidy=TRUE, tidy.opts=list(width.cutoff=50)}

my_wordnik_key <- "YOUR_API_KEY_GOES_HERE"

#the line below will set the "default" part of speech for your calls to Wordnik, but you will be able to override this setting in later code.
wordnik_pos = "adjective"

#
random_word <- function(key=my_wordnik_key,
                        pos=wordnik_pos, min_count=100, n=1,
                        min_length = 5, max_length = 10){
  
  param <- paste0("words.json/randomWords?hasDictionaryDef=true",
                  "&minCorpusCount=",min_count,
                  "&minLength=",min_length,
                  "&maxLength=",max_length,
                  "&limit=",n,
                  "&includePartOfSpeech=",pos)

  raw = birdnik:::query(key = key,params = param)
  do.call(rbind,lapply(raw,as.data.frame))
  
}

poem_word <- function(x) {
  random_word(pos=x,n=1,min_count=1000)[,2] %>%
    as.character()
}

poem_word("interjection")

poem <- paste(c(poem_word("verb"), " thy ", poem_word("noun"), " from ", poem_word("preposition")," my ", poem_word("noun"), ", and ", poem_word("verb"), " thy ", poem_word("noun"), " from ", poem_word("preposition"), " my ", poem_word("noun"), "! \nQuoth the Ravbot, '", poem_word("interjection"), "!'"), collapse = "")

cat(poem)

setup_twitter_oauth("YOUR_CONSUMER_KEY_GOES_HERE", 
                    "YOUR_CONSUMER_SECRET_GOES_HERE", 
                    'YOUR_ACCESS_TOKEN_GOES_HERE', 
                    'YOUR_ACCESS_SECRET_GOES_HERE')

woeid <- "2367105"
trend <- getTrends(woeid)[,1] %>%
  as_data_frame() %>%
  rename(trend = value) %>%
  filter(grepl("^#", trend))

poem <- paste(c(poem_word("verb"), " thy ", poem_word("noun"), " from ", poem_word("preposition")," my ", poem_word("noun"), ", and ", poem_word("verb"), " thy ", poem_word("noun"), " from ", poem_word("preposition"), " my ", poem_word("noun"), '!" \nQuoth the Ravbot, "Never ', trend %>% sample_n(1), "!'"), collapse = "")

cat(poem)

if(nchar(poem) < 140) {
  tweet(poem)
  } else {
    print("The poem is too long. Please rerun the generator and try again!")
  }
```