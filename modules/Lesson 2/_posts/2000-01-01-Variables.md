---
title: What are variables?
---

# What Are Variables?

Remember our analogy from our first lesson about how code is a bit like a recipe? Recipes have a list of ingredients, each with a specific amount, and then a list of instructions for what to do with those ingredients.
So far we've worked with _statements_, which are instructions for the computer to execute.

In this lesson, we're going to dive into _variables_, which are a bit like the programming equivalent of ingredients for our code recipes. They give our program a working memory and let us do some really powerful things with code that we can't do with statements alone.

### Declaring Variables
Here's how it works:

First, we "declare" a variable in our program by giving it a _type_, and a _name_. Here's an example of a variable declaration, where the _type_ is string, and the name is UserFirstName:

{% highlight csharp %}
{% raw %}
string UserFirstName;
{% endraw %}
{% endhighlight %}

The **type** comes first, then the **variable name**, then a semicolon

**IMPORTANT NOTE**
The variable name can **not** have any spaces in it! It also can't start with a number.

Next, we _assign_ some value to each variable, by using the equals (=) symbol:

{% highlight csharp  %}
{% raw %}
string UserFirstName;
UserFirstName = "Unknown Name";
{% endraw %}
{% endhighlight %}

We can also declare a variable and assign it a value, all in the same line:
{% highlight csharp  %}
{% raw %}
string UserFirstName = "Unknown Name";
{% endraw %}
{% endhighlight %}

### Another Analogy
Another way of thinking about variables, is that they're like a box with a label on it. The label on the box is the variable name, what's inside the box is the variable's value, and the shape of the box is the variable's '_type_.
(Todo: Add visual aid image)

### What Can I Do With Variables?

Remember our first program, where the computer asked for the user's name, and then said "That's a great name?"
{% highlight csharp  %}
{% raw %}
using System;

Console.WriteLine("Hello, what's your name?");
Console.ReadLine();
Console.WriteLine("That's a great name!");

{% endraw %}
{% endhighlight %}

Well, we can use a string variable to actually hold the user's name, and then use it later on in the program, like this:

{% highlight csharp  %}
{% raw %}
using System;

Console.WriteLine("Hello, what's your name?");
string UserName = Console.ReadLine();
Console.WriteLine("Nice to meet you, " + UserName);

{% endraw %}
{% endhighlight %}

That seems more useful, doesn't it?

One thing you'll notice we did on that last line there, is we _added_ to strings together:
{% highlight csharp  %}
{% raw %}

"Nice to meet you, " + UserName

{% endraw %}
{% endhighlight %}

You can use _operators_ like + to combine various types of data. In this case, we're adding together the string literal "Nice to meet you, ", and the variable Username.
The computer "evaluates" the value of Username, adds it together with the "Nice to meet you, " string, and then passes the combined value to the Console.WriteLine command.


Variables might seem complex at first, but you'll get used to them quickly! 

In the next section, we'll talk about the different types of variables and how to use them.

