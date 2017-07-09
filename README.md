# How to Make a Child Theme in WordPress #
---

> ### Why a Child Theme
> ---

A child theme is ALWAYS a good idea when using a theme for WordPress, quite simply so that when the theme updates, your WordPress site doesn't break as a result!

> ### Install WordPress ###
> ---

I like to have two installations, one for development, and a live one, usually set to an "Under Construction" type page until you are happy with the product.
Either way, setup is the same.  You can use something like XAMPP or anything that can serve files locally for testing and there are setups in AWS or similar server environments that can get your live site up and running and will have instructions there.  In the case of who this is actually for, his environment is already setup, and I can actually skip this part and... I'm going to.  ...I'm sorry.  To be honest, I just kind of wanted to make him read all of this for no reason.  Also, I thought having multiple sections in my README could be fun!

> ### Open Your Editor! ###
> *I want you to read that like its epic.  Like, "Start Your Engines!". Anyway...*
> ---

Don't be frightened though, I've already made the files for you and they are in the Repository.  The file is "Child Theme", and in it are two files:
* functions.php
* style.css

And its the style.css file you want to open.  Clone this Repo, and lets get started... I'll wait...







Ok. Looks like we're ready...
At the top of this document is a section completely commented out.  Leave it that way.

Currently, it looks like this...
```css
/*
 Theme Name:     Your Theme Name
 Description:    Describe Your Theme
 Author:         Your Name... or you know..whateva
 Author URI:     your website mabye. show off some stuff if they come lookin
 Template:       Divi
 Version:        1.0.0
*/
```

Everything should be changed except the Template (in the case of my friend), if you are child theming from a different parent theme, by all means, change it.

1. Theme Name - Give your theme a name
2. Description - Give it a small Description
3. Author - Put your name or Company Name for the Author
4. Author URI - Put a link to you or your company's website
5. Template - This is the most important one and MUST be included... without this it will not work.
6. Version - This is your version of child theme, not the parent. So if you're just starting the site, this probably does not need to change.

Once this is complete, save the file and then zip the folder up containing both your newly modified style.css and the functions.php file.

> ### Add to WordPress ###
> ---

Sign into the admin side of your WordPress and navigate to the Themes.  If you are installing your Parent Theme from a ZIP file (not child theme),
you will find the option to import the theme at the top of the page.  Click the Import Button, navigat to the parent theme .zip file, and select it.  WordPress will install the theme and automatically activate it.

Once your parent theme has been added, you can now follow the same process to import your child-theme!  Just make sure your child-theme is active before you start working.

> ### A Word... ###
> ---

Now, this will get you started, but of course... there's always more...

If you'd like to see all the options you can declare in the style.css header (there are more, things like License, and Tags, etc) or, maybe your parent theme css isn't acting quite right and you need to work something out this README file doesn't contain, you can find more information [HERE](https://codex.wordpress.org/Child_Themes).
