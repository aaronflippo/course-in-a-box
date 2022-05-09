---
title: Our First Function
---

# Our First Function
Alright, this section might be a bit mind-blowing, because it will totally change how you think about code. It might seem a little confusing at once, but hang in there, you'll figure it out with practice!

### Why Repeat Yourself?
Take a look at the following program. It should look pretty familiar to you now - it's prompting the user for input, then reading the input back into variables.

{% highlight csharp %}
{% raw %}
using System;

//get the user's first name
Console.Write("What's your First Name?");
string firstName = Console.ReadLine();

//get the user's last name
Console.Write("What's your last name?");
string lastName = Console.ReadLine();

//get the user's pet name
Console.Write("What's your pet's name?");
string petName = Console.ReadLine();


{% endraw %}
{% endhighlight %}

But I'd like you to take a look at the overall pattern in this code.

There are 3 sections here, and they're all *very* similar.
The only thing that's different for each of these 3 sections is the text that's written to the console, and the variable that stores the user input.

### Declaring our function
So let's write a *function* that does all of the common stuff above, and then just _call_ it 3 times and let it do the 'dirty work' for us.

Go ahead and write this out, exactly as you see it below. Write it above all of the other code in your file (after the using System; line)

{% highlight csharp %}
{% raw %}
string GetUserInput(string prompt)
{

}
{% endraw %}
{% endhighlight %}

There is a lot of new stuff happening here, so lets break this down!

On the first line above, we have what's called a function *declaration*:

This is a bit like a variable declaration - first, we have a _type_ (in this case, *string*).
Next, we have the function _name_, (in this case GetUserInput).

Then, we have a set of parenthesis, with "string prompt" in between them.
The "string prompt" between the parenthesis looks a bit like a variable declaration, doesn't it?' That's a "parameter" - an input value that will be passed into this function.

Now on the line next to the function declaration, we have a curly brace facing to the right, and then another curly brace facing left.

Those curly braces tell the computer where the code for the function will start and end.
So we have delcared a function called GetUserInput. It takes a single string parameter called 'prompt', and it has a return type of 'string', which means that the function needs to return a string when it's done.

### Giving our function... Well, Functionality!
So now that we've declared our function, 'let's put some statements inside it, between the two curly braces:

{% highlight csharp %}
{% raw %}
string GetUserInput(string prompt)
{	
	Console.Write(prompt);	
	string userInput = Console.ReadLine();
	return userInput;
}
{% endraw %}
{% endhighlight %}

This code is doing exactly what each of the 3 sections above do. Except, instead of passing in a specific string to the Console.WriteLine() function, we are passing in the "prompt" parameter.

To say that another way:

Our function takes a string parameter called 'prompt', and we pass that parameter into Console.WriteLine() - which it will then write to the Console.

We also don't have a specific variable name here, like "UserName" - instead, when we call Console.ReadLine(), we store it in a generic sounding variable called UserInput.
Then we "return" that UserInput variable, which is another way of saying we're goint to pass it back to whatever code called this function.

### Calling our function

Ok, we have written our function - now let's modify the rest of our program to *call* this function, passing in our prompts, and storing the values the function returns.
Your program should look something like this:

{% highlight csharp %}
{% raw %}
using System;

string GetUserInput(string prompt)
{
	Console.Write(prompt);
	string userInput = Console.ReadLine();
	return userInput;
}


string name = GetUserInput("What's your first name?");
string lastName = GetUserInput("What's your last name?");
string petName = GetUserInput("What's your pet name?");
{% endraw %}
{% endhighlight %}

This is kind of cool, isn't it? We can now do in one line what used to take 2 lines. The more complex our code gets, the more useful it becomes to put code into functions.

### Expanding Our Function

Now that we have a single functiion whose purpose is to prompt the user for input, let's improve it a bit!


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

I've made this function change the foreground color to red, just before it prints the prompt to the console.
Then it beeps, and changes the color to green before reading the user input.
Finally, it changes the color back to white before returning.

It gives the program a little bit of personality! 

Here's what that looks like if you run the program:
![alt]({{site.baseurl}}/img/3/functions2.png "image_tooltip")

Neat, right?

