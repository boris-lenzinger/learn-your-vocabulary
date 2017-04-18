Vocabulary tool
===============

The goal of this tool is to get a simple service that allows to check if
a vocabulary list is mastered.

This need has showed up when I was trying to learn Hungarian. It was quite
difficult to learn from my notebook and I was always tempted to check the
translation or could not get a good speed of questioning.

Moreover, I was not sure how good my knowledge was. I then understood that
repetition was, for me, the key. I then started to develop this tool with
a CSV file as basis and a given formalism in the comment to help parsing
the file.

Features
========
  The tool currently reads a CSV file. You can also use files from other
people if you share vocabulary files. My files are coming from my working
book Assimil. The format of the file is defined in a dedicated section below.

  Set a speed to be questionned : you can define a timer between each question.
So you can push your limits away until overflow !!

  Define the range of the lessons you want to study.

  The words are not in any order : this is a random questionning so you don't
have any pattern.

  When the words are displayed, the percentage for progression in the list is
displayed.

  You can interact with the tool using a set of command to increase/decrease
the speed of the questions. You can also stop the questions and change the
range of the lessons. The idea is to be able to reconfigure the questions
when in progress.

  When receiving a question, you should push right/up to say you know it.
Else the answer will be considered as unknown. If you don't know a word,
you use the left/down keys to tell it so.

  You can build a statistics database and then make some queries on it to
check where you fail to learn.

  You can ask to be questionned on the less known words/verbs to strengthen
you weak words.
  
The project
===========
This project is a personnal project to improve my skills in Go and try to use
different technologies.
I'm quite interested in Hashicorp products so I wanted to make a first implementation
with a CSV file and then use Consul to get an online API for a distributed and
scalable key/value table. That way, the service could serve multiple users
without bottleneck as it would with a single HTTP server.

Syntax/Options
==============

