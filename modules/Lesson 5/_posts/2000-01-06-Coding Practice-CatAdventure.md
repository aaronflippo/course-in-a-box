---
title: "Practice: Cat Simulator"
---

We've covered a LOT in this lesson so far! You've learned about if/else statements for simple control flow, loops, boolean operators, and arrays.
Let's put together the knowledge from this lesson and the previous ones, and make a more sophisticated program.

# Cat Simulator
This program will simulate a cat. You'll be able to interact with the cat by typing simple commands, and see the status of your cat change.

1. Create a new Visual Studio project called CatSimulator.
2. For starters, lets use the Cat class from earlier, and put it into its own file called Cat.cs:
{% highlight csharp  %}

using System;
class Cat
{
	public string name = "unnamed Cat";
	public int age = 1;
	public bool isHungry;
	public bool isSleeping;

	public void Sleep()
	{
		isSleeping = true;
	}

	public void Wake()
	{
		isSleeping = false;
	}

	public void Feed()
	{
		isHungry = false;
	}

	public void Meow()
	{
		Console.WriteLine("Meow");
		Console.Beep();
	}
	public void AddYearsToLife(int howManyYears)
	{
		age = age + howManyYears;
	}

	public void PrintInfo()
	{
		Console.WriteLine("Cat info: ");
		Console.WriteLine("Name: " + name);
		Console.WriteLine("Age: " + age);
		Console.WriteLine("Hungry: " + isHungry);
		Console.WriteLine("Is Sleeping: " + isSleeping);

	}
}


{% endhighlight %}

Next, we'll write a simple program that instantiates a Cat, and then lets the user enter commands to interact with it:

{% highlight csharp  %}

//put this code in the main program.cs file
using System;

Cat myCat = new Cat();

while(true)
{
	Console.WriteLine("Cat status: "+myCat.PrintInfo);
	Console.WriteLine("What would you like to do next?: ");
	string command = console.ReadLine();
	if(command == "feed")
	{
		myCat.Feed();
	}
	else if (command == "sleep")
	{
		myCat.Sleep();
	}
	else if(command = "quit")
	{
		break;
	}

}

## Your Turn!
Use the code above as a startint point, and make sure you understand what the code is doing.

Then, try to extend it in the following ways:
1. Add a few additional commands for the cat. Example: Hiss, Grow, etc.
2. Add a command to let the user name the cat. This will require an additional prompt using Console.ReadLine(), and some code that sets the cat's name variable using dot syntax
3. Add some additional variables to the simulation to make it more interesting. For instance - you could give the cat an age, and add a command to grow the cat older. How would the cat's behavior change as it gets older?

{% endhighlight %}