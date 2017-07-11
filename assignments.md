# Assignments

## Lab Tasks

_30% - Weekly_

Lab tasks are meant to exercise a particular practical skill from our lectures.

There are 9 lab exercises, evenly marked (each 3% of mark). Labs are marked on a scale of 0-10. Sometimes, just doing the task is a 10/10, other times it is divided by tasks.

**Due**: 1 hour before the following week's class.

## Small Assignments

- _20% - Two Assignments_
  - _10% - Twitter Bot Assignment_
  - _10% - Topic Modelling Assignment_

The small assignments are in lieu of lab tasks for their weeks. They differ in that you have more than 1 week to complete them, and their value is slightly higher.

### Twitter Bot Assignment

This project asks you to create a simple, rule-based Twitter Bot. There is no need to actually put it online: this is optional.

We'll use Cheap Bots Done Quick, powered by Tracery. To get started, follow along with [Your First Twitter Bot, in 20 minutes](https://sense.porganized.com/your-first-twitter-bot-in-20-minutes-35b2c610482d#.uz41sqy0k). Note that you can use any sources for data that you like, Corpora is merely one suggestion from the tutorial. 

Bot topic: Have fun with this. Your bot can be silly, avant garde, activitist. You may notice that there are limitations to Tracery: some things are really easy to do, but complex programming logic is not possible. How can you work within these restrictions?

One possibility to make a good bot is to apply what you've learned so far to prepare good source material. For example, can you use concordances or bigrams from a book to learn phrases that represent a writer that you want your bot to mimic? If you want to create realistic sounds but nonsensical sentences, look ahead to next week's Natural Language for Programmers reading by Liza Daly, which introduces Context Free Grammar, and the lab reading on identifying Parts of Speech with NLTK.

__Week 5: Post your idea for a Twitter bot on the Twitter Assignment forum.__

This can be brief: we want you thinking what can be done, and seeing what your colleagues are thinking about. 

__Week 6: Twitter bot due - describe it on the forum at least 1 hour before class.__

Post a short write-up (up to 600 words) about your bot and what motivated it. What issues did you run into? Include at least 10 randomly generated messages. If you put the bot up on Twitter (optional) share the handle*.

Finally, attach a text file with the full JSON for your bot.

The assignment will be marked out of 10, on the quality of the idea, the depth of the execution, and the clarity and quality of the written post. 1 point is automatically assigned for submitting the draft.

Engaging with colleagues in discussing their draft ideas will contribute to your participation mark. 

*Also, make sure to identify it as a bot in the bio, a convention that many botmakers follow for ethical reasons.

### Topic Modeling Assignment
For the topic modeling assignment, you'll use MALLET to perform text analysis on a collection of your choice.

MALLET is a Java-based toolkit for machine learning, including a module for Topic Modeling with Latent Dirichlet Allocation. To install and learn to use MALLET, follow along with [Getting Started with Topic Modeling and MALLET](http://programminghistorian.org/lessons/topic-modeling-and-mallet). As with the Twitter Bot Assignment, there is some self-directed learning with this assignment.

1. Find a good research question

Decide on an interesting set of texts to learn from. You can try something new, but you're also welcome to build on an idea from earlier in the course (e.g. from the Voyant lab) or do a preliminary version of something from your final lab.

What do you hope to explore? A better grade is rewarded for an idea that is appropriate for unsupervised learning, and for which learning topics can be insightful.

Are you stuck? Think about the genres of texts that we've seen in this class and in your colleagues' assignments: books, emails, tweets, lyrics, scripts, letters. Many of these can lead to an interesting idea. Think also about the examples we discussed in class.

Topic modeling is well suited for cases with many short texts. Since it learns from co-occurrence, you want your training texts to conceivably be about the same thing at the start as at the end. For example, modeling pages will give you better topics than modeling books.

Tip: When deciding on a research question, think ahead to the data collection step. Choose something that won't make this short assignment into a long one; remember that you'll have a final project to work on a more complex project if you want to return to topic modeling.

2. Find and prepare your source texts

Getting data is hard! You'll need to be resourceful.

MALLET needs input files that are structured either as a set of text files or one long text file, with each document on a different line. How do you collect your data? Can you find it already prepared? Do you have to do any cleaning?

Note that topic modeling is a bag-of-words approach, so if you want to use books from the HTRC Extracted Features dataset, you can write out tokens to files in a random order.

3. Build a topic model and write about it

Build a model and post about it on the Topic Modeling submission forum. Discuss both what you see in the output and what your process for building the models was.

Some possible questions to answer:

- What was your goal? Did topic modeling help?
- What is interesting about your topics? Do they match what you expect? If not, what looks peculiar?
- Which topics stand out? Which topics seem to be junk?
- How many topics did you choose? Why? Did you try alternate parameterizations?
- How did you collect your data? Were there headaches or necessary workarounds?
- What new research questions does this assignment inspire? If you had time for a bigger project, what would it be?

_Due: Week 12._

Grading - out of 10

- /2 - The Research question
- /2 - Data collection
- /6 - Forum post: quality of analysis and discussion of process

## Text Mining project

The final project is a culmination of your text mining expertise. You'll be putting your text mining skills to work. Up to now, the assignments have been method-based, where we tell you what to use and you find a problem for it. This time, you choose a problem to explore, formulate it as a research question, determine the methods to address it, and use it as part of a larger narrative.

The project has 3 components:

- 5% Problem statement: Due Week 12.
- 5% Literature review + 5% Data collection: Due Week 13.
- 20% Final report: Due one week after final class.

We'll still be learning methods that you may want to use throughout April, though the most prominent ones have already been covered: classification, clustering, topic modeling, stoplisting, concordances, part of speech tagging, document similarity etc.

A few more that we'll learn: feature selection - identifying the most discriminatory words in a collection; word embeddings - understanding the contexts of words and the relationships between them, removed from the document context; more document similarity methods; visualization, for better understanding what is going on in an analysis and for communicating it to others; sentiment analysis, for mining the opinions of texts.

Tell a compelling story. Remember that the complexity of the tool is not as important and the appropriateness. For example, something the top word frequencies make your point.

Here are some random research questions, alongside ways to ask them.

- RQ: Is there a specific language that belies conservative or liberal partisan media? Possible approaches: sentiment mining; term-weighted top frequencies.
- RQ: What characterizes my style in writing email? Possible approaches: topic modeling sent messages; building a classifier for time of day and seeing which words are notable for each class; visualizing sent email lengths.
- RQ: How do Alec Baldwin and Stephen Baldwin use Twitter different? Possible approaches: Term frequencies and concordances; classification (notable features via decision trees?); topic modeling; dimensionality reduction to 2 dimensions and observing outliers via scatter plot.
- RQ: Are there underlying trends motivating baby naming? Possible methods: classification or logistic regression using character patterns as features (e.g. last letter of the name, second letter, etc.).
- RQ: What do characters on Game of Thrones talk about? Possible methods: TF-IDF over scripts, compared to a [general language reference for IDF](https://www.ideals.illinois.edu/handle/2142/89691).
- RQ: How do people talk about food? Possible methods: identify types of food in a [dataset of food reviews](https://www.kaggle.com/snap/amazon-fine-food-reviews), and look at terms that coccur with them; topic model reviews and see which topics are most prominent for different words.
Good luck. We've been very impressed by the quality of your project ideas this term, and look forward to seeing what you come up with.

### Details

#### Problem Statement (Week 12):

Develop your idea and share a description of what you hope to do, what methods you hope to use, and early ideas for getting the data. Post it on the Problem Statement forum. Max 400 words.

#### Literature Review and Data Collection (Week 13):

Find examples of other people pursuing similar questions or using similar methods, and tell us about them. This will require some self-directed reading, searching. This isn't a lofty academic literature review, so you do not need to worry about how formal the literature is: it can include forum posts, blogs, new articles. (Tips: finding information online can be tricky - don't be afraid to share cool sources with your classmates or ask for advice on the forums).

For the data collection section, we want to see that you've started trying to compile your data. If it's been easy, them us more about the data. If it's been hard, tell us about the problems that you're running into, and whether you've had to adapt from your original problem.

Post these parts on the Final Project Lit + Data forum.

#### Final Report (One week after final class)

For the final report, write about your findings. Structure a narrative about what you hoped to do, how you pursued it, and what you found.

Think of the report as a piece for the portfolio: to show your text mining skills to future employers while demonstrating your ability to communicate the results. Tell us how about how you addressed your problem. You want to catch the reader by having the most intriguing points summarized at the start, then give us the details: what analyses you ran, what subquestions you asked, what was seen. When appropriate, use tables or visualizations.

Below is our suggested structure. This is not a research paper, so you do not need to use these headings or structure. Rather, it's just a set of guidelines. Foremost, structure your report so it is easy to read for a non-expert.

 

1. Introduction

Provide a high-level explanation of what you did and the main interesting points. This is the section that convinces us to read further.
 

For the next three parts, reuse your text from the Problem Statement, Literature Review, Data Collection, editing it as you might see fit.

  2. Problem

  3. Related Work

  4. Data

5. Findings

Tell your data's story!

6. Conclusions and Next Steps

What was most salient or intriguing? What interesting new questions came out of your project? What else can be done?

__How to submit Final Report__

Post the final report on the submission forums, in one of the following ways:

- Written directly in Moodle, as a post
- Linked to a blog post (e.g. on Medium)
- Linking to a Jupyter notebook (e.g. on Github)
- Attaching a Jupyter Notebook (make sure you check that any images are included)

__Inspiration for writing__

Share examples on the forums: Yun and I will post some too.

## Participation

- 15% of mark
 - 5% Attendance
 - 10% Forum posts, comments, class engagement

## Late Policy

- Lose 10% day, up to 50%. Late is better than never.
- 2 late 'freebies': We won't count late marks for two labs, because sometimes life gets in the way.

- Last day for late assignments:
  - Labs: Turn in by May 3rd
  - Anything else: May 8th
