
To review, we have a namespace called MyFirstApp, and that namespace contains some additional code inside of it. Let’s take a look at what’s inside that namespace:


![alt]({{site.baseurl}}/img/1/classdeclaration.png "image_tooltip")


Here we have a line that says:

***class Program***


What do you see directly after that line?

That’s right, we’ve got a right-facing curly brace. If you follow those dashed lines down, you can see a matching left-facing curly brace a few lines below with some additional code “inside” those curly braces.

What this line means is “I’m declaring a new class called Program”.

We’ll get into “classes” a bit more later! For now, all you need to know is that a **class** represents an object, and it will have additional code inside of it.

Let’s zoom in a little further and see what’s “inside” this class:

{% highlight csharp linenos %}
{% raw %}
using System;
void main()
{

}
{% endraw %}
{% endhighlight %}


![alt]({{site.baseurl}}/img/1/inside_class.png "image_tooltip")


This is a pretty complicated line with a lot of new words that we don’t need to totally understand yet. 

For now, ignore everything except for a couple key parts of this line: The word “Main”, and then a right-parenthesis and a left-parenthesis (with some additional stuff in between the parenthesis)


![alt]({{site.baseurl}}/img/1/function_name.png "image_tooltip")


This is what’s called a “Function” You can always tell you’re dealing with a function when you see the parenthesis.

**Functions** are a way of grouping lines of code together that will run in sequence. When the computer “**calls**” a function, it runs all of the code inside of it.

_Note: You’ll also see functions like this referred to as “methods”. A “method” is just a name for a function that belongs to a class._

Currently, this function has nothing in between the curly braces - it’s “empty”: \

![alt]({{site.baseurl}}/img/1/function_inside.png "image_tooltip")


So, let’s add some code in here!

Add the following two lines of code in between the curly braces:


![alt]({{site.baseurl}}/img/1/statements.png "image_tooltip")


❗ You’ll need to write these _exactly_ as they’re shown, making sure to get the capitalization right, and putting the semicolon at the end of each line as shown.

These two lines of code are called “**statements**”, which means they contain some instructions for the computer to carry out directly. The computer will read them from the top downward, running one statement after another. Statements will _always _need to have a **semicolon** at the end. This tells the computer that it’s the end of the statement.

Now, save your file (Ctrl+S or Cmd+S on a Mac) and hit the Play button at the top of Visual Studio. It will take a minute for the computer to “**compile**” the program. If everything has been entered correctly, you should see the following:


![alt]({{site.baseurl}}/img/1/program_output.png "image_tooltip")


If the program doesn’t run, double check that you’ve entered everything exactly as shown above, and that you didn’t delete any of the curly braces or code that you started with.

This window that pops up is called the “**console**”. The console is a way for the program to communicate things to the program’s user and to gather user input.

Congrats! You've now written your first code, and started your journey as a programmer.




# C# File Structure

Now, we have  a project with a single file in it called Program.cs.

Visual studio has a panel called Solution Explorer, and you should be able to see Program.cs listed there.

(If you don’t see the Solution Explorer, use the View->Solution Explorer option to bring it up)


![alt]({{site.baseurl}}/img/1/5_solutionexplorer.png "image_tooltip")



### Structure of a C# File

Program.cs should look something like this:


![alt]({{site.baseurl}}/img/1/6_programoverview.png "image_tooltip")
(It might look a little different depending on which version of Visual Studio you're using, For instance, there might be more or less lines that say 'using' at the top of the file, or the names might look a little different.)


There’s a lot going on here! It’s not too important that you understand everything you see just yet, but we’re going to break this down a bit so you can understand the basic structure of a C# code file.

We’re going to break down everything you see here, which includes:



* “using” statements
* Namespaces
* Classes
* Functions
* Lots of curly braces

**Using statements**

First, we have a bunch of lines that start with the word “**using**”:

(It’s possible your program won’t have all of these lines, but you’ll probably see at least the first line where it says “using System;”


![alt]({{site.baseurl}}/img/1/7_usingstatements.png "image_tooltip")


For now, the way you can think about “using” statements is that they’re telling the computer that this file might want to make use of the code in the specified “namespaces”. For instance, at line 4, we have “using System.Text” - by adding this line, it will allow us to use code in the System.Text namespace, so we can do things with text. 

### Namespaces

Next, we have the following at line 7:


![alt]({{site.baseurl}}/img/1/8_namespace.png "image_tooltip")


What this line means is “I am creating a namespace called MyFirstApp”. A “**namespace**” is just a way to group related code together. 

### Curly Brace

You’ll notice that right after that line, there is a curly brace that opens to the right. And if you follow the dashed lines  down the screen, you’ll see a matching curly brace that opens up to the left:


![alt]({{site.baseurl}}/img/1/curlybraces_namespace.png "image_tooltip")


These **curly braces** are something you’ll see all over code, and they’re very important! In this case, everything in between the curly braces is part of that “MyFirstApp” namespace. The two curly braces “contain” everything in between them. You can think of them like two hands, holding everything in between:


![alt]({{site.baseurl}}/img/1/curlybracehug.png "image_tooltip")


If you ever have a curly brace that opens up to the right, you’ll always have to have a matching one that points to the left. If you don’t do this, your code won’t run!

