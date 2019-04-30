![Alt](../Assets/Images/gem.png "Big Shmeck")

# Welcome to the Big Shmeck Website project! #

During the course of this readme file I will be explaining the methods I have used to complete this project in a number of sections below.

The sections will be structured as follows:

###
1. Initial Concept
2. Ideas and First Attempts
3. Corrections and Mistakes
4. Final Website Design
#

## 1. Initial Concept #

The initial concept I had of this website was to have a sturdy header with a built in menu which will link you to other areas of the site. When viewing in mobile this would then condense down into a drop down menu which gave the same functionality. I would then use social media icons next to the header menu to promote my other social spaces such as Soundcloud / Instagram etc...

I would then have a video on the main page showing the latest music video I have put together.

Following this I would have a short biographical section explaining my motives as an artist and also a bit about myself.

Further down the page I would then have a 'Gigs' section which would show the shows I am yet to play throughout this year, these would also have buy links that would link you through to the relevant Ticketmaster page.

At the bottom of the screen, I would have a header which would show my social media links again.

The overall styling would have been black for headers, white for text, white / grey for section backgrounds and then a purple glow around most elements where it fit.

I also had the initial idea of having an intro screen which showed my logo, when clicked this would take you through to the main.html page of my website.

The additional page I also added was the Songs page which had embedded Spotify links from my Spotify page.


## 2. Ideas and First Attempts #

The first attempts were mostly made around the header and footer sections to make them work with links when in a full view of the screen, and to be in a dropdown menu when viewing in mobile.

~~~~html
<header class="container-fluid black">
    <div class="row header-height">
    <div class="">
        <a href="/main.html">
                <div alt="gem" class="small-logo"></div>
        </a>
        </div>
        <div class="artist-name">Big Shmeck</div>
~~~~

This is how the header started off bit this did not work as I intended to begin with and I was missing social links and the ability to move the social / page links into a dropdown for easier viewing on mobile.

I will go further into how I did this later, for now I would like to focus more on the body elements such as images, videos and the Songs page as well as the styles that were applied to these areas also.

When looking into my css file you will see that I have had to use quite specific styles in some areas. This was due to bootstrap pulling through a lot of unnecessary and unwanted styles in some areas. I would not leave these as they were and so I changed them to be more specific to my goal.

~~~~html
~~~~

~~~~css
.small-logo {
    background-image: url(../Images/gem.png);
    background-size: 90%;
    background-repeat: no-repeat;
    height: 80px;
    margin-top: 0px;
    margin-right:0px;
    width: 70px;
    position: relative;
}

.artist-name {
    color:black;
    font-family: 'Open Sans', sans-serif;
    font-size: 30px;
    font-stretch: expanded;
    letter-spacing: 2px;
    font-weight: lighter;
    padding-left:0;
    background-color: white;
    border-color: black;
    border-bottom-width: 2px;
    border-right-width: 2px;
    border-left-width: 2px;
    border-bottom-style: solid;
    border-bottom-color: purple;
    border-left-style: solid;
    border-right-style: solid;
    border-top-color: purple;
    border-top-width: 3px;
    border-top-style: solid;
    box-shadow: 2px 2px 5px #333444;
    text-align: center;
    transform: skewX(0deg);
    text-transform: uppercase;
    height:60%;
    -webkit-box-shadow: inset 3px 3px 79px -15px rgba((128,0,128,1));
    -moz-box-shadow: inset 3px 3px 79px -15px rgba(128,0,128,1);
    box-shadow: inset 3px 10px 27px -15px rgba(128,0,128,1);
    margin-left:5px;
    margin-top:17px;
}
~~~~

This corrected a lot of the problems caused by the sizing of the row / container-fluid classes.