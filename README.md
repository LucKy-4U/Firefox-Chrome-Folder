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
CustomizationView_WithButtonsAtTheBottom.jpg is a screenshot of how it is supposed to look like. :((
