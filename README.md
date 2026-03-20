# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page.
- View the optimal layout for the interface depending on their device's screen size.

### Screenshot

![Design screenshot](https://github.com/TheCoder-Rahul/fontend_mentor_blog_prev_card/blob/main/project_screenshot.png)

### Links

👉 [Solution URL](https://github.com/TheCoder-Rahul/fontend_mentor_blog_prev_card.git)
👉 [Live Site URL](https://thecoder-rahul.github.io/fontend_mentor_blog_prev_card)

## My process

### Built with

👉 **Markup:** Semantic HTML5 for better accessibility and SEO.
👉 **Styling:** CSS3 with Custom Properties (variables) for a maintainable color scheme.
👉 **Layout:** Flexbox for centering the card and managing the internal alignment.
👉 **Typography:** Local font integration using @font-face for performance and privacy.
👉 **Workflow:** Mobile-first approach and Responsive Design using Media Queries.

### What I learned

In this project, I focused on improving my asset management and interactive styling. Key takeaways include:

👉 **Local Font Integration:** I learned how to host font files locally using the `@font-face` rule to ensure consistent rendering across all devices.
👉 **Interactive States:** I implemented smooth CSS transitions for hover effects, enhancing the tactile feel of the card.

```html
<section class="blog-card">
  <img class="blog-thumbnail" src="./assets/images/illustration-article.svg" alt="Blog Preview Card Image">
  <div class="blog-details">
    <span>Learning</span>
    <p>Published 21 Dec 2023</p>
    <h1>HTML & CSS foundations</h1>
    <p class="description">These languages are the backbone of every website, defining structure, content, and presentation.</p>
  </div>
  <div class="author">
    <img src="assets/images/image-avatar.webp" alt="Blog Author Image">
    <p>Greg Hooper</p>
  </div>
</section>
```
```css
@font-face {
  font-family: 'Figtree';
  src: url(assets/fonts/static/Figtree-Medium.ttf) format('truetype');
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}
@font-face {
  font-family: 'Figtree';
  src: url(assets/fonts/static/Figtree-ExtraBold.ttf) format('truetype');
  font-weight: 800;
  font-style: normal;
  font-display: swap;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  height: 100vh;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  font-family: 'Figtree', sans-serif;
  background-color: hsl(47, 88%, 63%);
}
.blog-card {
  display: flex;
  padding: 24px;
  row-gap: 24px;
  font-size: 12px;
  font-weight: 500;
  overflow: hidden;
  line-height: 150%;
  border-radius: 20px;
  flex-direction: column;
  width: min(384px, 87%);
  color: hsl(0, 0%, 7%);
  border: 1px solid hsl(0, 0%, 7%);
  background-color: hsl(0, 0%, 100%);
  box-shadow: 8px 8px 0 hsl(0, 0%, 0%);
  -webkit-transition: all 0.3s ease-in-out;
  -moz-transition: all 0.3s ease-in-out;
  -ms-transition: all 0.3s ease-in-out;
  -o-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}
.blog-card:hover {
  box-shadow: 12px 12px 0 hsl(0, 0%, 0%);
}
.blog-card:hover .blog-details h1 {
  color: hsl(47, 88%, 63%);
}
.blog-card .blog-thumbnail {
  width: 100%;
  height: auto;
  border-radius: 10px;
}
.blog-card .blog-details {
  display: flex;
  row-gap: 12px;
  flex-direction: column;
}
.blog-card .blog-details span {
  font-weight: 800;
  padding: 4px 12px;
  border-radius: 4px;
  width: fit-content;
  background-color: hsl(47, 88%, 63%);
}
.blog-card .blog-details h1 {
  font-size: 20px;
  font-weight: 800;
  -webkit-transition: all 0.3s ease-in-out;
  -moz-transition: all 0.3s ease-in-out;
  -ms-transition: all 0.3s ease-in-out;
  -o-transition: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}
.blog-card .blog-details .description {
  font-size: 14px;
  color: hsl(0, 0%, 42%);
}
.blog-card .author {
  display: flex;
  column-gap: 12px;
  align-items: center;
}
.blog-card .author img {
  width: 32px;
  height: 32px;
  border-radius: 50%;
}
.blog-card .author p {
  font-size: 14px;
  font-weight: 800;
}
.attribution {
  bottom: 1rem;
  font-size: 11px;
  text-align: center;
  position: absolute;
}
.attribution a {
  color: hsl(228, 45%, 44%);
}
@media (min-width: 768px) {
  .blog-card .blog-details h1 {
    font-size: 24px;
  }
  .blog-card .blog-details .description, .blog-card .author p {
    font-size: 16px;
  }
}
```

## Author

👉 GitHub - [TheCoder-Rahul](https://github.com/TheCoder-Rahul)
👉 Frontend Mentor - [@TheCoder-Rahul](https://www.frontendmentor.io/profile/TheCoder-Rahul)
👉 LinkedIn - [@Rahul Kumar](https://www.linkedin.com/in/rahul-the-developer/)
