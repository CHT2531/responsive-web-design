# Responsive Web Design

* Download the repository.
* Unzip the files, open the HTML page in a text editor and in a web browser.
* Make sure you are using responsive design mode in the browser.
* Apply some basic CSS e.g. simple typography, colours etc. A couple of rules is fine.
* Put an outline around each of the different content blocks:
    * holder
    * img_holder
    * intro
    * industry
    * sport
    * famous-people
* Add some padding to each block. It's probably a good idea to also change the ```box-sizing``` to be ```border-box```. This tells the browser to include padding and borders in the width of elements. See https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing for more info.

* Add a viewport meta tag to the head of document.
```
<meta name="viewport" content="width=device-width, initial-scale=1">
```
* Refresh the page and make sure you can see the effect of the viewport tag.
* Now think about using some simple media queries to specify additional CSS rules
  * Using the browser resize the page and pick a breakpoint. As a guideline, a column should be approx. 8-10 words in width.
  * Create a new CSS file
    * Add a single, simple CSS rule in this file to change the background colour of the page. This is just so you can test the media query works.
    * Add an additional link element in the head of the HTML document that will use this CSS file when the browser width hits your breakpoint e.g.
    ```
      <link rel="stylesheet" media="(min-width:572px)" href="css/style-wide.css">
    ```
  * Refresh the page in a browse and test this works
* Now think about how the layout might change when the screen size is wider
  * Use the CSS flexbox to try and create a two columned design.
* At some point when the screen size is really wide (greater than about 900px) we don't want the design to re-size any further. Create another breakpoint so that when the screen size is bigger than 900px the design doesn't get any bigger.
* Now turn your attention to the image.
  * You might find that at some points it overlaps other page elements. Have a look at using the *max-width* property to see if you can make the image stay within it's container.
  * It would be good if the image was centred when in a single columned design. Add some CSS so that image always sits in the centre of the design.
  * If you look in the images folder, you should be able to find a larger version of the Northumberland Street image. have a look at using the *picture* element to use the larger image when in the two-columned layout.
