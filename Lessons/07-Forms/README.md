Lesson 1:7 - Forms
==================

Goal:  So far everything we have built is about show information to users of our web pages.  Our goal now is to learn how to take some information in from our users.

Introduction:  In order for the world wide web to not be just like one big book for reading, we have to create pages that actually can ask the user for some information.  We do that with the HTML form tags.  That's what we're going to focus on now.

#### Step 1: Allow some user input

User input is collected via form tags (&lt;form&gt; and &lt;/form&gt;).  There are several different types of input that can be collected, but the most common is simple a text input field.  Create the following in your sample program:

	<br>
	<form >
	   <p>
	   Name: <input type="text" name="FirstName" />
	   </p>
	   <p>
	   Email: <input type="text" name="Email" />
	   </p>
	</form>

When we run this, we end up with two fields on the screen that we can enter data into.  One is called name and one is called email.  But this is pretty useless if we can't "give" this information back to the computer.  We'll do that next.


#### Step 2:  Add a submit button

When data is collected from a user in a form, that data has to then be sent (submitted) to the computer.  Add the following line to your form entry just above the ending &lt;/form&gt; tag:

	<input type="submit" value="Submit My Info" />

When we run this, our form now has a button we can click to submit the data.  But when we click this button, we see nothing but our data disappear.  What's going on?

All of our data is being gathered and submitted, but we have not told our form where to submit the data to.  When it doesn't know where to submit data to, the browser simply submits it to the page its currently on.  If you look at the browser URL, it changed when you submitted your data. It should now look something like this:

	file:///...path to file...MyHtmlTest.html?FirstName=John&Email=john%40gmail.com

Notice that the end of the URL now has a question mark followed by the names you gave your input fields, an equal sign, and the values.  There is also perhaps some strange characters added.  For example, if you typed an "@" character into your email address, it has been replaced by the value "%40".  This is how a computer encodes your data for transferring it wherever the form tells it to go.

Congratulations!  You have done an amazing amount of learning about HTML at this point.  You have used nearly all of the common HTML tags and learned a great deal about how to use them to create web pages.  You are ready to build great things - explore and see what you can come up with.

If you want to take the example with the form data one step further, follow the bonus step here:


#### Bonus step:  Getting your data to another page.

If we want to get our form data to show up in another page, there are a lot of ways to do it.  The following is one of the more basic ways we can make it happen.  Often we will create "server" applications that work with our HTML programs to do lots of interesting things with the provided data.  Here we will simply process our parameters in another HTML page.

Before we can do anything, we have to tell the form to send the data to another page when the user submits it.  Find the <form> tag entry and change it to look like this:

	<form action="AnotherHtmlPage.html">

Now we want to create a new file in the same place that has this name (AnotherHtmlPage.html). 

When you are done with this, your whole form should look like the following:

In this new file, we're going to put a little code in another langauge called Javascript that can take the URL syntax we talked about in Step 2 and get back our parameters from it.  Copy the following code into your new html file:

	<script>
	// This is a pretty advanced function designed to take the URL
	// string (see the header line of your browser) and pull out the 
	// parameters that were submitted from the form.  Each can be 
	// retrieved with the following syntax:
	//   <script>document.write(getParameter('parameter_name')); < /script>
	function getParameter( name ){
		name = name.replace(/[\[]/,"\\\[").replace(/[\]]/,"\\\]");  
		var regexS = "[\\?&]"+name+"=([^&#]*)";  
		var regex = new RegExp( regexS );  
		var results = regex.exec( window.location.href ); 
	 	if( results == null )    
			return "";  
		else    
			return unescape(results[1]);
	}
	</script>

The script tags (&lt;script&gt; and &lt;/script&gt;) allow us to put code in another language directly into our html page.  That's about all the further we will go in learning about this for right now.  This code knows how to get our input names from our other page when the submit button is clicked.

Now, after the script, write the following code:

	<h1>Hi <script>document.write(getParameter( 'FirstName' ));</script></h1>

	I see that your e-mail address is <script>document.write(getParameter( 'Email' ));</script>.


This HTML code will get the two parameters from our form and show them in this page when the submit button is clicked.  Lets look at one of those programming statements:

	<h1>Hi <script>document.write(getParameter( 'FirstName' ));</script></h1>

By simply changing what we have in single quotes (FirstName here), we could get any parameter we wanted to from the form.  Go ahead and experiment with adding more text fields to your form and displaying them in this page when the submit button is clicked.
