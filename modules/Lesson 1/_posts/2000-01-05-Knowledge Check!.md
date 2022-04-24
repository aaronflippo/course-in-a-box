
# Knowledge Check!


### Here’s what we learned in this lesson:

1. We made a program with a single file in it.
2. This file has a “namespace” called MyFirstApp, which was created automatically for us.
3. This “namespace” has a _class _inside of it called Program.
4. The Program class has a function inside of it called Main(). It just so happens that the computer knows to “call” the main function when you run the program, so this is like the “entry point” for the program.
5. We added two lines of code inside the main function.


<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
## Quiz
{% assign q1-text = "I'm a programmer now!" %}
{% assign q1-choices = "True, False" | split: ', ' %}
{% assign q1_feedbacks = "Correct! You've written your first code, and that makes you a programmer! Now let's continue the journey!, You are a programmer!" | split: ', ' %}
{% assign q1-correct = 0 %}
{% include mc-quiz.html text=q1-text choices=q1-choices answer=q1-correct feedback=q1_feedbacks %}


{% assign q1-text = "I'm a programmer now!" %}
{% assign q1-choices = "True, False" | split: ', ' %}
{% assign q1_feedbacks = "Correct! You've written your first code, and that makes you a programmer! Now let's continue the journey!, You are a programmer!" | split: ', ' %}
{% assign q1-correct = 0 %}
{% include mc-quiz.html text=q1-text choices=q1-choices answer=q1-correct feedback=q1_feedbacks %}

