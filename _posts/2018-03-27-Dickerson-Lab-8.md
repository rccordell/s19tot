---
layout: page  
title: "Lab 8"  
author: "Claire Dickerson"  
categories:  
    - fieldbooks
    - model
comments: false  
show_meta: true     
---

## Computational Reading I
---

Even though it is a relatively simple feature, I was very much drawn to the 
```{r}
  select(text,title)%>%
  filter(text != "")%>%
  na.omit()
```
bit of code we worked with in class. Of course, in its form above it will not *do* anything, so inspired by the end of *The Thrilling Adventures of Lovelace and Babbage* I also wrote this little bit of code to pull in *Alice's Adventures in Wonderland* for the feature to actually work.

```{r}
library(tidytext)
library(tidyverse)
library(gutenbergr)

alice <- gutenberg_download(11, meta_fields=c("title","author"))

alice <- alice %>%
  select(text)%>%
  filter(text != "")%>%
  na.omit()

View(alice)
```


Looking at the variable 'alice', most people would identify it as *Alice's Adventures in Wonderland* without issue, but in reality this particular form of it is a different novel. *Alice's Adventures in Wonderland* is a completely different story without its specific formatting and John Tenniel's illustrations. Part of the reason I like the function I picked is because it seems so simple, like it is only making a text easier for formatting, but it realistically does more than that. I hate to continually reference 'the medium being the message,' but this is an instance where, when aesthetic features are removed, the reaction to the text becomes different.  Like George Eliot's book that was not actually George Eliot's book in *The Thrilling Adventures of Lovelace and Babbage*, the text is treated as an object of analysis to be ripped apart and put back together again. 

On the one hand, that is distressing for a lover of literature. It seems blasphemous to have such disregard for the structure of the novel and to treat the spacing and stylistic flairs as unimportant. But on the other hand, is that not what literary analysis generally does? Will not (most) every literature professor tell their students to disregard the author's intention and treat the text as their own to rip apart and reassemble in the way they find meaningful? Is that not essentially what an essay is, a blend of original information polluted with external input?

Thinking of it that way, it is interesting to interpret the type of textual analysis we did in this lab as somewhat like literary composition. In a way, it is reminiscent of a grossly simplified type of erasure poetry. The author of the code filters out the words in the book that do not contribute to their storyline, similar to how an author of erasure poetry filters through what is already there to create something entirely new. 

Similarly, generating ngrams is poetic in a way, reminiscent of Ernest Hemingway's ( [almost certainly misattributed](http://www.openculture.com/2015/03/the-urban-legend-of-ernest-hemingways-six-word-story.html) ) [six word memoirs](https://www.sixwordmemoirs.com/). Though ngrams' use for finding the reproductions of texts in newspapers in the 19th century was mentioned during the lab, as a self contained unit each ngram either tells its own story or hints at part of one. It creates a somewhat beautiful relationship between literature and programming that is particularly striking when thinking of how programming and literature fields have been separated in the past several years.

This distinction need not exist, though. Historically, some of the best programmers have not distanced themselves from creative fields. As Sydney Padua writes about towards the end of *The Thrilling Adventures of Lovelace and Babbage*, both Ada Lovelace and William Rowan Hamilton were interested in poetry, and even though it may not have been 'good,' literature quality is subjective, and the point is that this separation between computers and literature has been drawn in nonsensically somewhere along the way.

Code is much more similar to literature than it might initially appear, and thinking about it as such is important for multiple reasons. Of course, it is useful for breaking down social barriers and helping to eliminate somewhat elitist attitudes that, realistically, have appeared on both sides of the technology/humanities schism. But also artistic expression has been shown to have a [noticeable psychological impact](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2804629/) when dealing with mental health issues, as well as simply improving work function. Coders today are some of the most stressed employees on the planet, [constantly getting burnt out](https://www.theparisreview.org/blog/2014/09/05/the-beauty-of-code/), and allowing for more creativity *could* (could, not necessarily would) help with those issues. 

Looking at how code and literature are related is good, but it can also be beneficial to think of how code could learn from, or be inspired by, literature. I know no more code than what we have learned in this class, but there is still the potential for coding to change if it is looked at as something creative, rather than strictly an input to create an output. It is impossible to predict the future, but it is always fun to think about how the technology of programming will change as it becomes more accessible. And who knows, maybe one day people *will* be writing their poems in code.