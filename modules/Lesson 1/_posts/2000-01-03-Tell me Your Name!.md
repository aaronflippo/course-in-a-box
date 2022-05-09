---
title: Tell Me Your Name!
---

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

One thing to remember about programming is that the computer will always do *exactly what we tell it to* - nothing more, and nothing less.

Later on, we'll learn about how to make the computer "remember" things like your name, using variables.



