---
title: "Control Flow: if not now, when?"
---

# Control Flow: If Not Now, When?

Sometimes, you only want parts of your code to run if a certain condition is met.
For instance - if you sign into an app but supply the wrong password, you're taken to a different screen than if you had provided the right one.

This area of programming is called *Control Flow*. 


### if() statements
The most common form of control flow you'll see in code is called an "if statement". Let's jump right in with an example to demonstrate how it works.

Imagine you're writing a game, and you've 're handling the logic for whether the player won the game or lost.

{% highlight csharp  %}

bool wonGame;

... //not shown: code that sets wonGame to true or false

if(wonGame)
{
	Console.PrintLine("Contrats, you won!");
}	


{% endhighlight %}

that *if* statement is an example of control flow. If the value between the parenthesis (in this case, the 'wonGame' bool variable) is true, then the code between the curly braces will execute.  
Otherwise, excecution will pass right over that whole section.


### if/else statements
We can expand on this concept, by adding an *else* statement. If the condition for the if statement evaluates to false, thent the code in the else block will run instead.


{% highlight csharp  %}

if(wonGame)
{
	Console.WriteLine("Contrats, you won!");
}	
else
{
	Console.WriteLine("Sorry, you lost!");
}


{% endhighlight %}

### More Examples
{% highlight csharp  %}

Console.WriteLine("Would you like to feed your cat?");
string input = Console.ReadLine();

//this makes use of the string function Contains(), which returns a bool value (true/false)
//instead of storing that value in a variable, we pass it directly into the if statement:
if(input.Contains("y"))
{
	Console.WriteLine("Your cat seems content");
}
else
{
	Console.WriteLine("Your cat looks at you hungrily");
}
{% endhighlight %}

when using if() statements, you can put *anything* in between the parenthesis, as long as it evaluates to a true/false value.

### Boolean Operators
Now that we're working with control flow, 'bool' values (true/false values) are going to become more important.
But what if we need to handle more sophisticated decisions about control flow?

As an example: Let's say you are writing code to let the user set a password for an account in an app. 

You might need to check the following to decide if the password is valid:

The password is at least 10 characters long.  
**AND**  
The password contains at least one letter.  
**AND**  
The password contains at least one number.  

if all three of these conditions are 'true', then the password is correct.


This is where **boolean operators** come in.

The three most common boolean operators are:  
AND (&&)  
OR (||)  
NOT (!)


It can be a little confusing to explain these, so here are some examples of these operators in action:

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


### Practice time!

Write if or if/else statements to handle the following:
1. Query the user for a string input, and then print something if the string contains "Y" OR if it contains "y" (handle both upper case and lower case)
2. Write a function that takes two numbers, and returns the larger of the two
3. Write a function that takes two numbers, and returns true if they're not equal (hint: You can write this with a single line inside the function, using the != operator)
4. Make an int variable, and then write an if() statement that executes if the number is between 10 and 50
5. Make an int variable, and then write an if() statement that executes if the number is less than 0 or more than 100


