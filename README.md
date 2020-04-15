# Pulling Signals Out of Speech with NLP in Python

The goal of this project is to find out if responses to questions asked to Siri are correct.  

We pull out different signals to see what we can use to understand which is correct in the context of customers asking to find a particular place(i.e. "close Starbucks", "Barry's Cafe") or kind of place("good restaurant").

I broke down the signals into different categories by "intent" as in the intention of the customer(e.g. "GetHoursIntent" = Customer wants to get the hours of a place or a kind of place).

Then with reGex I matched for the actual content, as in did we give hours.

There I go a percentage or rate of customers wanting some content and how often we were able to give that information.
-------
Then I wanted to see WHERE, as in which city these questions were being asked and succeeding or failing.

This is to identify data gaps, as in where Siri has better, or worse data associated to places asked about by customers.
-------
I did a dive deep into the questions to find if there were concentrations of words with certain intents, as in if the words "telephone number" have a very high occurrence when customers want to get hours, that likely means the wrong intent has been assigned and Siri thought the customer wanted hours when they really wanted the phone number.
------------
Finally I used a Naive Bayes ML model to try and judge that accuracy between intent and answer given using word frequency


