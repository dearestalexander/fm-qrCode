# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Questions and thoughts](#questions-and-thoughts)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![](./screenshot.png)

### Links

- Solution URL: [Github Repository](https://github.com/dearestalexander/fm-qrCode)
- Live Site URL: [Github Pages Live View](https://dearestalexander.github.io/fm-qrCode/)

## My process

### HTML / structure

- Starting from `<body>`:
  - Add one `div` for the white box.
    - Add `img` for the QR code 
    - Add `h1` for "Improve your front-end..." text 
    - Add `p` for "Scan the qr code... " text
- Note I left the .attribution div in the design.

### CSS / styling:

Preparation:

- To start I applied some CSS to normalise the body::
  - Margin & padding to 0, width and height to 100vw/vh, overflow to hidden
- Next I set up every style input as a variable
  - All colors plus font family, size and weights. Maybe this is overkill for this excercise, but I wanted to devlop a habbit of using variables.
- I added the stylesheet link to the HTML for the google font 'Outfit'

Styling:

- White box 
  - Positioning:
    - To centre vertically & horiztonally I used absolute with top/left 50% and transform -50%
  - Sizing:
    - For desktop: used %vw, estimated to be 20% of view width
    - For mobile: specified 325px and put both 20vw and 325px within Max()
  - Others:
    - Set border radius to 15px
    - Set display as flex in order to use align-items: center for the children.

- QR code
  - Sizing: Set witdth to 90% of it's container, leaving 5% white space each side
  - Added margin-top of 5% to match sides

- h1
  - Sizing: set width to 80% (a bit less than QR code)
  - Set font family/weight, color as per specifications
  - Text-align to center
  - Took a guess on font-size as 20px
    - I put this in a max(20px, 1rem) for accessibility consideraitons.
  - Set margin top to try and mirror specification spacing.

- p
  - Similar settings to h1, but with specific font size of 15px
  - Set margin bottom to 10% to try and mirror specification spacing

 
### Built with

- Plain CSS (it's on my to do list to learn SCSS)
- Flexbox
- Heavy use of variables? Maybe overkill for this exercise.

### What I learned

- I learnt how to control git via terminal and use github pages

For HTML and CSS the points I had learned during freeCodeCamp's responsive web design seemed to be enough to create a basic version of this. I did have to brush up on a few points:

- The structure of the links for google fonts
- Using max() with font sizes
- Everytime I use flexbox I need to remind myself on justify-content vs. align-items etc. 

### Questions and thoughts

- Is `<div>` the right element for the white box or maybe `<section>` is more appropriate?
- I set the white box size as a % of viewport, then set the QR to scale with it. 
  - Alternatively is there a benefit to setting fixed sizes for the QR code (mobile and desktop) for  and having the other elements scale with it?
- The specification includes paragraph at 15px, is this okay from an accessibility standpoint?
  - Should we not design with minimum 16px text? Also I wondered whenever specifying text size in px, should we do something like max(15px, 1rem) in case the individual has increased their browswer font size due to eyesight issues?

### Continued development

I think as this is only an introductory exercise there isn't anything specific to think about.

### Useful resources

I took detailed notes while working through freeCodeCamp and created my own reference which I used when working on this haha

[my quick reference](https://raw.githack.com/dearestalexander/RWBQuickRef/main/rwb.html)

## Author

- Website - [Alexander Roan](https://www.alexroan.com)
- Frontend Mentor - [@dearestalexander](https://www.frontendmentor.io/profile/dearestalexander)
- Twitter - [@xander_roan](https://x.com/xander_roan)

## Acknowledgments

I just want to thank everyone at frontend mentor for putting this together. The HTML and CSS wasn't too challenging for this introductory exercise, but it was the first time I set up Git and used it from terminal. The instructions and links were very helpful. This first challenge also helped me to get into the mindset of creating little projects and referencing my notes and refreshing on things. I also enjoyed the process of trying to build something from a design image, it's a bit like a puzzle!
