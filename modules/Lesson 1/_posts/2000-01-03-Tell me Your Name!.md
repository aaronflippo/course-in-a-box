# Tell Me Your Name!

So we've figured out how to make the computer write a line of text to the console. Great!
What else can we do?

Let's have the computer ask the user for their name:

{% highlight csharp linenos %}
{% raw %}
using System;

Console.WriteLine("Hello, what's your name?");
Console.ReadLine();
Console.WriteLine("That's a great name!");

{% endraw %}
{% endhighlight %}

Again, you'll need to pay careful attention to the capitalization of everything, and also remember to put a semicolon (;) at the end of each statement.

Here's what it should look like if you run the program now:
![alt]({{site.baseurl}}/img/1/tellmeyourname_console.png "image_tooltip")

Of course, the computer doesn't care what we type in - the only instruction we've actually given it is to read a line of text from the user in the console!
The thing to remember about programming is that the computer will always do *exactly what we tell it to* - nothing more, and nothing less.

## Dot Syntax and "Intellisense"
You may have noticed as you type out these lines of code that a little window pops up right when you hit the '.' key:

![alt]({{site.baseurl}}/img/1/dotsyntax.png "image_tooltip")

It turns out that "Console" refers to a whole set of different built-in functions, and we access those functions by typing Console. ("Console dot") and then the name of the thing we want to do.

But we don't have to memorize all of these different functions, because Visual Studio has a handy tool called Intellisense that will tell us all the options available to us.
Here's how it works:

Type Console. to bring up the intellisense window.
Now, as you type more letters, intellisense will search all the possibilities for you, narrowing it down according to the letters you type.
Here's what intellisense shows me if I write Console.wr:

![alt]({{site.baseurl}}/img/1/intellisense2.png "image_tooltip")

It highlights the option that's its best guess at what we want. If the option you want is highlighted, press the **enter** key or the **tab** key, and Intellisense will go ahead and write the rest of the line for you!
If you see an option in the list that's not highlighted, you can press the up and down arrows to scroll through them, and press the Enter or tab key to write that line.

![alt]({{site.baseurl}}/img/1/intellisense_anim.gif "image_tooltip")

Intellisense is great because it helps us explore the different options available to us, and also makes it faster to write out lines of code.
It's like we're *collaborating* with the computer to write code!





