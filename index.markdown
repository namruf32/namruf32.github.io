---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: splash

excerpt: "Welcome to the Lake"
header:
  overlay_image: /assets/images/lake_splash.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  #caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  caption: "Photo credit: Josh Furman"
  actions:
    - label: "Member Login"
      url: /lcia/members/encrypted/

feature_row:
  - image_path: /assets/images/big_island.jpg
    alt: "LCIA Membership"
    title: "LCIA Membership"
    excerpt: "**Sign up** or **renew** your LCIA membership or make a donation"
    url: /lcia/dues
    btn_label: "Join Today"
    btn_class: "btn--inverse"
  - image_path: /assets/images/lake_splash-2.jpg
    alt: "Lake News"
    title: "News From the Lake"
    excerpt: "Find out about the latest news"
    url: /community/
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - image_path: /assets/images/northshore-768x576.jpeg
    title: "Events Calander"
    excerpt: "Mark your calendars for new events at the lake!"
    btn_label: "Events"
    btn_class: "btn--inverse"
    url: /events/
---    

{% include feature_row %}

<a class="weatherwidget-io" href="https://forecast7.com/en/48d33n122d02/lake-cavanaugh/?unit=us" data-label_1="LAKE CAVANAUGH" data-label_2="WEATHER" data-theme="original" >LAKE CAVANAUGH WEATHER</a>
<script>
!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src='https://weatherwidget.io/js/widget.min.js';fjs.parentNode.insertBefore(js,fjs);}}(document,'script','weatherwidget-io-js');
</script>
