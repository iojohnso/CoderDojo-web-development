Lesson 4 - Links and Images
===========================

Goal:  To expand our knowledge of tags allowing us to show pictures and link multiple HTML files together.

Introduction:  So far we have done some great things by marking up text.  Now its time to add pictures to our documents.  Then we're going to explore what makes the world wide web a web.

#### Step 1:  Lets continue with our existing application which should look like this:

	<h1 align="center">Listen up!</h1>
	<p>I have something important to say.  Soon I will tell you what it is.</p>
	<hr color="red" size="10" width="50%" align="left">
	<p>Actually, I think I forgot what I was going to say.</p>

At the bottom of the application, add this line:

	<img src="http://coderdojo.com/wp-content/themes/collective/images/logo.png">

That's a pretty ugly line but when you run it, you get pretty spectacular results - an image shows up at the bottom of our document.

Here's what happened:  

	<img> is just another HTML tag.  It says "put an image where this tag is".  
	And src is just an attribute that says what image to use.  
	
Just like all the different html pages on the web can be referenced by a URL (name), so can all the images.  We included an image from the CoderDojo site in the page we were making.


#### Step 2: Just like we can link in an image from another location, we can also link to another page.  For this, we use "anchor" tags (&lt;a&gt; and &lt;/a&gt;).

Type the following line at the end of your program and see what it does:

	<a href="http://coderdojo.com/">Go to the CoderDojo Page</a>

Here the anchor tag (&lt;a&gt;) needs an attribute named href.  Href stands for html reference and is the name of some page on the web.  In between the beginning and ending tags you put the text that you want the user to be able to select to go to the page.


#### Step 3:  Its not only text that can be used in anchor tags.  Replace the last two lines of your program with this combined version:

	<a href="http://coderdojo.com/">
		<img src="http://coderdojo.com/wp-content/themes/collective/images/logo.png">
	</a>

Now there is no text to click - just an image!  By wrapping the anchor around the image, we have created a clickable image that takes us where the anchor says to go.


Conclusion:  We've taken another big step forward with this lesson.  Now we are able to create colorful and creative pages with images from all over the web (or with our own images from our local computer).  We can also link our documents to other documents creating a "web" of pages that work together.
