=== Countdown FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, count, down, countdown, free, flash, effect, animation, xml, as3, clock, time
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced Countdown on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. It's a completely customizable flipping countdown clock. The general width and height and each item's width and height can be easily modified. It can show/hide the days, hours, minutes and seconds and arrange them in any order. It has shadow properties available like distance, color, angle, alpha, blur with customizable font faces, colors and sizes.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/countdown-fx.zip "Countdown FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/countdown.zip "Countdown FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **countdown-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Countdown FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[countdown-fx][/countdown-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Countdown FX part of your theme, edit the template files and add `<?php countdownfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Countdown FX](http://www.flashxml.net/countdown.html "Countdown FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/countdown-fx/settings.xml`

= Additional settings file =

To embed the Countdown FX more than once, you will need another settings file. Let's assume your new file is called `settings2.xml`. Add `[countdown-fx settings="settings2.xml"][/countdown-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `countdownfx_echo_embed_code()` function call (for example `<?php countdownfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[countdown-fx]` and `[/countdown-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `countdownfx_echo_embed_code()` function call (for example `<?php countdownfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[countdown-fx width="600" height="300"][/countdown-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `countdownfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/countdown.html "Countdown FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/countdown-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/countdown.html "Countdown FX") is the utility that helps easily customize your Countdown FX to fit all your needs.