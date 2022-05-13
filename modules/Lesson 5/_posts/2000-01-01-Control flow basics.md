---
title: "Control Flow: if not now, when?"
---

# Control Flow: If Not Now, When?

Sometimes, you only want parts of your code to run if a certain condition is met.
For instance - if you sign into an app but supply the wrong password, you're taken to a different screen than if you had provided the right one.

This area of programming is called *Control Flow*. 


### if() statements
Let's jump right in with a code example to demonstrate how it works.
Imagine you're writing a game, and you've created a function that's called when the game is finished.

This function takes a single bool parameter that's true if the player won the game:

{% highlight csharp  %}

void GameOver(bool wonGame)
{
	if(wonGame)
	{
		Console.PrintLine("Contrats, you won!");
	}	
}

{% endhighlight %}

that *if* statement is an example of control flow. If the value between the parenthesis is true, then the code between the curly braces will execute.  
Otherwise, excecution will pass right over that whole section.


### if/else statements
We can expand on this concept, by adding an *else* statement. If the condition for the if statement evaluates to false, thent the code in the else block will run instead.


{% highlight csharp  %}
void GameOver(bool wonGame)
{
	if(wonGame)
	{
		Console.WriteLine("Contrats, you won!");
	}	
	else
	{
		Console.WriteLine("Sorry, you lost!");
	}
}

{% endhighlight %}

### More Examples
{% highlight csharp  %}

Console.WriteLine("Would you like to feed your cat?");
string input = Console.ReadLine();

//this makes use of the string function Contains(), which returns a bool.
//instead of storing that value, we pass it directly into the if statement:
if(input.Contains("y"))
{
	Console.WriteLine("Your cat seems content");
}
else
{
	Console.WriteLine("Your cat looks at you anxiously");
}

//how to read this:
// "if cat isHungry and also cat is NOT sleeping, then run the code..."
if(cat.isHungry && !cat.isSleeping)
{
	Console.WriteLine("Maybe you should feed your cat?");
}

{% endhighlight %}

### Practice time!

Write if or if/else statements to handle the following:
1. Query the user for a string input, and then print something if the string contains "Y" or if it contains "y"
2. Write a function that takes two numbers, and returns the larger of the two
3. Write a function that takes two numbers, and returns true if they're not equal (hint: You can write this with a single line inside the function)
4. Make an int variable, and then write an if() statement that executes if the number is between 10 and 50
5. Make an int variable, and then write an if() statement that executes if the number is less than 0 or more than 100


