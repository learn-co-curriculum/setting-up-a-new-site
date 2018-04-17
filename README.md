# Setting up a New Site

## Objectives

1. Learn a basic file structure of a static HTML website

## Overview

We will be creating a website for a fake real estate company called 'Exceptional
Realty Group.' To begin, we will set up a basic file structure.

## Setting Up Site File Structure

Let's start by creating some initial folders and files to help organize us as we
grow our website. Note: if we were so inclined, we could program everything for
our new site in a single HTML file! As programmers, a file structure is valuable
for a few reasons:
  - it keeps us organized by separating discrete parts of our program
  - by following a general pattern, it allows other programmers (and programs!) to quickly understand and interface with our code

Before anything else, let's create a directory that will act as our website's
root directory. In the terminal, create a project folder (`mkdir
exceptional-realty`) and navigate into it (`cd exceptional-realty`). Since,
(being the passionate real-estate tycoons that we are), our hearts have been set
on building this website for awhile, we have a good idea of what we want it to
do. We would like our website to have the following discrete components:
  - a main page
  - a contact page
  - a page to report on the state of the real estate market
  - a page to show all real estate listings we currently have up
  - a page to show new properties on the market

Let's create some basic files with the `touch <file>` command that can house the
HTML for each of these views. Once created, each file should appear in the file
tree as a child of the `exceptional-realty/` directory:
  - `index.html`
  - `contact.html`
  - `market-report.html`
  - `new-properties.html`
  - `real-estate-listings.html`

In addition to keeping us organized, naming these files based on what they will
contain can also help when it comes to search engine optimization. Many search
engine strategies can use file names to find relevant information. Finally,
let's follow best practices and create an empty `README.md` file so that other
programmers can have some introduction and context when looking at our project.

### Making Room For Image Assets

Being a real estate website, we know we will need have images of our properties
on our website to keep our viewers interested. After all, not everyone in this
modern day has the patience (no matter how engaging the content is) to read a
[text only site.][stallman-posix]

We will want a separate folder for storing some image files. Create an `images`
directory using `mkdir`. It should be a child of our websites root directory
(`exceptional-reality/`). Let's go ahead and add an image to this folder. You
may be used to downloading images off the internet by simply navigating to that
image, right clicking, and saving the file. Instead, let's employ a special
terminal command that does the same: `wget`. First, though, we need an image.
Since we're building a real estate website, let's use the image found at this
url:
`http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/intro-pic.jpg`:

![Intro Pic](http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/intro-pic.jpg "Intro Pic")

Copy the full url path of the image, navigate (`cd`) into your `images` folder,
and: `wget <url>`.

The file `intro-pic.jpg` should appear in `images/`. You may not be able to view
this image directly, but that is fine; if we have copied from the correct url we
can still use it in our site.

### Testing our Website Using `httpserver`

While we build our website and add content, we need to be actively checking to
see what the actual site looks like. In the Learn IDE, we can use a tool that is
already built in, `httpserver`!

* Navigate out of the `images` folder using `cd ..`, so you are in your main `exceptional-realty` folder (you can check where you are anytime with the `pwd` command)
* In your terminal, type `httpserver` and press `return`.
* You will see a message `Your server is running at ...`, followed by a string of numbers, with periods and a colon. Copy that string, open a new tab, and paste
* At this point, you should see a blank page because we don't have anything in `index.html`. Go ahead and add a line to the `index.html` just to make sure everything is working properly. For example, `hello world!` and restart your `httpserver`. (to stop `httpserver`, make sure your terminal is in focus and press `control` + `c`)
* Now, when go the url, we should see that line in the browser!
* Let's also make sure our image files are being served by adding the following to the end of the url: `/images/intro-pic.jpg`
* If all is well, the image we retrieved using `wget` should appear

## Looking Forward

In the upcoming labs, we will be building this website step by step. You will be
introduced to various HTML concepts and components while applying them your
site. Each lesson will contain up-to-date starter code so we can focus on the
discrete skill of the lesson in context of our growing website.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/setting-up-a-new-site' title='Setting up a New Site'>Setting up a New Site</a> on Learn.co and start learning to code for free.</p>

[stallman-posix]: https://stallman.org/articles/posix.html
[sb]: http://help.learn.co/ide-in-browser/ide-in-browser-sandbox
