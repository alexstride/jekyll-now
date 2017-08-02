---
layout: post
title: Genetic Algorithms 1 - Getting Stuck In
---

## Plan: 
1. Mission statement of this series of the blog (This is a series of articles to document my exploration of genetic algorithms, as I have some ideas for potential applications and want to see what they are capable of).

2. Documentation of resources followed so far + links. 

3. Links to the python library which I have written and brief gif of the genetic a basic phrase being evolved. 

Hello! This is the first post on my blog and I am starting with a series where I am getting stuck into genetic algorithms, from the point of view of somebody who has never really looked at them before. I will be documenting what I learn and the resources that I find useful, as well as linking to pieces of Python code which I write along the way.

The reason for wanting to look at genetic algorithms is partially because I want to know if they are suitable for a couple of practical applications which I have in mind (involving scheduling), but also because I have always been curious about how the process of natural selection could be mimicked by computers and, if so, whether it would be possible to create anything which behaves roughly like a life-form, as we might recognise the term. 

So the first place I went in my search was, of course, Youtube. And I watched the excellent [series of videos](https://www.youtube.com/watch?v=9zfeTw-uFCw&t=60s) by Daniel Schiffman on [The Coding Train](https://www.youtube.com/channel/UCvjgXvBlbQiydffZU7m1_aw) channel on Youtube, in which he talks about the basic ingredients of a genetic algorithm. Those videos definitely explain the basics much better and more thoroughly than I could here, so watch those if you are starting from scratch, but in general there are just a few things you need to create a working genetic algorithm: 

1. An initial population of 'individuals'*.
2. A method by which two (or any other number) of parents can reproduce to create a new individual. 
3. A method to judge the fitness of each individual.

**An 'individual' is the work used to describe just one evolvable thing, with one set of genetic material. In genetic algorithms we talk in terms of individuals and populations.*

