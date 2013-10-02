Lesson 1:5 - Lists
==================

Goal:  To learn a new set of tags allowing us to show different types of lists of information.

Introduction:  A very common type of information we need to present on the web is lists of data.  In this lesson we will explore how to make lists.

#### Step 1:  Create an unordered list

Lets go back to our sample application and add the following to the bottom of the program:

<br>
<ul>
	<li>Sally</li>
	<li>John</li>
	<li>Jessica</li>
</ul>

The <br> tag is just ensuring that we start on a new line with our lists.  The <ul> and </ul> are the "unordered list" tags.  Inside the unordered lists tags we provide the list item tags (<li> and </li>).  Each list item becomes a new entry in the list being created.

#### Step 2:  Lets have some order

Unordered lists are great, but sometimes you really want people to know that the items are in a particular order.  Change our example to the following:

<ol>
	<li>Sally</li>
	<li>John</li>
	<li>Jessica</li>
</ol>

Here we've gone from "unordered list" tags to "ordered list" tags.  When we run this program we see that the items in our list are not numbered (they have an order).


#### Step 3:  Building more complex lists

Lets say we have a list of children and we want to show which classes each of them go to each day.  There is no order to the children, but we want their classes to show up in the order each child has them each day.  We could program that like this:

<ul>
	<li>Sally</li>
		<ol>
			<li>Math</li>
			<li>English</li>
		</ol>
	<li>John</li>
		<ol>
			<li>English</li>
			<li>Math</li>
		</ol>
</ul>

If we view this example, we have a list with students without an order and a list of classes under each student this is in order.


Conclusion:  This lesson has again expanded the number of tags we know how to use to make HTML documents.  We learned how to keep track of lists of information.  We learned how to deal with either ordered lists of information or lists in which we didn't care about the order of values.  With every lesson that we complete, we're getting to be better web programmers.  
