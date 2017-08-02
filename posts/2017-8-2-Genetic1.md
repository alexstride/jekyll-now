---
layout: post
title: Genetic Algorithms 1 - Getting Stuck In
---
Hello! This is the first post on my blog and I am starting with a series where I am getting stuck into genetic algorithms from the point of view of somebody who has never really looked at them before. I will be documenting what I learn and the resources that I find useful, as well as linking to pieces of Python code which I write along the way.

The reason for wanting to look at genetic algorithms is partially because I want to know if they are suitable for a couple of practical applications which I have in mind (involving scheduling), but also because I have always been curious about how the process of natural selection could be mimicked by computers and, if so, whether it would be possible to create anything which behaves roughly like a life-form, as we might recognise the term. 

So the first place I went in my search was, of course, Youtube. And I watched the excellent [series of videos](https://www.youtube.com/watch?v=9zfeTw-uFCw&t=60s) by Daniel Schiffman on [The Coding Train](https://www.youtube.com/channel/UCvjgXvBlbQiydffZU7m1_aw) channel on Youtube, in which he talks about the basic ingredients of a genetic algorithm. Those videos definitely explain the basics much better and more thoroughly than I could here, so watch those if you are starting the topic from scratch, but in general there are just a few things you need to create a working genetic algorithm: 

1. An initial population of 'individuals'*.
2. A method by which two (or any other number) of parents can reproduce to create a new individual. 
3. A method to judge the fitness of each individual.

**An 'individual' is the work used to describe just one evolvable thing, with one set of genetic material. In genetic algorithms we talk in terms of individuals and populations.*

If you have never looked at any machine learning before and haven't come across the idea of a 'cost function' then you might be a bit confused about what we mean by calculating the 'fitness' of a solution, but really this is just a number which you assign to a solution to say how good it is. For example, if you are evolving a seating plan for a dinner, a solution where lots of people were sitting next to their sworn enemies and others had to sit on the floor would probably have a low fitness, whereas you would want the best seating plan imaginable to have a very high fitness. The numbers don't really matter, what matters is that more desirable solutions have a higher fitness value than less desirable solutions. 

Once you have each of these things, it is simply a case of assessing the fitness of every individual in the population and then using this fitness to decide *probablistically* how likely each individual is to produce offspring. You can then produce the offspring using the reproduction method and then rinse and repeat until you find what you are looking for. 

In one video in the series (linked in the thumbnail below), Daniel Schiffman demonstrates the genetic algorithm at work by showing an example algorithm trying to evolve to find a specific string - in this case "to be or not to be". 

<a href="https://youtu.be/nrKjSeoc7fc?list=PLRqwX-V7Uu6bJM3VgzjNV5YxVxUwzALHV
" target="_blank"><img src="https://img.youtube.com/vi/nrKjSeoc7fc/0.jpg" 
alt="Video Link" width="320" height="240" border="10" /></a>

He actually provides links to all of the code for this demonstration (see the youtube video for those), but I decided that the best way to get my head around how this all works was to make my own version from scratch, so in my next post I will be providing some generic Python code for implementing a genetic algorithm, as well as some code to evolve strings of characters.

Until then, happy coding!
