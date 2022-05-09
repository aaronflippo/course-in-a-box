# Let's Say Hello

The first thing we're going to do, is to delete all of the text in Program.cs.
That's right! We are going to start from scratch to keep things simple.

Tip: You can select all the test in a file by pressing Ctrl+A (Or Cmd+A on a Mac).

After you've deleted everything in program.cs, add in the following line, exactly as it's written here:


{% highlight csharp linenos %}
{% raw %}
using System;
{% endraw %}
{% endhighlight %}

Pay attention to the capitalization of the word 'System', and also the semicolon at the end of the line.
We'll talk about what this line means in a bit.

Next, add the following line - again, be careful to write it out exactly as it is here:

{% highlight csharp linenos %}
{% raw %}
using System;

Console.WriteLine("Hello World!");

{% endraw %}
{% endhighlight %}

Now, hit the "Play" button at the top of Visual Studio: 
![alt]({{site.baseurl}}/img/1/playbutton.png "image_tooltip")


If everything is entered correctly, you should see a window pop up with some text in it - and the first line should be "Hello World"
![alt]({{site.baseurl}}/img/1/program_output.png "image_tooltip")

### Dealing With Errors
If there's an error, Visual Studio will tell you that it can't run the program.
Usually, you can look at your code and see little red "squiggly lines" telling you where the problem is.
For instance, here's what it looks like if I use a lower-case C in the "Console.WriteLine" statement:
![alt]({{site.baseurl}}/img/1/program_error.png "image_tooltip")

If you have an error, just refer back to the reference code above and fix it, then your program will run.

## Add some more!
Go ahead and extend your program with a few more lines that are just like the first.
Hint: Copy+paste the first line using Ctrl+C, then Control+V (Or Cmd+C/Cmd+V on Mac) and then modify the part between the quotes.

{% highlight csharp linenos %}
{% raw %}
using System;

Console.WriteLine("Hello World!");
Console.WriteLine("How are you today?");
Console.WriteLine("Is anyone there?");

{% endraw %}
{% endhighlight %}

### What did we just write?
One way to think about code is that it's like a **recipe** for a computer to follow.
Recipes always have two parts - the ingredients, and the directions.
![alt]({{site.baseurl}}/img/1/recipeanalogy.png "image_tooltip")
Usually, the ingredients are listed first, and then the directions are listed step-by-step.

With computer programs, the equivalent of the ingredients is what we call **data**. We'll get to data in the next lesson!
What we just wrote is an example of a **statement**, or an instruction that the computer will execute.
When the computer encounters statements, it executes them from the top to the bottom of the file, one after another.

This Statement we wrote is telling the computer that we want it to write a line to the "Console" (which is that window that pops up when we run the program), and the text between the quotes is the line of text we want it to write.

## Why "Hello World"?
If you have ever looked at coding tutorials like this, it seems that everyone uses 'hello world' in our first lesson. Why is that?
Well - nobody knows for sure! But here's an interesting article on the topic if you'd like to read it:

[History of Hello World](https://www.thesoftwareguild.com/blog/the-history-of-hello-world/#:~:text=Traditionally%2C%20Hello%20World%20programs%20are,World%20both%20easily%20and%20correctly)

When you're ready, let's move onto the next part of the lesson!
