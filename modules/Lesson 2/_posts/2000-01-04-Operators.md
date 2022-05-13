
---
title: Operators
---
# Operators

So far, we've looked at a few types of variables: **int, float, string,** and **bool**.

So, what are some things we might want to do with these types?
Well, for numbers, we might want to add, subtract, multiply, or divide them. 

After all, computers are great at math!


### Math Operators For Numbers (And Strings)
Math operators include:  
 Addition (+)  
 Subtraction (-)  
 Multiplication (*)  
 Division (/)  

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

### Boolean Operators

bool values have their own speical operators, which are used to combine bool values in logical ways.
The three most common boolean operators are:  
AND (&&)  
OR (||)  
NOT (!)

It can be a little confusing to explain these, so here are some examples of the && and || operators in action:

{% highlight csharp  %}
{% raw %}

//true if user is over 16 years of age
bool UserIsOver16;
//true if user has a driver's license
bool UserHasDriversLicense;

// a new bool value that's true only 
// if user is over 16 AND has a driver's license 
//(and false if either of these values is false)
bool UserCanDriveLegally = UserIsOver16 && UserHasDriversLicense;

// a bool value that's true if EITHER UserHasADog or UserHasACat is true:
bool UserHasAPet == UserHasADog || UserHasACat

//here's the "not" operator: It's true if the variable it's applied to is *not* true:
bool IsSleeping = !IsAwake;


{% endraw %}
{% endhighlight %}

### Relational Operators
Todo: Explain >, <, >=, <=, ==, and !=

### Operator Order:
Just like in math, operators are used in a particular order.
We won't go over all the details here, but one thing you should know is that youy can use parenthesis to control the order operators will be evaluated.

Examples:
{% highlight csharp  %}

//Add C+D first, then multiply by B:
float A = B*(C+D);

//Multiply B*C, then add D:
float A = (B*C)+D;

{% endhighlight %}


