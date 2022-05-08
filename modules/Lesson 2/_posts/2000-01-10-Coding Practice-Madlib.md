---
title: Let's Make a Madlib!
---

# Let's Make A Madlib!

Have you heard of a Madlib? It's a sort of game that was invented in 1953 by Leonard Sterrn and Roger Price. 
The basic idea is that the player is prompted for a series of words and phrases, without knowing how those will fit into a story. Then the player reads back the story, inserting their chosen words and phrases at key points, to hilarious results.

The original madlibs were presented in book form - we're going to write a computer program madlib!

This program will be a little longer, and you're going to have to design the story structure, so get ready to get creative!

Here's the basic structure of our program: 
1. We'll ask the user for a word or phrase one at a time, and store their answer in a series of variables, each with its own unique name.
2. Then we'll print out the story at the end, using all of those stored variables to generate a story.

{% highlight csharp  %}
{% raw %}
using System;

Console.WriteLine("Location (noun)");
string Location1 = Console.ReadLine();

Console.WriteLine("Object (noun)");
string Object1 = Console.ReadLine();

Console.WriteLine("Number");

//note: We could have used an int here, but it doesn't actually matter if it's a string.
string number = Console.ReadLine();

Console.WriteLine("Verb, past tense");
string verb1 = Console.ReadLine();

//Now output our story.

Console.WriteLine("Today, I went to " +Location1);
Console.WriteLine("While I was there, I bought a " + Object1);
Console.WriteLine("It cost me " + number+" dollars!");
Console.WriteLine("After that, I went back home and " + verb1);
Console.WriteLine("The end");


{% endraw %}
{% endhighlight %}

If you run the program, it will look something like this:

![alt]({{site.baseurl}}/img/2/madliboutput.png "image_tooltip")

### Coding Time!
Alright - up until now, we've walked you through every step with these lessons.
Now, it's time for you to get creative and expand this 'madlib' program to make it your own.
1. Replace the example story structure with your own.
2. Add 10-15 more words and phrases

You may want to test run your program frequently, in case you accidentally add any errors.


