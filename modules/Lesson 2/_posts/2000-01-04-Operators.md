
---
title: Operators
---
# Operators

So far, we've looked at a few types of variables: **int, float, string,** and **bool**.

So, what are some things we might want to do with these types?
Well, for numbers, we might want to add, subtract, multiply, or divide them. 

After all, computers are great at math!


Here's a C# program that adds several int variables together representing the number of animals of various types, and stores them in a new int called NumAnimalsTotal
{% highlight csharp  %}
{% raw %}
using System;

int NumCats = 5;
int NumDogs = 10;
int NumFerrets = 2;
int NumAnimalsTotal = NumCats + NumDogs + NumFerrets;

{% endraw %}
{% endhighlight %}



Here's another C# program that calculates how much you might spend on coffee in a year.
This one is a little more sophisticated, because it's working with both int and float values, and multiplying them together:

{% highlight csharp  %}
{% raw %}
using System;

int NumCoffeesPerMonth = 10;
float CostPerCoffee = 3.61f;
float Total = NumCoffeesPerMonth * CostPerCoffee * 12;
Console.WriteLine("You'll spend" + Total + " on coffee every year");

{% endraw %}
{% endhighlight %}

Also, take a look at that last line: We are adding a string value to an int value, to another string value. The computer knows how to convert number values into strings, so the result is just one longer string.

This


