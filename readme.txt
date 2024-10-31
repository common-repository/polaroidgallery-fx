=== Polaroid Gallery FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, polaroid, gallery, as3, image, effect, auto, xml, animation, html, css, photo, random
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

Probably the most advanced Polaroid Gallery on the web. Completely XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. It's completely customizable and it uses HTML/CSS formatted text. There are rotation and expanding scale properties of images as well as grid, random or desk layout for them. Effects like shadow and blur, many background and shade features are also available. Many other particular properties are available on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/polaroid-gallery-fx.zip "Polaroid Gallery FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/polaroid-gallery.zip "Polaroid Gallery FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **polaroid-gallery-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Polaroid Gallery FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[polaroid-gallery-fx][/polaroid-gallery-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Polaroid Gallery FX part of your theme, edit the template files and add `<?php polaroidgalleryfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Polaroid Gallery FX](http://www.flashxml.net/polaroid-gallery.html "Polaroid Gallery FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/polaroid-gallery-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/polaroid-gallery-fx/images/` and update the `wp-content/flashxml/polaroid-gallery-fx/images.xml` file accordingly

= Additional settings file =

To embed the Polaroid Gallery FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[polaroid-gallery-fx settings="settings2.xml"][/polaroid-gallery-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `polaroidgalleryfx_echo_embed_code()` function call (for example `<?php polaroidgalleryfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[polaroid-gallery-fx]` and `[/polaroid-gallery-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `polaroidgalleryfx_echo_embed_code()` function call (for example `<?php polaroidgalleryfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[polaroid-gallery-fx width="600" height="300"][/polaroid-gallery-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `polaroidgalleryfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/polaroid-gallery.html "Polaroid Gallery FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/polaroid-gallery-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/polaroid-gallery.html "Polaroid Gallery FX") is the utility that helps easily customize your Polaroid Gallery FX to fit all your needs.