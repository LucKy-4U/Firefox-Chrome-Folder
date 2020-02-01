My Firefox Version is 70.0, using ElementaryOS--a flavor of Ubuntu 16.04.5 LTS.

Inside your Firefox profile folder, paste this chrome folder and then in firefox browser, go to about:config and set toolkit.legacyUserProfileCustomizations.stylesheets to TRUE. Restart Firefox.

MyFirefoxScreenshot_WithoutTheTucking.jpg: This screenshot shows what my firefox looks like with the userChrome.css file given in the folder, ie, without the tucking.
sorry, I forgot how I got firefox to tuck at the bottom, ie, firefox going inside a frame or something when I added -34px in userChrome.css. I tried various things but couldn't do it again. :((

But Thanks to you making me make this repository. :P :)) I was able to resolve the full_screen issue by adding the below code:

#main-window {
    min-height: 900px !important;
    max-height: 900px !important;
} /*you can check the height of your display size and change the pixel number accordingly. :)*/

but this gave me one more issue: At certain places, Firefox going outside the visible screen. :((
CustomizationView_WithoutButtonsAtTheBottom.jpg: This screenshot shows the customization view of firefox. Notice how the buttons at the bottom are only half visible?
CustomizationView_WithButtonsAtTheBottom.jpg: This is a screenshot of how it is supposed to look like. :((

Firefox_WithLastTabHalfVisible.jpg: Notice how at the bottom of the TreeStyleTab you see only half of the last open tab?

WELL, THE GOOD NEWS IS THAT I WAS ABLE TO RESOLVE ALL THESE ISSUES WITH A PRETTY STUPID TRICK. :P

just do the min-height and max-height thing, then when the full screen shows up. kill firefox and edit userChrome.css, remove min-height and max-height settings and replace them with height: 900px !important; Restart Firefox and voila, it's all fixed up. :P

Solved_Perfect.jpg: This screeenshot shows my firefox, all fixed up. :))

shoot me up if you have any questions. :))
also, if you experiment with this all and are able to fix firefox without my stupid trick, please do let me know. :)) Thanks a lot for your help. :))
now, if you can figure out how to expand the TreeStyleTab to grab the entire right side of the screen and how to shrink the navigation bar to the right to make space for the TreeStyleTab then that would be a huge huge bumper help. :))
and hey, it would also make your firefox and many other's firefox much better and easier to use. :))
still, Thanks a lot for your help. :))

