name: My Travel Site
owner: AkkuuPlayzz
repo: my-travel-site
url: https://akkuuplayzz.github.io/my-travel-site/
branch: main

structure:
  root:
    - index.html
    - style.css
    - fruit.png
    - mountain.jpg
    - temple.jpg

html:
  title: My Travel Website
  sections:
    - navbar:
        links:
          - Home
          - Places
          - Contact
    - header:
        headline: Places to Explore in the Hills
        description: Discover hidden gems in India’s mountains...
    - cards:
        places:
          - Fruit Village
          - Snowy Mountain
          - Kedarnath Temple
    - contact:
        info:
          - phone: +91 7302017538
          - email: quotesmotivation409@gmail.com
          - whatsapp: https://wa.me/917302017538
        form:
          service: Formspree
          action: https://formspree.io/f/xnnvlnjg
          method: POST
          fields:
            - name
            - email
            - message
          spam_protection:
            honeypot: true
            recaptcha:
              enabled: true
              site_key: YOUR_SITE_KEY
    - footer:
        copyright: © 2025 Akash Rawat | All rights reserved.

css:
  fonts: Arial, sans-serif
  colors:
    background: #ffffff
    text: #333
    primary: #0d47a1
    card-bg: #f9f9f9
    contact-bg: #e3f2fd
  layout:
    responsive: true
    flexbox: true
    card-width: 300px
    form-max-width: 500px

deployment:
  platform: GitHub Pages
  config:
    source:
      branch: main
      folder: /
    status: enabled

notes:
  - Make sure images are uploaded at root level or update paths
  - Replace YOUR_SITE_KEY with actual Google reCAPTCHA key
  - Enable GitHub Pages from repo Settings > Pages
