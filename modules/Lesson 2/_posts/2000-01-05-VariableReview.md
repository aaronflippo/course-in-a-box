---
title: Variable Review
---

# Variable Types Review

Let’s think a little bit about what type would be most appropriate for the following variables:

Name

Height

IsSleeping

HoursSinceAte

IsHappy

HappinessAmount

AngryAmount

MyCat

That last one is a little tricky isn't it? After all, a cat is not a number, a string, or a bool. It's something more complex.
Later on in this course, we'll introduce you to 'classes', which are used for more complex 'object' data types, like cats, cars, people, and other types of objects.

### Declaring Variables review:
Remember, when you declare a variable, it always comes in this form:

type name = initialValue;

example:

int age = 10;

### Expanding our Hello World Program
Let's get a little more practice with using variables in a real application.

This program is a little longer! But if you read it carefully, you should be able to understand it.
Pay attention to the comments for details!

{% highlight csharp  %}
{% raw %}
using System;

//get the user's first name
Console.WriteLine("What's your first name?");
string UserFirstName = Console.ReadLine();

//get the user's last name
Console.WriteLine("What's your last name?");
string UserLastName = Console.ReadLine();

//get the user's age
//NOTE: Console.ReadLine always gives us a string, so we need to store that input in a string, and then "convert" it to an int, using the int.Parse() commmand.
Console.WriteLine("How old are you?");
string ageString = Console.ReadLine();
int UserAge = int.Parse(ageString);

//get the user's pet name
Console.WriteLine("What's your pet's name?");
string UserPetName = Console.ReadLine();

//Now repeat it all back to them
//NOTE: We add an extra space (" ") in between the first and last name, otherwise it wouldn't look right when printed.
Console.WriteLine("Nice to meet you, " + UserFirstName + " " + UserLastName);
Console.WriteLine("You are " + UserAge);
Console.WriteLine("And your pet name is " + UserPetName);

{% endraw %}
{% endhighlight %}




