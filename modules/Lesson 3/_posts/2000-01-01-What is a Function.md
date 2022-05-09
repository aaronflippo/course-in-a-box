---
title: What is a function?
---

# What Is A Function?

So far, we've been writing statements, which are single line instructions for the computer.

Sometimes though, we find that we want to do the same thing repeatedly in different parts of our code, and that's where functions can save us time.


### Using Functions
It turns out - we've already been using functions!

Remember this code?
{% highlight csharp %}
{% raw %}

Console.WriteLine("Hello, what's your name?");

{% endraw %}
{% endhighlight %}

Here we're *calling* a function called Console.WriteLine(), and we're passing in a string value ("hello, what's your name?'"), which the function then prints to the console.

You can think of a Function as a *command*. From the point of view of our code above, we are _calling_ the WriteLine function. It turns out that the function actually has statements of its own inside - we just can't see them.

The WriteLine() function takes a single string "parameter" - the value you want to print to the console.
In fact, if we use intellisense, we can see what the parameters of the function are:
![alt]({{site.baseurl}}/img/3/functions1.png "image_tooltip")

A function can have paramemters, which are _inputs_ to the function.
It can also have a "return value", which is an _output_ from the function.

In fact, we've already been working with a function that has a return values:

{% highlight csharp %}
{% raw %}

string name;
Console.WriteLine("Hello, what's your name?");
name = Console.ReadLine();

{% endraw %}
{% endhighlight %}

Do you see where we're using a return value?

The Console.ReadLine() _returns_ a string value that represents the user's input.

### Algebra, really?!
If you've taken an algebra class, you may recognize that what we're dealing with here looks a lot like a function in algebra. In algebra, functions take an input, do something with it, and then produce an output.
It's the same idea here - except in code, functions can have any number of inputs.

### More Functions

Here's another fun function to call:
{% highlight csharp %}
{% raw %}

Console.Beep();

{% endraw %}
{% endhighlight %}

Can you guess what this function does? Why don't you put it in your program and find out!
This beep function doesn't take any parameters - you can tell because we're not passing anything in between the parenthesis: ()

So to recap: 
1. Functions are like commands. 
2. Sometimes they take input, called parameters. 
3. Functions have code inside of them, which you can't see from the outside when you call them. This code is what gives the function its usefulness.
4. Sometimes, functions "return" values, which we can store in variables.
5. Sometimes, like with the beep function, the function just does some stuff, but doesn't take any input or output.

Got all that? Good, now let's write our own function!
