# Assignment 05

**DUE: Monday, December 10, 2018 @ 5:00PM**

**WHERE TO GET IT**: `/users/library/csis/comp1501/assignments/5.asg`

**SUBMISSION PROCEDURE**:

To submit your assignment, just use the usual **submit1501** on INS.
When asked for the task identifier, please use **asg05**.

**WEIGHT: 6%**

**ANY QUESTIONS?** You know the drill!

## Overview

This assignment has 1 challenge - you are being asked to create a single application of non-trivial size using object-oriented programming.

## !!! WARNING !!!!

Although you have nearly 3 weeks to complete this assignment, you will want to get started right away.

You know by now from your experiences in this course that programming takes time - lots of time - especially considering you are dealing with a new thing like object-oriented programming.

In addition, you will likely have other assignments and projects due around the same time as this one.

And you're probably pretty weary by the end of the semester.

So it's a perfect storm of craptacular awesomeness.

## A suggested plan of attack

Starting a major assignment can feel overwhelming...where do you start?!?

Here are my suggestions.

1. make sure you look through the samples [here](201804.asg05.ascii.art.docs.md) in the docs so that you have a good idea as to how a functioning program works - you can't build something unless you know what it's supposed to do!
1. skim through the documentation blocks and look at everything marked with a TODO; you want to familiarize yourself with what's in the source code and get a general feel for what needs to be done
1. build the solution class by class - starting with the easier ones - and make sure you pass all the tests for that class before moving on to the next class. By doing this, you'll be fairly confident that when you start working on the `ArtiiApp.java` code, all the objects involved will work properly so any bugs that appear should be confined to dealing with user input. A suggested progression would be:
   1. `FileHelper`: this class is very small with short easy-to-code methods that _mostly_ deal with String concatenation. And you don't have to deal with files and exceptions here.
   1. `AsciiArt`: this class has only a few methods as well and you don't need to worry about files and such until the very end (when you need to deal with them in the second constructor). Once you have this working - even without the file-related constructor complete - you could safely move on to the next class and come back and finish the other constructor....
   1. `CharToColorMap`: this is a tiny class - we probably would have started here first, but it does require us to deal with files and exceptions.
   1. `AsciiToPngConverter`: hard to believe, but this is also a tiny class!  
   1. `ArtiiApp` can be left for last - it's easily the longest class...but if you've completed the previous 4 classes and have them passing the tests, you'll be surprised at how nicely everything comes together.

By working in this fashion, coding a bit and testing as you go, you feel like you're accomplishing something and moving forward - THIS IS SUPER IMPORTANT! A huge part of being successful in any programming task is about confidence (both in yourself and your code).

Another benefit of working this way is that it is harder for bugs to creep in, because you are working in small steps and testing as you go.

## Running tests

Because you're (hopefully!) testing your classes one at a time, I've added a few new `make` commands to make your testing life easier:
- `make fht`: run just the tests for `FileHelper.java`
- `make aat`: run just the tests for `AsciiArt.java`
- `make cmt`: run just the tests for `CharacterToColorMap.java`
- `make apt`: run just the tests for `AsciiToPngConverter.java`
- `make app`: run just the tests for `ArtiiApp.java`

`make tests` runs everything, just like always.
