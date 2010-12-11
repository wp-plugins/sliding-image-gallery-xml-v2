=== Sliding Image Gallery XML v2 ===
Contributors: flashblue
Tags: image, gallery, font, flashblue, css, color, blur, alpha, xml, sliding, slide, showcase, scroll, radius, product, mouse, wordpress, joomla, plugin, module
Requires at least: 2.8.0
Tested up to: 3.0.3
Stable tag: trunk

Dynamic sliding image gallery for product showcase.

== Description ==

You can do following with XML:

* First visible item
* Rounded corner radius
* Transition type to x, y or alpha. (Default value is y).
* Duration / delay time of each item
* Show / hide buttons
* Show / hide content
* Set blur values (0 to not blur)
* Content background alpha, bgcolor, bottom padding
* Rollover, rollout, selected color of texts on buttons
* Color - font size of title & description contents
* CSS file path
* Includes WordPress plugin & Joomla module

You can change button positions to left or right by XML.

Auto-scroll just appears if you enter more than 5 items. 

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. Create a new folder inside your **wp-content** folder called **flashdo**, inside this folder create a new one called **flashblue**, inside this folder create a new one called **sliding-image-gallery-xml-v2** and copy files under **deploy** folder there
2. If you copied the **deploy** to a location different than the one above, go to **Sliding Image Gallery XML v2** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
3. Add `[sliding-image-gallery-xml-v2][/sliding-image-gallery-xml-v2]` where you want the Flash to show up in your post/page
4. If you want to make the Sliding Image Gallery XML v2 part of your theme, edit the template files and add `<?php slidingimagegalleryxmlv2_echo_embed_code(); ?>` where you want it to show up
5. Modify the `banner.xml` content and use it to overwrite `wp-content/flashdo/flashblue/sliding-image-gallery-xml-v2/xml/banner.xml`
6. To use your own images / swf, upload them to `wp-content/flashdo/flashblue/sliding-image-gallery-xml-v2/images/`

= Additional settings file =

To embed the Sliding Image Gallery XML v2 more than once, you will need another settings file. Let's assume your new file is called `banner2.xml`. Add `[sliding-image-gallery-xml-v2 xmlUrl="xml/banner2.xml"][/sliding-image-gallery-xml-v2]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `slidingimagegalleryxmlv2_echo_embed_code()` function call (for example `<?php slidingimagegalleryxmlv2_echo_embed_code("xml/banner2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[sliding-image-gallery-xml-v2]` and `[/sliding-image-gallery-xml-v2]`. If you made the Flash part of your theme, add the text as **the second argument** of the `slidingimagegalleryxmlv2_echo_embed_code()` function call (for example `<?php slidingimagegalleryxmlv2_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[sliding-image-gallery-xml-v2 width="590" height="300"][/sliding-image-gallery-xml-v2]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `slidingimagegalleryxmlv2_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 590 and 300 are just examples.

== Screenshots ==

1. You can view the live demo on [flashdo.com](http://www.flashdo.com/item/sliding-image-gallery-xml-v2/56 "Sliding Image Gallery XML v2") for Sliding Image Gallery XML v2.