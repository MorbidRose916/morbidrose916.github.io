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

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets\img\excursion_proj\excursion_redline_MOCK.png" title="excursion_redline_mock" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This is the designer mock to go off of.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

Below is the HTML:

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
