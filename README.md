# My sixth project and solution to the profile card component challenge over at [Frontend Mentor](https://www.frontendmentor.io/challenges)

## This was the assignment

![](./design/desktop-design.jpg)

## This is my solution

[Click here to see the live page](https://arthurpog.github.io/profile-card-component/)

![](./design/Profile_%20card_component-my_solution.png)


This is my sixth project on my journey to learning HTML &amp; CSS while doing Frontend Mentor challenges.

My biggest challenge here was creating the backround bubbles so that they stay static and don't move around or resize.

I still haven't completely grasped how background images work 100% of the time, but this has shed some valuable light into the whole ordeal and so I will keep on experimenting.


Here's the bubble code:

First create a `div` or any block element in the HTML and classify it as `bubbles`. Then set the parent container's `position` to `relative` or `absolute`


| Syntax | Description |
| ----------- | ----------- |
|.bubbles {||
|opacity: .5;|50% transparency of the background.|
|position: absolute;|This will make it so the background "floats" above where it normal should be, thus helping us position it freely.|
|min-height: 100%;|Use the maximum height of the viewport.|
|min-width: 100%;| Use the maximum width of the viewport.|
|background-repeat: no-repeat;|Background repeats by default on the X and Y axis, this stops that.| 
|z-index: -1;|Moves the background behind everything else on the page. The Z axis is basically the layer axis of a page.|  
|background-attachment: fixed;|Makes the background static and stops it from moving when scrollin the page.|  
|background-image: url(./images/bg-pattern-top.svg), url(./images/bg-pattern-bottom.svg);|Here we bring in two images, the bubble on the top and the one on the bottom.|
|background-position: calc(50% - 490px) calc(50% - 400px), calc(50% + 470px) calc(50% + 430px);|This calculates positions for the top and bottom bubble using the calc function. Basically for the top bubble for example, it is starting from the middle horizontally (X axis, that's the first number, 50%) then it is subtracting 490px from it which moves it to the left 490px and then vertically in the middle 50%-4000px which moves it up along the Y axis.|
|}||
