---
layout: page
title: "Poetry Bot Prep"
subheadline: "Getting Ready for Next Week"
categories:
    - in-class
comments: false
show_meta: true
header:
  image_fullwidth: 4880254551_9a35151a0d_b-banner.jpg
  caption: Creative Commons licensed photograph, "Underwood," by Flickr user Canned Muffins
  caption_url: https://flic.kr/p/8rfzDR

---

There are a few things you can do to prepare for next week's poetry bot lab and ensure we can get started in short order. You’ll need to create a few accounts from which we’ll either be drawing or to which we’ll be adding data:

+ Sign up for [a Wordnik account](https://www.wordnik.com/signup) and then [sign up for a Wordnik API Key](http://developer.wordnik.com/). Wordnik is an open-source dictionary from which we will be drawing words to fill in our mad libs.
+ If you want to post to Twitter, you will need to create a new Twitter account for your bot. Think about what kind of bot you want to make and then sign up. Be sure to add a mobile number to the account, as we’ll need that for one the steps later on.
+ While signed into your new account, visit [Twitter’s Application Management site](https://apps.twitter.com). You will want to `Create New App.` Fill out the required fields and then click `Create Your Twitter Application.` Then click on the name of your new app, navigate to `Settings`, and set your app's `Callback URL` should be set to `http://127.0.0.1:1410`. Then navigate to `Permissions,` select `Read and Write,` and save settings. We’ll be getting some essential information from the `Keys and Access Tokens` menu during our Twitterbot lab.