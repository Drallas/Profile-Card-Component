# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)



## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- BEM CSS
- Mobile-first workflow

### What I learned

**Dual Background** 

I never used it, so i had to research it a bit. Main question marks, "should i set dual background image and how do i position them"? It's Possible and not that hard.

```css
#example1 {
  background-image: url(img_flwr.gif), url(paper.gif);
  background-position: right bottom, left top;
  background-repeat: no-repeat, no-repeat;
}
```

**Background Position**
Setting the background-position was more tricky, but with some trial and error i ended up with this code.

```css
background-position: left -40rem top -30rem, right -40rem bottom -30rem;
```

**Card Picture**

Had to figure out how to place picture and make it overflow the card background. 

```css
box-sizing: content-box;  # To exclude the 5px border box size.
position: absolute;	# To give the initial postion.
transform: translate(-50%, -100%); # To move it over to the correct spot.
```

### Continued development

I still struggle with the many options to layout and position divs, other point of improvement are that i struggle a bit with correct BEM class naming; i'm going to ask some advice. For the card rem value's didn't work so good and px seemed to be better to recreate the card exact (almost pixel perfect).

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@drallas](https://www.frontendmentor.io/profile/drallas)

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.
