---
layout: post
title: Genetic Algorithms 3 - Parameters
---

Before I set of into the world of world of parameters in genetic algorithms, I will show you why they are important.

Remember this image? This is the algorithm evolving the string "to be or not to be"

<div>
  <img src="../images/short-evolve.gif" alt="Evolution of to be or not to be" style="width: 100%">
</div>

Evolving this short string all goes pretty smoothly, but look what happens if I now add a few more characters onto the end of the string:

<div>
  <img src="../images/bla_increased.gif" alt="Evolution of slightly longer string" style="width: 100%">
</div>

In this new example, I have only increased the length of the string by ten characters, but it takes much longer for the algorithm to find the solution.

Of course we shouldn't be surprised by this; finding a string in the pool of all random strings is a problem which scales exponentially. That is to say, for every character I added onto the end of the string, I increased the size of the problem by a factor of 27. But if you look closely at what is going on, you will see that the algorithms reaches a solution which is nearly perfect quickly and then hangs at that point for another 100 generations or so, unable to correct the final letter of the string which it has wrong.

(As a side note, it is a complete coincidence that the final letter the algorithm gets wrong is the final letter in the string; it doesn't search for the letters in any order or anything like that.)

I don't know about you, but I intuitively feel that this shouldn't be the case; there doesn't seem any reason that it should be harder for the algorithm to find the final letter than it was to find any of the other letters, but to understand why this is happening we are going to have crack open the process and really look at what is going on inside.
