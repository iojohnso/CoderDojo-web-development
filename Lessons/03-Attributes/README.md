Lesson 3 - Attributes
=======================

Goal:  To expand our knowledge of HTML tags and how they can be customized with attributes.

Introduction:  We've already learned several useful HTML tags and build some pages.  Everything in HTML programming is made up of using these mark-up tags.  HTML tags can be further customized by attributes which are ways to make the tags behave in special ways.

#### Step 1:  Open or recreate our simple HTML file that looked like this:

    <h1>Listen up!</h1>
    <p>I have something important to say.  Soon I will tell you what it is.</p>
    <hr>
    <p>Actually, I think I forgot what I was going to say.</p>


#### Step 2:  Apply some attributes to a tag

Change the &lt;hr&gt; tag to look like this:

    <hr color="red" size="10" width="50%">

After that change, run the program again and see how it has changed.

You will notice that the horizontal bar is now much thicker, it is red and it doesn't go all the way across the screen anymore.

Color, size and width are examples of attributes.  And attributes serve to modify a tag's behavior.  


#### Step 3:  Change the units of an attribute

Change the &lt;hr&gt; line in your program to the following (remove the percent sign):

    <hr color="red" size="10" width="50">

Run the program again and you will notice that the horizontal rule got shorter.  This is because width is being measured in pixels now, not percentage of the screen.  While 50% is one half of the window, 50 pixels is just a count of little dots that make up the screen picture.


#### Step 4:  Apply a couple more attributes.  

Add the align attribute to both the header and the horizontal bar like so:

    <h1 align="center">Listen up!</h1>
    <p>I have something important to say.  Soon I will tell you what it is.</p>
    <hr color="red" size="10" width="50%" align="left">
    <p>Actually, I think I forgot what I was going to say.</p>

You should now see the title centered on the page and the horizontal bar all the way over to the right.  Notice that these two HTML tags had different default ways to display on the screen but both could be changed with our code to different ways of presenting.

Congratulations!  You now know every concept of HTML.  That's all there is to it - tags and attributes.  Over the next several lessons we will learn tags and attributes which will allow us to make more exciting programs, but we now have all the concepts we need to be HTML programmers!
