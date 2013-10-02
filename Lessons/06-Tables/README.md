Lesson 6 - Tables
===================

*Goal*:  To learn how to use HTML's table tags to display charts of information in our web pages.

*Introduction*:  Tables are one of the most popular topics in HTML programming.  Nearly any page created will have at least one table in it.  Here we will build up a table of data that is similar to our list examples from the last lesson. 

#### Step 1:  Create a basic table

Type the following into the bottom of our web application:

	<br>
	<table>
		<tr>
			<td>
				Sally
			</td>
			<td>
				Math
			</td>
		</tr>
		<tr>
			<td>
				John
			</td>
			<td>
				English
			</td>
		</tr>
	</table>

There's a lot going on there, so lets take it one step at a time:
	- the &lt;br&bt; tag is only used to start on a new line for our table.
	- The table tags (&lt;table&gt; and &lt;/table&gt;) tell our program "we are building a table now".
	- Inside a table are table row tags (&lt;tr&gt; and &lt;/tr&gt;).  A table is made up of one or more rows of information to be displayed.
	- Inside each table row are table definition tags (&lt;td&gt; and &lt;/td&gt;).  These make up all the columns in the table.
	

#### Step 2:  Make it easier to see the table

Change the table definition tag to this:

	<table border="1">

By adding the border attribute to the table, our program draws lines for all the cells in the table, making our table's structure much easier to see.


#### Step 3:  Make our table colorful

Update the line for sally like so:

	<td bgcolor="red">
	
The bgcolor attribute stands for "background color" and can be used to spice up the presentation if information.


#### Step 4:  Put HTML into our table

Replace the line with the word math in our example with the following several lines:

	<ol>
		<li>Math</li>
		<li>English</li>
	</ol>
	
This places an ordered list inside the table cell.  You can put pretty much any HTML you want to inside a table cell - even another table!

Try putting an image tag like the one from lesson 4 in one of our table definition cells. 


#### Step 5:  Adding a header to our table

Right after the &lt;table&gt; tag but before the first <tr> tag, add the following HTML:

	<tr>
		<th>
			Student
		</th>
		<th>
			Favorite Class
		</th>
	<tr>

At first this looks just like another table row (&lt;tr&gt;), but instead of using table definition tags, it used table header tags (&lt;th&gt;).  These tags create titles for the columns in our table.  


Conclusion:  In this section we learned all about tables in our html pages.  We learned not only about the html tags we use to create tables, but also that we can build up tables with other HTML content inside them.  At this point, our familiarity with HTML's tags and how to build web pages is really growing fast.
