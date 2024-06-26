---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: splash

excerpt: "Welcome to the Lake"
header:
  overlay_image: /_lfs/images/lake_splash.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  #caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  #caption: "Photo credit: Josh Furman"
  actions:
    - label: "Member Login"
      url: https://members.lakecavanaugh.info

feature_row:
  - alt: "LCIA Membership"
    title: "Join the LCIA"
    excerpt: "**Sign up** or **renew** your LCIA membership or make a donation"
    url: /lcia/membership
    btn_label: "Join Today"
    btn_class: "btn--inverse"
  - alt: "Lake News"
    title: "News From the Lake"
    excerpt: "Find out about the latest news"
    url: /community/
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - title: "Events Calendar"
    excerpt: "Mark your calendars for new events at the lake!"
    btn_label: "Events"
    btn_class: "btn--inverse"
    url: /events/
  - alt: "Donate to the LCIA"
    title: "Donate to the LCIA"
    excerpt: "Help support the LCIA with a donation"
    url: /lcia/donations
    btn_label: "Donate Today"
    btn_class: "btn--inverse"
  - title: "Advertise Your Business"
    excerpt: "Help support the Lake Cavanaugh Improvement Association by advertising your business on the website and in the Newsletter."
    btn_label: "Learn More"
    btn_class: "btn--inverse"
    url: /sponsors/advertise
  - title: "Rent the Community Center"
    excerpt: "The Lake Cavanaugh Community Center is available to rent. Contact us now to coordinate your event."
    btn_label: "Learn More"
    btn_class: "btn--inverse"
    url: /lcia/cc_rental
---

{% include feature_row %}

{% include weather.html %}
