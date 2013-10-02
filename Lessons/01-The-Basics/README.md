Lesson 1 - The Basics
=====================

Goal:  Just to get started programming in HTML. To learn a couple basic tags and understand the structure of HTML documents.


Step 1:  Getting a page created

Every html page is just a file with a name that ends with the extension html or htm.  For example, the is an html file named MyWebPage:

	MyProgram.html
	
So lets create our first page.  Open a new file in a text editor of your choice and save it as MyWebPage.html.  Save it in an easy to find place like your computers main root directory.  Your instructors can help you if needed.

In our newly created file, lets type a little message:


	This is my web page.
	
Save the file with the changes and open a web browser like internet explorer, firefox, chrome or safari.

For the url, type the location and name of the file.  On my computer, I type this into the browser:

	file:///Users/mrddqb/MyWebPage.html
	
The class instructors will help you get your browser displaying your file.

Once you are able to see the page in the browser, consider creating a bookmark so you can easily get back to the page.  

Step 2:  Adding Tags

Our web page, so far, is really boring.  It doesn't do anything but display a little message.  It doesn't even have any html in it yet.  HTML is all about tags.  Tags are special directions given to the computer to tell it to do something with your text.  For example, lets change our file to this:

	This is <u>my</u> web page.
	
Notice that we have something different going on around the word "my" here.  This is HTML tagging.  All tags are surrounded by angle brackets (less than and greater than characters).  There is a starting tag (<u>) and an ending tag (</u>).  The ending tag is always the same as the starting tag but with the extra forward slash character (/).

Try this change to the file out by updating your html file, saving it, and clicking to refresh the page in your browser.  You should now see the word my in the sentence with an underline under it.  This is because the <u> and </u> characters are the html tag for starting and stopping underlining.  Tags do not get displayed, instead they tell the web browser to start doing something special - in this case underlining the text.


Step 3:  A couple more useful tags

Lets update our example to this:

'''html
	<i>This</i> is <b><u>my</u> web page<b>.
'''

Try this out in your browser (don't forget to save it) and you'll see that our example is getting more interesting.  The <i></i> tags mean italics or "slanted text".  The first word now looks special.  Notice that "my web page" is now in bold text. That's what the <b></b> tags do.  Everything between them (all the text) will be in bold.  Notice that the word "my" is not both bold and underlined because it is inside both tags.


Step 4:  Official html structure

To this point, we have just made a small example html text document.  However, HTML file usually have more structure to them.  They have a tag that goes around the outside of the whole file (the <html> tag itself) and a section for a title and the body of the file.  Lets update our example program to look like this:

<html>
	<title>
		My Example
	</title>
	<body>
		<i>This</i> is <b><u>my</u> web page<b>.
	</body>
</html>

When you run this example, it should look just like the previous one because the body of your document (the mean part we see in the browser) is just the same.

The only difference is that now the title will be seen on the top of the browser window.


Congratulations!  You've done an amazing amount of learning in a very short time.  You are now able to create and save your own web pages.  You can view them in web browser, and you have learned how to use your first HTML tags to display pretty content.
