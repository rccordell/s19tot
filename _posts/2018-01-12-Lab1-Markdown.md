---
layout: page
subheadline: "Lab #1"
title: "Understanding Textual Structure with Markdown"
categories:
    - labs
comments: false
show_meta: true
header:
  image_fullwidth: 4880254551_9a35151a0d_b-banner.jpg
  caption: Creative Commons licensed photograph, "Underwood," by Flickr user Canned Muffins
  caption_url: https://flic.kr/p/8rfzDR
---

## The Assignment

Your assignment for this coding session is pretty straightforward. You will write a post in Markdown that uses your experience learning and using Markdown to reflect on our our initial readings (McLuhan, Liu) about media and its messages. How does the Markdown medium shape the way you think about your messages (i.e. your writing)? What affordances does Markdown provide, or might it provide, and what limitations does it introduce? 

It will be perhaps artificial, but to practice writing in Markdown your fieldbook entry should include:

+ Some italicized text
+ Some bold text
+ At least one link
+ At least one ordered (numbered) or unordered (bulleted) list
+ Headlines for different sections
+ I won't require it, but *extra kudos* if you can include an image and/or a footnote. 

Your post must also be named correctly and include the header outlined in [the fieldbook assignment](http://s18tot.ryancordell.org/assignments/fieldbook) and reiterated at the bottom of this lab assignment.

## What is Markdown?

Markdown is a lightweight standard for writing in plain text while encoding the **structure of your document** for later representation in a format like Word, PDF, or HTML. If you have ever marked up a text using HTML tags, Markdown works quite similarly, but uses simple typographical symbols to encode text rather than longer HTML tags. There are a number of *affordances* to working in Markdown, including:

1. Simplicity. Because Markdown is a plain-text system of encoding structural elements typographically—rather than, as in proprietary formats like `docx`, though hidden, underlying code—Markdown files are small in size and simple to compose. You do not need to interrupt your writing to format your document while writing in Markdown.
2. Flexibility. When writing in Markdown you encode directions for styling your text, but you do not style it directly. Because of this, an `md` file can be easily converted to many other standard file types, including `html` or `pdf`. You can easily convert a single `.md` file into a range of other formats, giving you flexibility when you wish to publish your writing. When you send me your fieldbooks in Markdown, our website will translate the Markdown you wrote into HTML for display online. 
3. Durability. Unlike files composed in specific version of proprietary software, Markdown files are, essentially, plain text files. This means they can be opened by a wide range of applications and they will look essentially the same, and that they are not subject to the vicissitudes of software updates or platform dependencies. You can open and edit a Markdown file on virtually any computer, and you will likely be able to do well into the future. Even if the conventions of Markdown are no longer understood, the central text should remain widely compatible and portable. 

As with any medium, of course, there are also *limitations* to writing in Markdown, such as:

1. You have less granular control over the appearance of your text than you would in a full featured word processor. In order to ensure the flexibility and durability of Markdown, its grammar is relatively constrained. While you can indicate text should be `bold` or formatted in a `numbered list` using Markdown, for instance, you could indicate that one paragraph's font should be 2 points larger than another. 
2. You typically have to convert Markdown files into another format before publication. This is not *quite* true on the web, where some frameworks (like [Jekyll](https://jekyllrb.com/), in which our class website is built) can understand Markdown directly, but usually the production stage for a Markdown document involves converting you `md` file into another format and converting its structural encoding into actual stylistic changes.

For our class, writing in Markdown will help you reflect on the relationship of your texts' structure to the media of their presentation. You will compose your [fieldbook entries](http://s18tot.ryancordell.org/assignments/fieldbook/) in Markdown or [R Markdown](http://rmarkdown.rstudio.com/), the latter of which will allow you to embed code written in the R programming language directly into a Markdown document.

## Markdown References

Below I will describe the most common Markdown syntax, but for additional reference you can consult:

+ The [Markdown Wikipedia page](https://en.wikipedia.org/wiki/Markdown), which includes a very handy chart of the syntax.
+ John Gruber's [introduction to Markdown](https://daringfireball.net/projects/markdown/syntax). Gruber developed the standard and knows what he's talking about!
+ This [interactive Markdown tutorial](http://www.markdowntutorial.com/), which will teach you the syntax in a few minutes.
+ You can also download [the Markdown version of this page](https://raw.githubusercontent.com/rccordell/s18tot/gh-pages/_posts/labs/2018-01-12-Lab1-Markdown.md) if you'd like to compare what you see in your browser with the marked-up text that created it.

In short, in Markdown your text will not include any visible stylistic variations such as italics or bold text; Markdown is a *plain text* format. 

## Applications for Writing in Markdown

One advantage to this is that you can write valid Markdown in many, many editors, including the free text editors (such as TextEdit on the Mac or Wordpad on the PC) that come with most computers. You can also write in Markdown in my favorite writing application, [Scrivener](https://www.literatureandlatte.com/scrivener.php). 

There are many dedicated Markdown composition applications with additional features, such as syntax highlighting or the ability to preview what your documents. Some are paid, but here are some free ones:

+ [Macdown](http://macdown.uranusjr.com/) (Mac)
+ [Mou](http://25.io/mou/) (Mac)
+ [Markdownpad](http://markdownpad.com/) (Windows XP-8)
+ [Markdown Edit](http://markdownedit.com/) (Windows)
+ [Ghostwriter](http://wereturtle.github.io/ghostwriter/) (Windows & Linux)
+ [Remarkable](https://remarkableapp.github.io/) (Linux)
+ [Hashify](http://hashify.me/IyBUaXRsZQ==) (online) 
+ a bit more complicated to get started with, but [Atom](https://atom.io/) is more full-featured than some of those above (Mac, Windows, Linux)

## Markdown Syntax

So, a few basics:

1. If you want your text to be italicized, then *enclose it in single asterisks*. (i.e. \*enclose it in single asterisks\*).
2. If you want your text to be bold, then **enclose it in double asterisks**. (i.e. \*\*enclose it in double asterisks\*\*).
3. To start a new paragraph, simply hit return twice, so that you see a single line space in between paragraphs.
4. To start a new line without a paragraph break, add two spaces to the end of the first line and then hit return once.
5. To create a hyperlink, enclose the [words you want linked in brackets and the link in parentheses following](http://s17tot.ryancordell.org/). 
    i.e. \[words you want linked in brackets and the link in parentheses following\]\(http://s18tot.ryancordell.org/\)    

You can also create headlines of descending sizes, lists (numbered or bulleted), footnotes, block quotations, embedded images, and more. See the reference materials above for details on these other elements. 

## Conventions for Posting on the ToT Website

Our course website is built in [Jekyll](https://jekyllrb.com/), which understands Markdown natively for blog posts and pages. There are a few additional conventions you will need to follow so that your fieldbook entries appear as we would wish on the website. These conventions are also outlined in the [fieldbook assignment](http://s18tot.ryancordell.org/assignments/fieldbook/).

### File Name

The filename must follow a very specific convention in order to post correctly. Essentially, it lists the date (of submission) in Year, Month, Day format, followed by your last name (or pseudonym) and the lab number. Essentially, it should look like this: ```YYYY-MM-DD-NAME-LAB-NUMBER.md```.

### Header

The file also needs a header that will allow me to publish your fieldbook easily on the course website and makes clear precisely which lab activity a given entry records. I've included a model below you can simply copy, paste, and modify. As an example, you might include the following lines at the top of each file (or each entry if you're using a single file), modified to suit the specifics of each week:

```
---
layout: page  
title: "Your TITLE HERE"  
author: "Your NAME or PSEUDONYM"  
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
    
Your file must include the lines for `layout` (which may stay exactly the same each week, `title`, `author`, and should include at least the `lab number` under `categories`. Note that `title` and `author` are enclosed in quotation marks and `lab number` is preceded by four spaces, a hyphen, and another space. If your file does not include these fields I will ask you to revise it before I can consider a given fieldbook entry complete. You need not include the other fields, and if you do not wish to include them I would recommend you simply delete their whole lines from your header.


## R Markdown

Another reason I am asking you to write in Markdown is that understanding these conventions will make it much easier for you to write about computer code. Once we start working with R in our coding sessions, we will use [R Markdown](http://rmarkdown.rstudio.com/) for writing up anything that includes R code. Essentially, R Markdown blends the markdown conventions you are learning today with a few customizations that let you embed snippets of code, as well as any outputs (e.g. graphs, maps) produced by that code into Markdown documents. This lets you weave together prose and code, so your readers can see the technical aspects of your work while reading about their interpretive significance. We will talk about this more in the near future (and you'll see some examples of R Markdown), but I want you to understand that we are learning Markdown both for its flexibility in representing the typical kinds of texts literature students write *and* for writing about code.

 