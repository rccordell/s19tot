---

#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: 8155665827_08680a7ca1_o.jpg
  caption: Creative Commons licensed photograph "Letterpress" by Flickr user Livy
  caption_url: https://flic.kr/p/dqFVj4
widget1:
  title: "Course Description and Objectives"
  url: '/description/'
  image: Le_diverse_et_artificiose_machine.jpg
  text: 'In ToT we will study the long history of new media, asking how technologies should shape our understanding of texts and the people who write, read, and interpret them. Many debates that seem unique to the twenty-first century—over privacy, intellectual property, information overload, and textual authority—are but new iterations of familiar battles in the histories of technology, new media, and literature…'
widget2:
  title: "Assignments"
  url: '/assignments/'
  video: '<div>
        <!-- <iframe width="182" height="182" src="/images/zoetrope2.mp4" frameborder="0" allowfullscreen></iframe> -->
        <video width="302" height="302" controls loop autoplay>
            <source src="/images/zoetrope.m4v" type="video/mp4">
        </video>
        </div>'
  text: 'Technologies of Text is an experiential, lab-based course. Students complete a wide range of assignments from setting type on a letterpress printer to coding a literary bot in the R programming language (& much more in between)…'

widget3:
  title: "Course Policies"
  url: '/policies/'
  text: 'Location: Barrs Room (472 Holmes Hall)<br />
  Teacher: <a href="http://ryancordell.org" target="_blank">Ryan Cordell</a> (<a href="mailto:r.cordell@northeastern.edu" target="_blank">email</a>)<br />
  Cordell Office: 415 Nightingale<br />
  Cordell Office Hours: Thursday 10am-noon, Friday 11:30am-12:30pm, and by appointment
  <hr>
  Section 1: Tuesday-Friday 9:50-11:30am<br />
  Practicum Student: <a href="mailto:quinn.wi@husky.neu.edu" target="_blank">Bill Quinn</a>
  <hr>
  Section 2: Tuesday-Friday 1:35-3:15<br />
  Practicum Student: <a href="mailto:medina.d@husky.neu.edu" target="_blank">David Medina</a>
  <hr>'
  image: 4917215160_85bfa9e75c_b-302x182.jpg


#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: /schedule/
  text: Go to the daily schedule &#9758;
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true

---

<!-- <div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://youtu.be/3OV5mWQc7II" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div> -->
