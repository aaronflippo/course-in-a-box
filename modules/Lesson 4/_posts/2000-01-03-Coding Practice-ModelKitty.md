---
title: Building A Better Cat
---

# Building A Better Cat

Add the following to your Cat class:

Variables that represent:

1. Age in years
2. Is the cat hungry?
3. Is the cat sleeping?


And methods (member functions) that do the following:

Wake() - should set the appropriate variable from the list above  
Sleep() - should set the appropriate variable from the list above  
Feed() - should result in the cat not being hungry  
AddYearsToLife() - should take an int parameter.  
PrintStatus() - a function that prints out all of the cat's variables.



Here's what that class might look like, along with some code to instantiate a cat instance and test it out:

{% highlight csharp  %}

Cat cat = new Cat();
cat.name = "Fluffy";
cat.Sleep();
cat.Meow();
cat.PrintInfo();


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
