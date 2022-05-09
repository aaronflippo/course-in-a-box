
# Knowledge Check!
TODO:

### Here’s what we learned in this lesson:
TODO:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
## Quiz
{% assign q1-text = "I'm a programmer now!" %}
{% assign q1-choices = "True, False" | split: ', ' %}
{% assign q1_feedbacks = "Correct! You've written your first code and that makes you a programmer! Now let's continue the journey!, Wrong - You are a programmer!" | split: ', ' %}
{% assign q1-correct = 0 %}
{% include mc-quiz.html text=q1-text choices=q1-choices answer=q1-correct feedback=q1_feedbacks %}

