---
title: More About Functions
---

# More About Functions

So far, we've created our first function, and learned how to 'call' it to execute the code inside. 
Let's expand on that, and learn a bit more about what we can do with functions!

### Expanding Our Function
Now that we have a single functiion whose purpose is to prompt the user for input, let's improve it a bit!

{% highlight csharp %}
string GetUserInput(string prompt)
{
	Console.ForegroundColor = ConsoleColor.Red;
	Console.Write(prompt);
	Console.Beep();
	Console.ForegroundColor = ConsoleColor.Green;
	string userInput = Console.ReadLine();
	Console.ForegroundColor = ConsoleColor.White;
	return userInput;
}

{% endhighlight %}



I've made this function change the foreground color to red, just before it prints the prompt to the console.
Then it beeps, and changes the color to green before reading the user input.
Finally, it changes the color back to white before returning.

It gives the program a little bit of personality! 

Here's what that looks like if you run the program:
![alt]({{site.baseurl}}/img/3/functions2.png "image_tooltip")

Neat, right?

### Void Functions
Sometimes, you'll see a function declaration that looks like this:

{% highlight csharp %}
void DoSomething()
{
	...
}
{% endhighlight %}

What does that *void* mean?
Well, it just means that this function doesn't *return' anything. It may have input parameters, but it doesn't send anything back to the calling code.


