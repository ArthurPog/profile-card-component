# Profile Card Component Challenge Using Frontend Mentor

This is my sixth project on my journey to learning HTML &amp; CSS while doing Frontend Mentor challenges.

My biggest challenge here was creating the backround bubbles so that they stay static and don't move around or resize.

I still haven't completely grasped how background images work 100% of the time, but this has shed some valuable light into the whole ordeal and so I will keep on experimenting.

Here's the bubble code:

First create a `div` or any block element in the HTML and classify it as `bubbles`. Then set the parent container's `position` to `relative` or `absolute`

`.bubbles {`<br>
`&nbsp&nbspopacity: .5;`<br>
`&nbsp&nbspposition: absolute; /* This will make it so the background "floats" above where it normal should be, thus helping us position it freely. */`<br>
`&nbsp&nbspmin-height: 100%; /* asd */`<br>
`&nbsp&nbspmin-width: 100%; /* asd */`<br>
`&nbsp&nbspbackground-repeat: no-repeat; /* Background repeats by default on the X and Y axis, this stops that. */`<br>
`&nbsp&nbspz-index: -1; /* Moves the background behind everything else on the page. The Z axis is basically the layer axis of a page. */`<br>
`&nbsp&nbspbackground-attachment: fixed; /* Makes the background static and stops it from moving when scrollin the page */`<br>
`&nbsp&nbspbackground-image: url(./images/bg-pattern-top.svg), url(./images/bg-pattern-bottom.svg); /* Here we bring in two images, the bubble on the top and the one on the bottom */`<br>
`&nbsp&nbspbackground-position: calc(50% - 490px) calc(50% - 400px), calc(50% + 470px) calc(50% + 430px); /* This calculates positions for the top and bottom bubble using the calc function. Basically for the top bubble for example, it is starting from the middle horizontally (X axis, that's the first number, 50%) then it is subtracting 490px from it which moves it to the left 490px and then vertically in the middle 50%-4000px which moves it up along the Y axis. */`<br>
}`
