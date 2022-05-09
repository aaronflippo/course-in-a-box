---
title: Numbers and Strings
---

# Numbers and Strings
In code when we say "Data", we're referring to the information the computer is working with. In code, data is stored in variables of different types.
Data types can be simple, or more complex. We'll get into the more complex ones later, but for now, here are the most important data types you'll want to know about.

### Numbers
There are two basic types of number variables in code: integers (whole numbers) and "floating point" numbers, (or decimals).

Here's are some examples of int and float variables:

{% highlight csharp  %}
{% raw %}
using System;

int AgeInYears = 15;
int NumStudentsInThisClass=19;
float DistanceInMiles = 5.2f;
float TempInDegrees = 92.6f;

{% endraw %}
{% endhighlight %}

*Note: In C#, when you declare a float variable, you need to put an 'f' at the end of the number, otherwise the computer will complain.*

There are also more data types for storing _large_ numbers: **long** and **double**, which are for larger integers and larger decimal numbers.
long and double use more computer memory, but can store bigger numbers. But for now, int and float should meet our needs.

**Try it now:**  Go ahead and declare a few of your own int and float variables in your Hello World code! Don't worry that they don't do anything yet, just get comfortable declaring variables and assigning values to them.

### Strings
We used a string in the previous module, so you already have a sense of what they do, but just to recap: A string holds text, or sequences of characters.
Any time you're reading text on a computer of any time, you're looking at something that's stored as a _string_ internally.

*Note: String values are always surrounded by a quotation mark on either side.*

Here are some examples of string variables.
{% highlight csharp  %}
{% raw %}
using System;

string UserName = "John Doe";
string Greeting = "Hello!";
string Greeting2 = "Well howdy!";
string ErrorMessage = "I'm sorry, something went wrong.";
string FirstName="John";
string LastName = "Doe";
string FullName = FirstName + LastName;

{% endraw %}
{% endhighlight %}

See that last example? I'm adding two strings together (FirstName and last name) and then assigning that value to another variable called FullName.

**Try it now:**  Go ahead and declare a few of your own string variables in your Hello World code. Output them using the Console.WriteLine() command.
