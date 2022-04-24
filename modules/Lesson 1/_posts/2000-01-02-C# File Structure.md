

#C# File Structure

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

**Namespaces**

Next, we have the following at line 7:


![alt]({{site.baseurl}}/img/1/8_namespace.png "image_tooltip")


What this line means is “I am creating a namespace called MyFirstApp”. A “**namespace**” is just a way to group related code together. 

**Curly Braces**

You’ll notice that right after that line, there is a curly brace that opens to the right. And if you follow the dashed lines  down the screen, you’ll see a matching curly brace that opens up to the left:


![alt]({{site.baseurl}}/img/1/curlybraces_namespace.png "image_tooltip")


These **curly braces** are something you’ll see all over code, and they’re very important! In this case, everything in between the curly braces is part of that “MyFirstApp” namespace. The two curly braces “contain” everything in between them. You can think of them like two hands, holding everything in between:


![alt]({{site.baseurl}}/img/1/curlybracehug.png "image_tooltip")


If you ever have a curly brace that opens up to the right, you’ll always have to have a matching one that points to the left. If you don’t do this, your code won’t run!

