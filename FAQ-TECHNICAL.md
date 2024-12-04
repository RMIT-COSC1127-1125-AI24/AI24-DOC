# FAQ - Technical - RMIT AI COSC1125/1127

This FAQ contains some common technical questions.

- [FAQ - Technical - RMIT AI COSC1125/1127](#faq---technical---rmit-ai-cosc11251127)
  - [Is stochastic and non-deterministic the same?](#is-stochastic-and-non-deterministic-the-same)
  - [Are HSLD and Manhattan distance same?](#are-hsld-and-manhattan-distance-same)
  - [In terms of evaluation function `f(n)`, is A\* search combination of uniform-cost search and greedy best-first search?](#in-terms-of-evaluation-function-fn-is-a-search-combination-of-uniform-cost-search-and-greedy-best-first-search)
  - [Are uniform-cost search and best-first search the same?](#are-uniform-cost-search-and-best-first-search-the-same)
  - [Do I have to use every clause in a resolution proof?](#do-i-have-to-use-every-clause-in-a-resolution-proof)
  - [Can we use a clause more than once in a resolution proof?](#can-we-use-a-clause-more-than-once-in-a-resolution-proof)
  - [Can we resolve more than one literals in one step?](#can-we-resolve-more-than-one-literals-in-one-step)
  - [Are starting utilities initially set to 0, or to the reward for that state?](#are-starting-utilities-initially-set-to-0-or-to-the-reward-for-that-state)
  - [How should I structure a proof?](#how-should-i-structure-a-proof)

## Is stochastic and non-deterministic the same?

Not quite. Both refer to the issue of an action having not just one effect, but one out of a few possible effects. The usual example is rolling a dice: there are many possible effects, and one will ensue. 

This could happen because nature is inherently non-deterministic (quantum? Check post [Is the universe fundamentally deterministic?](https://physics.stackexchange.com/questions/63811/is-the-universe-fundamentally-deterministic) if interested...) or most probably because you have _incomplete_ information (about the exact effects of the action), you don't know all the details and mechanics to craft ``the'' effect.

So the question is at what level one _models_ that phenomenon (of nature or uncertainty). If you attach a ``weight", a probability, to each possible effect that could ensue, then you are building a _stochastic model_. MDP and RL (we'll see them later) are those type of models, where every possible transition between states is annotated with a probability of that effect happening.

On the other hand, if one just wants to state what could happen but not say anything about their relative weight, then you are doing a _non-deterministic model_. This is the case of Fully-Observable Non-deterministic Planning, for example. That's all, it's about _modeling_.

It is important to observe that a non-deterministic model does _not_ mean that every option has the same probability. No! It means you just don't know the exact probabilities. Basically, you just know that the probability of each effect is greater than 0, but nothing else...

##  Are HSLD and Manhattan distance same?

No. HSLD is the straight-line distance heuristic. Straight-line distance is the distance that we measure with a ruler on a paper map by aligning two points, say from A to B.

And Manhattan distance is the distance between two points in a grid based on a strictly horizontal and/or vertical path (that is, along the grid lines). It is the sum of the horizontal and vertical blocks.

In this Figure, Manhattan distance is 10, However, determining HSLD requires more calculations.

![H_SLD-vs-Manhattan.jpg](img/H_SLD-vs-Manhattan.jpg)

## In terms of evaluation function `f(n)`, is A* search combination of uniform-cost search and greedy best-first search?

In some (conceptual) sense, _yes_!

In A* search, the evaluation function is $f(n) = g(n) + h(n)$, where, $f(n)$ is the path cost from the initial state to the search node `n`, and `h(n)` is the _estimated_ cost of the shortest path from n to a goal state. So, `f(n)` is the estimated cost of the best path that "continues" from `n` to a goal state.

Greedy best-first search expands first the node with the lowest `h(n)` value (the node that appears to be closest to the goal). So, the evaluation function `f(n) = h(n)`.

In uniform cost search, evaluation function is the cost of the path from the initial to the current search node `n`. So, evaluation function is `f(n) = g(n)`.

## Are uniform-cost search and best-first search the same?

Dijkstra’s algorithm or Uniform-cost search is Best-first search when the evaluation function is the cost of the path from the root to the current node. So, UCS is one of the many possible instantiations of best-first search.

## Do I have to use every clause in a resolution proof?

No!

It helps to remember what a resolution proof is actually doing, rather than just thinking of symbols moving around on paper. You have a knowledge base which represents a lot of things you know about the world. For example:

1. Bob is a cat, 
2. no cat is a dog, 
3. elephants are large, 
4. Edwina is an elephant, 
5. cats are not large, 
6. ....

If you are trying to prove 'Bob is not a dog', then you can intuitively see that you should only need facts 1 and 2. If your resolution proof requires facts 3-5, something has gone wrong!

## Can we use a clause more than once in a resolution proof? 

Yes, see answer to prior question. Just because you have used a fact, does not make it become less true after the fact.

## Can we resolve more than one literals in one step?
No, this is technically incorrect. Review the textbook, or see [this question](https://math.stackexchange.com/questions/1506990/logical-resolution-why-only-one-pair-of-complementary-literals-can-be-used)

## Are starting utilities initially set to 0, or to the reward for that state?

This is just a matter of convention. In an assessment we will make sure the explicitly specify what to do.


## How should I structure a proof?

In general if you are asked to prove $X=Y$, you generally want to prove this "in one direction", rather than "meeting in the middle". I.e. set up the proof in the form of a series of statements. $X=X_1, X_1=X_2, \ldots, X_2=X_n, X_n = Y$ Rather than $X=X_1, X_1=X_2, \ldots, X_{n-1}=X_n, X_n = Z$ and $Y=Y_1, Y_1=Y_2, \ldots, Y_{n-1}=Y_n, Y_n = Z$

Why is this? If you are strictly proving $A=B$ and every statement is of the form of an equality, then I think it is mainly a matter of style. But you are often only proving $X\Rightarrow Y$, in which case $X\Rightarrow X_1, X_1\Rightarrow X_2, \ldots, X_2\Rightarrow X_n, X_n \Rightarrow Y$ is a valid proof, but the other form is not. (Why? This is left as an exercise to the reader, try to come up with a counterexample.)

I do find sometimes it is more natural to meet in the middle somewhere, but once you have the actual links you need, it is best to rearrange into this standard form. 