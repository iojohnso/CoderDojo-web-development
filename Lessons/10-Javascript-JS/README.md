10 - Javascript 01:  Getting started and variables
===============================================

Goal:  For us to get some javascript running in a web page and to learn a new programming concept:  the variable.

Javascript is fun because its a "real" programming langauge.
HTML programming is fun but its mostly about presentations and layouts.  When we start adding Javascript to our files, we
have basically all the power of a complete language for expressing ourselves.


#### Step 1:  Create a page we're going to work with.

For this set of tutorials, lets create a new page.  Create a new page called:

  TestJavascript.html
	
In your new file, type the following code and then run it in the browser.

	<html >
		<head>
			<title>JavaScript Tutorial</title>
		</head>
		<body>
  	
			<H1>Javascript code coming soon!!!</H1>
	
			<script language="javascript" type="text/javascript">
				// here is where we will code...
				</script>
		</body>
	</html>


You should see this message:


	Javascript code coming soon!!!
	
Let's talk about what's going on here.  Almost everything we see here, you have already learned.  This is just 
a normal html document.  It has nothing to display but a simple header (h1 tag) to proudly announce that soon we
will be writing Javascript.

The cool thing about Javascript is that it works right in the same browswer that shows our HTML - without any changes.
So all we have to do learn the new tags for writing Javascript code (\<script\>\</script\>) and we are ready to start.

When the \<script> tag is seen, the computer switches from building web pages for you and starts building a Javascipt
program.  Right now, our program doesn't do anything at all except show a comment.  

Comments are notes that programmers write for themselves and others who have to look at the program later.  Comments 
help you remember what your program is supposed to do as it gets bigger and more complex.  The // characters means 
"everything from here to the end of the line is just a comment for me... please don't try to run it Mr Computer"

#### Step 2:  Variables

Boring!  You say to me.  Our program doesn't do anything new yet.  Ok, add the next 4 lines to your program 
(where the comment is):

	var favoriteNumber = 7;
	var favoriteColor = "Green";
	var pi = 3.14159;
	var iAmNice = true;
	
If you run it again, you will be amazed to see... absolutely nothing has changed.  But we have done something wonderful here.
We have created VARIABLES!  Varaibles are places in the computer to store information.  You can think of a variable a little 
like a suit case.  I create a suit case and then I can put something in it.  Later I can open up the suit case take 
whatever I put in it back out again.  Because programs need lots of information, we need lots of suitcases in most programs.
In order to keep track of all of our suit cases, we give them names.  In the example above, we created 4 different suit
cases and named them "favoriteColor", "favoriteNumber", "pi", and "iAmNice".

#### Step 3:  Writing something out to the screen

Boring!  You STILL say to me.  Ok, lets start doing something with our program that we can see.  Add the following lines
to our program after the variables have been created:

	document.write("My favorite number is " + favoriteNumber);
	document.write("My favorite color is " + favoriteColor);
	document.write("Pi is approximately  " + pi);
	document.write("Am I a nice person? " + iAmNice);

When you run the program now, you should get a long line of text that tells you all the variables.  But its ugly!  What happened?
Turns out that the document.write operation is creating more HTML in your page.  So if you don't give it any tags, it doesn't
know how to format what it sees.  So change the statements above in your program to look like this:

	document.write("My favorite number is " + favoriteNumber + "<br>");
	document.write("My favorite color is " + favoriteColor + "<br>");
	document.write("Pi is approximately  " + pi + "<br>");
	document.write("Am I a nice person? " + iAmNice + "<br>");

With that change, we get some nice output.  Now we can read the values from our four variables in our html file.  As you
can see, we use the plus sign (+) to paste together text and variables to make something to show on the screen.


#### Step 4:  Attributes and Functions

We have just one more concept to add to our first lesson on Javascript.  There are operations you can use on variables to 
to do different things.  HAdd the next two lines to your program and run it:

	document.write("My favorite color length is " + favoriteColor.length + "<br>");
	document.write("Part of my favorite color is " + favoriteColor.substring(2,4) + "<br>");

To keep it simple for now, we will leave it at this.  There's a lot of operations you can run on variables but help you 
along the way while you are programming.  

You might be interested to know that document is a variable too!  Its a varaible that got created automatically in the background
for you.  That's why you didn't need to add it to your program.  And write is just a function you can use with the document
variable that does work for you.  

Congratulations!  In this lesson, we have learned a huge amount about programming.  We're not ready to really 
take off into the world of programming.  Next lesson, we will learn more about working with variables and how to compare them 
to each other.

