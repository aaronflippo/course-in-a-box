---
title: Our First Object
--- 
### Our First Object

Let's build a cat!

On the previous module, we talked about thinking in *objects*. In code, when we want to make an object, first we need to write a **class**.  
A class is like a "template" or a "blueprint" for an object. It describes to the computer what variables and methods this type of object should have - and then we can make one or more "Instances" of that class as objects.

Without further ado, let's go ahead and write a simple Cat class. 

First, make a new C# Console application called **Cat Adventure**
Then, clear out the contents of that first program file, and add the following to Program.cs:  


{% highlight csharp  %}
using System;
class Cat
{
    public string name;
    
    public void Meow()
    {
        Console.Write("Meow!");
    }
}
{% endhighlight %}

Let's break this down. First, we have a class delcaration, followed by open and close curly braces:

{% highlight csharp  %}
class Cat
{

}
{% endhighlight %}

This looks a bit like a function declaration - a class has a name, and then curly braces that hold all of its contents.
Then, inside the class (between the curly braces) we have a variable, and a function called Meow():  
{% highlight csharp  %}

    public string name;
    
    public void Meow()
    {
        Console.Write("Meow!");
    }

{% endhighlight %}

The only thing that's new here is that this variable and function both have the word "public" in front of them. For now just keep in mind that if you want to access those members from any code that's 'outside of the class itself, those members need to be "public".  
And that's it! Pretty simple, right?  

### Summon The Cat!
So far, we've written a Cat **class**. However, we're doing **object** oriented programming now, right? To actually make a cat **Object**, we need to make an **instance** of this class.  
Let's expand our program by adding the following **before** our Cat class in Program.cs:


{% highlight csharp  %}
using System;

//create a Cat object called aCat
Cat aCat = new Cat();

//call the Meow() method on it.
aCat.Meow();

class Cat
{
    public string name;
    
    public void Meow()
    {
        Console.Write("Meow!");
    }
}

{% endhighlight %}

Did you catch all that?
We declared a **variable** here called aCat. Instead of it being an int, a float, a string or a bool, instead it's type is **cat**.

Then we called the Meow() function on our Cat instance, usind "dot syntax", just like we've been doing with Console.Log()