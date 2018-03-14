# Setting up a New Site

**Note for In-Browser Learn IDE Users:** Some steps in this video will be
different when using the in-browser IDE. If you would like to code along during
this lesson, please refer to the notes below the video for more information.

**Note for stand alone Learn IDE Users:** You do not need iTerm or Sublime. You
can run all commands and perform all actions in the IDE terminal and text
editor. To add images, right click on the directory you'd like to add them to
(in the tree) and select 'Import'.

<iframe width="640" height="480" src="//www.youtube.com/embed/i61lTJ6OpDE?rel=0&modestbranding=1" frameborder="0" allowfullscreen></iframe>

[Alternate video link.](https://www.youtube.com/watch?v=i61lTJ6OpDE)

[Click here to save the intro pic used in this code along.](http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/intro-pic.jpg)

[Here is a direct link to the gitignore code referenced in the video.](https://gist.githubusercontent.com/octocat/9257657/raw/3f9569e65df83a7b328b39a091f0ce9c6efc6429/.gitignore)

#### Notes for In-Browser Learn IDE Users

* To get started, click `OPEN IDE` to clone down a copy of this lesson. Once
  cloned, you will be able to add folders and files, as well as practice git
  commands.
* Since you have already cloned down a copy of the lesson, you already
  have an initialized git repo. Running `git init` will work as normal, but
  trying to run `git remote add origin git@github.com:<YOUR_USERNAME>/exceptional-realty.git`
  will produce an error.
* To copy to a new git repository, `cd` to the main folder of your cloned
  lesson, then type `git remote set-url origin git@github.com:<YOUR_USERNAME>/exceptional-realty.git`
  into your terminal. Attempting to change your remote url from the folder
  `exceptional-realty` will produce an error.
* After setting your remote url, `git push -u origin master` will update your
  new repo on github.com.
* Images can't be downloaded to your in-browser IDE, so instead, you'll have to
  use a terminal command, `wget`, to retrieve the image file. Run the following
  in your terminal: `wget http://ironboard-curriculum-content.s3.amazonaws.com/front-end/lab-assets/intro-pic.jpg`.
  The image file will appear in whatever folder you are currently in in your IDE.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/setting-up-a-new-site' title='Setting up a New Site'>Setting up a New Site</a> on Learn.co and start learning to code for free.</p>
