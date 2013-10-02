Lesson 2 - Mark-up vs. Presentation
=====================================

Goal:  To understand the difference between what we see in our HTML text file and what we see in the browser window when we display the HTML file.

#### Step 1:  Create the following page:

	  This is 
	  a file
	  with 
	  many
	  lines of
	  text.

Save it and load it in your browser.  You might be surprised to see the results look like this:

	This is a file with many lines of text.
	
What's going on here?  In order to show an HTML page, the web browser has to read the page and look for tags that it is supposed to process.  While its doing that, it throws away any spaces return characters, replacing them with basically just one space.  So all our text in our file gets displayed as just a normal sentence by the browser.

#### Step 2:  Getting our lines split apart for real 

When we want our text to really start on a new line, we use the line break HTML tag to tell the browser what to do.  Change your file to look like this:

	This is 
	a file
	with <br>
	many
	lines of
	text.

When you run it now, you will get two lines.  The first will have everything before the line break (`<br>`) and the second will have everything after it.

#### Step 3:  Using paragraphs

Just like in a book, we can create paragraphs with HTML tags.  Try the following example which uses the paragraph tags (`<p>` and `</p>`):

	<p>I have something important to say.  Soon I will tell you what it is.</p>
	<p>Actually, I think I forgot what I was going to say.</p>

#### Step 3:  Headers and horizontal lines

We can put titles in our HTML pages and draw a line to separate two sections using a couple more tags.  Update the previous example to look like this:

	<h1>Listen up!</h1>
	<p>I have something important to say.  Soon I will tell you what it is.</p>
	<hr>
	<p>Actually, I think I forgot what I was going to say.</p>

The header tags (`<h1>` and `</h1>`) put a big title on the page.  The horizontal rule (`<hr>`) tag drew a line to further separate our two paragraphs.

Awesome!  We've come a long way really quickly.  We now have a good understanding of how what we type is changed into what we see in the browser.  We have also learned a bunch of cool new HTML tags to use in making our pages pretty.

