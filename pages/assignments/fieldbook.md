---
layout: page-fullwidth
title: Lab Fieldbook Entries
permalink: /assignments/fieldbook/
header:
  image_fullwidth: 14934283002_9663bae608_k-banner.jpg
  caption: Creative Commons licensed photograph "Field book, Raffles Lighthouse museum" by Flickr user Jnzl's Photos
---

## Assignment Overview:

+ A portfolio of at least 9 documents, composed in [MultiMarkdown](http://fletcherpenney.net/multimarkdown/)
+ Individual work submitted; collaborative development encouraged
+ Entries due 1 week after the final session for a given lab
+ Entries will be posted on the course website and be available under [Class Updates](/updates/)
+ At least 3 entries due by Monday, February 19
+ 40% of total grade

## Details:

Technologies of Text is an experiential course and defined by hands-on labs throughout the semester. There will be a diversity of activities associated with labs in particular, from observations made at museums to physical documents printed on a letterpress. Some of these activities will be conducted individually and some in groups.

Your ToT fieldbook will constitute your central scholarly activity during the semester. I call this assignment a "fieldbook" rather than a "journal" to convey its hybridity: week by week, your entries will include a mix of description, analysis, code, and figures or images. This ongoing assignment will give you the chance to organize the diverse tasks of the class' experiential work, practice the skills introduced in the labs and coding sessions, bring your experiential work into conversation with class readings and personal research, and experiment with ideas that will be further developed in your [Unessay projects](/assignments/unessay).

### Organizing Your Fieldbook

Your fieldbook will be, essentially, a folder comprising at least 9 `.md` files, perhaps including supplemental files such as images referenced in the documents. We'll work on setting this up in our first code session, so you don't need to understand precisely what this means right now. Your fieldbooks will be posted to the [Class Updates](/updates/) section of the course website.

### Composition

Your fieldbook entries will vary quite a bit from lab to lab. However, there are a few elements I will expect in each entry:

1. Completion of any lab-specific activities. Most of our experiential activities will include a specific set of outcomes. For example, I might ask you to reflect on a set of questions about your experiences or challenge you to adapt the day's code to solve some practice problems, or you might produce a specific material product such as a letterpress printed sheet. The first task of any fieldbook entry will be to demonstrate completion of these tasks. In the case of a coding session, you will likely integrate code snippets directly into the .RMD file (more on this as those labs approach). For other labs you may instead reference external proof of your work (and possibly submit that external evidence separately).

2. Prose that both describes the work done and reflects analytically on that work. This prose need not be as formal as a research paper, but it should demonstrate careful thought and preparation. You should integrate our course readings into these reflections, often through direct quotation. Use your fieldbooks to explore ideas from the readings that you found particularly interesting, and especially ideas we did not have time to discuss in class. Use this writing to experiment with intellectual pairings you think might be generative to your larger thinking and help you prepare for the class' Unessay projects.

3. Evidence of your experiential work, particularly for code entries. One reason we will produce some entries in R Markdown is that Markdown provides a way to integrate executable code with prose that comments and reflects on that code. You needn't include every snippet of code you attempted (though keep in mind "failed" code can be interesting as a subject of reflection). Instead, you should include the most enlightening or intellectual productive bits of code that help illustrate the larger ideas you are working through in your fieldbook.

4. A header that will allow me to publish your fieldbook easily on the course website and makes clear precisely which lab activity a given entry records. We will go over this header in our first lab, but I've included a model below you can simply copy, paste, and modify. As an example, you might include the following lines at the top of each file (or each entry if you're using a single file), modified to suit the specifics of each week:
    ``` 
    ---
    layout: page  
    title: "Your TITLE HERE"  
    author: "YOUR NAME or PSEUDONYM"  
    categories:  
        - fieldbooks
    comments: false  
    show_meta: true
    header:
        image_fullwidth: OPTIONAL-IMAGE-NAME.FILE-EXTENSION
        caption: OPTIONAL CAPTION FOR IMAGE WITH CITATION
        caption_url: OPTIONAL URL FOR IMAGE CITATION
    ---
    ```
If your file does not include these fields I will ask you to revise it before I can consider the entry complete.

5. The filename must also follow a very specific convention in order to post correctly. Essentially, it lists the date (of submission) in Year, Month, Day format, followed by your last name (or pseudonym) and the lab number. Essentially, it should look like this: ```YYYY-MM-DD-NAME-LAB-NUMBER.md````.

### Flexibility

ToT is a challenging and full class. The semester will include 12 labs. To give you some flexibility, you must complete a fieldbook entry for 9/12 labs over the semester. You may complete more than 9 entries over the semester, so long as you continue to meet the guidelines for timing and submission outlined below. If you complete more than 9 entries, I will include only the strongest 9 in my grade book (meaning you can make up for a weaker submission). 

### Pacing Your Field Work

Your fieldbook should be a developing record of your thinking about our class and its activities. Thus you should be working on it steadily, responding to the labs and code sessions in a timely manner, in part to keep your thinking fresh and in part to avoid falling too far behind as new labs and code sessions approach. 

Unless otherwise noted, a fieldbook entry is due within 1 week of the associated lab session. If a particular lab session extends through multiple classes, its fieldbook entry is due within 1 week of the final classroom session devoted to it. You may not wait until late in the semester to complete fieldbook entries for activities earlier in the semester, and I will collect your fieldbooks periodically to ensure you are working steadily. The coding labs, in particular, will build on each other and you will find it difficult to complete fieldbooks for later coding labs if you do not complete earlier ones. 

I regularly assign ongoing assignments in my classes and every semester I strongly urge students to start working early in order to complete the work. Each semester at least a few students ignore this urging, usually to their later dismay. Complications will almost certainly arise during the semester, and if you put off starting your fieldbook entries you will struggle to earn full credit on this assignment. In order to pressure you a bit toward responsibility: **you must complete at least 3 entries by President's Day, February 19**. I strongly recommend you complete more before this date, but I will not assess more than 5 entries completed after this date if at least 3 were not completed before. 

### Why Markdown?

I am asking you to write in Markdown for two primary reasons: 

1. Markdown makes it very easy to weave together code and prose, which I see as a necessity for a class that wants to think humanistically about code. 

2. Markdown itself will help us think about text and remediation in a very direct way. Writing outside of a GUI (Graphical User Interface) like Word will challenge use to think about the structure of our texts and how that structure translates among different media. I don't want to pretend like the plain text of Markdown is somehow less mediated than a GUI; Markdown is an interface just like Word is an interface. But I suspect it is an unfamiliar interface for many of you, which will prompt you to think about how interface shapes our interactions with text. 

3. Markdown is flexible. A single Markdown document can be instantly translated through a program like [Pandoc](http://pandoc.org/) into HTML, DOCX, PDF or a range of other formats, and we can use these transformations to think through the affordances and limitations of those formats for contemporary writing.