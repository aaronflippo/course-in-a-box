

#Writing Some Code

To review, we have a namespace called MyFirstApp, and that namespace contains some additional code inside of it. Let’s take a look at what’s inside that namespace:


![alt]({{site.baseurl}}/img/img/1/classdeclaration.png "image_tooltip")


Here we have a line that says:

class Program

 \
What do you see directly after that line?

That’s right, we’ve got a right-facing curly brace. If you follow those dashed lines down, you can see a matching left-facing curly brace a few lines below with some additional code “inside” those curly braces.

What this line means is “I’m declaring a new class called Program”.

We’ll get into “classes” a bit more later! For now, all you need to know is that a **class** represents an object, and it will have additional code inside of it.

Let’s zoom in a little further and see what’s “inside” this class:


![alt]({{site.baseurl}}/img/image12.png "image_tooltip")


This is a pretty complicated line with a lot of new words that we don’t need to totally understand yet. 

For now, ignore everything except for a couple key parts of this line: The word “Main”, and then a right-parenthesis and a left-parenthesis (with some additional stuff in between the parenthesis)


![alt]({{site.baseurl}}/img/image13.png "image_tooltip")


This is what’s called a “Function” You can always tell you’re dealing with a function when you see the parenthesis.

**Functions** are a way of grouping lines of code together that will run in sequence. When the computer “**calls**” a function, it runs all of the code inside of it.

_Note: You’ll also see functions like this referred to as “methods”. A “method” is just a name for a function that belongs to a class._

Currently, this function has nothing in between the curly braces - it’s “empty”: \

![alt]({{site.baseurl}}/img/image14.png "image_tooltip")


So, let’s add some code in here!

Add the following two lines of code in between the curly braces:


![alt]({{site.baseurl}}/img/image15.png "image_tooltip")


❗ You’ll need to write these _exactly_ as they’re shown, making sure to get the capitalization right, and putting the semicolon at the end of each line as shown.

These two lines of code are called “**statements**”, which means they contain some instructions for the computer to carry out directly. The computer will read them from the top downward, running one statement after another. Statements will _always _need to have a **semicolon** at the end. This tells the computer that it’s the end of the statement.

Now, save your file (Ctrl+S or Cmd+S on a Mac) and hit the Play button at the top of Visual Studio. It will take a minute for the computer to “**compile**” the program. If everything has been entered correctly, you should see the following:


![alt]({{site.baseurl}}/img/image16.png "image_tooltip")


If the program doesn’t run, double check that you’ve entered everything exactly as shown above, and that you didn’t delete any of the curly braces or code that you started with.

This window that pops up is called the “**console**”. The console is a way for the program to communicate things to the program’s user and to gather user input.
