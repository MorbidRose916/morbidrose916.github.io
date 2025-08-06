---
layout: page
title: Excursion
description: CodeCademy Off-Platform website project
img: 
importance: 1
category: work
related_publications: true
---

In this project, I had to create a web page which advertises a product called “Excursion.” From start to finish using HTML, CSS, Command Line Interface, Git, and GitHub.

The web page needed to advertise a mobile app which helps users record and share their experiences, using a video and landscape imagery to set the scene. 

I had built a landing page since it's a vital tool in marketing a product these days, the goal will be to entice potential customers into using the product.

The files given to me were:

Images:
    - camp.jpg (Tents in the dirt, at night) 
    - phone.png (small white smartphone icon)
Video:
    - excursion.mp4 (smartphone framed video of nature) 

*I would rather have shown the files rendered w/ their name captioned underneath. Something going on that I can't quite figure out yet.*


Below is the HTML:
{% raw %}

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="resources\css\style.css" />
    <title>Excursion</title>
  </head>
  <body>
    <h1>Discover hidden places in the world around you</h1>
    <a href="#">Download Excursion (Coming soon!)</a>

    <div class="phone-vid">
      <video autoplay loop muted playsinline>
        <source src="resources\videos\excursion.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
    </div>

    <div class="section">
      <h2>Your personal travel guide</h2>
      <p class="subtitle">
        Excursion remembers places you like, and recommends new points of
        interest around you.
      </p>
      <img
        src="resources\images\camp.jpg"
        alt="Tent at night"
        class="camp-img"
      />
    </div>

    <div class="section">
      <div class="icon">
        <img src="resources\images\phone.png" alt="phone-icon" />
      </div>
      <h2>Coming Soon for iPhone and Android</h2>
      <a href="#">Download Excursion (Coming soon!)</a>
    </div>

    <div class="footer">© Excursion</div>
  </body>
</html>
```

Below is the styling:

```css
body {
  margin: 0;
  padding: 0;
  background-color: black;
  color: white;
  font-family: Verdana, Tahoma, sans-serif;
  text-align: center;
}

h1 {
  font-size: 50px;
  margin-top: 40px;
}

h2 {
  font-size: 42 px;
  font-weight: 300;
}

h2 p {
  font-size: 21px;
  color: #808080;
}

a {
  color: #7fffd4;
  text-decoration: none;
  font-size: 16px;
}

a:hover {
  text-decoration: underline;
}

.phone-vid {
  margin: 20px 0;
}

.section {
  margin: 60px 20px;
}

.subtitle {
  color: gray;
  font-size: 0.9em;
  margin-top: -10px;
  margin-bottom: 40px;
}

.camp-img {
  width: 90%;
  max-width: 800px;
  border-radius: 8px;
}

.icon {
  font-size: 3em;
  margin: 20px 0;
}

.footer {
  text-align: right;
  margin-top: 40px;
  font-size: 0.7em;
  color: #808080;
}
```

A preview of the page is available [here!](https://content.codecademy.com/programs/freelance-one/excursion/index.html?_gl=1*1f0xdsd*_gcl_au*MTk1NDM0OTYwOS4xNzUzNzk1OTczLjE1NDg5NDAzODIuMTc1NDMzMDUxMC4xNzU0MzMxNTcw*_ga*MTM1MjM0MjE2OS4xNzUzNzk1OTcz*_ga_3LRZM6TM9L*czE3NTQ0OTkxMjYkbzEzJGcxJHQxNzU0NTAxMzAzJGo1MiRsMCRoMA..)

{% endraw %}
