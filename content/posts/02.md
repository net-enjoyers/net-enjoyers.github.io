---
title: "Link collection: 2"
date: 2022-02-28
draft: false
---

# Mateusz

Taking a look back to materials that made a lasting impression on me very few blog posts come to mind.
I take this as a weakness of mine, but I ask for your attention regardless.

## [Physics is going to be finished in six months](https://www.youtube.com/watch?v=KD3BeEDr0Gk)

Thinking that you are something greater that you really are, is a trope that each homo sapiens embodies.
Being an expert in a given field boosts your confidence to absurd levels but not equally in each specialization.
A professional stonecutter is far more confident is the things he's saying then a scientist.
This does not mean that one is superior from the other, in reality quite the contrary.
The job of a scientist in one sentence is "Doubt from the start. Don't believe, know from empirical data."
Taking this to the extreme and extrapolating to unbelievable lengths is something one can waste his time doing but simplifications are always lies.
Here we can observe how the job of a stonecutter plays with the scientist, because jobs as these can provide empirical data upon which knowledge is built.

Getting to the point of this, doubting is your job, even in yourself.
No matter how big your name is, how much credit and respect you've built up over the years you're still a monkey.
The lecture I'm speaking about shows this perfectly, and it's title is a callback to the most blatant example of this.
For those that don't know the context, Max Born (aka. One of the inventors of quantum physics) in 1927 said:

> Physics as we know it will be over in six months.

He said that in time in which many things were still popping up (like Dirac Equation not so long after this quote) yet he still came to the conclusion that nothing new can't appear on the horizon.
Such a brilliant mind, winner of the Nobel Prize, scientist whose the most basic job is to doubt, is certain about a fact that we know right now is totally bonkers.
Going over this talk puts you in your place, you may be smart, you may know this and that, but you're still a monkey standing upright, doubt is a good thing.

## [Modulo division and remainder division](https://twitter.com/ID_AA_Carmack/status/1476294133975240712)

Have you ever noticed how the modulo operator is different between C and Python in special cases?
For example:

```c
5 % 3 = 2
5 % -3 = 2
-5 % 3 = -2
-5 % -3 = -2
```

```python
5 % 3 = 2
5 % -3 = -1
-5 % 3 = 1
-5 % -3 = -2
```

What gives?
Well, the operator may be the same, but the _operation_ which it's doing is different.

- C uses *remainder division*.
- Python uses *modulo division*.

Well, what's different not taking the name into account?

As you can see in in the C example, the sign of the result is the same as the sign of the divisible (the one we want to *divide*).
This produces some inconvenience when we want to access an array with wrap around and we may produce an index that is negative.
The simplest example are [Cellular automatons](https://en.wikipedia.org/wiki/Cellular_automaton) when we want to constrict the board on the edges so that it goes back to the other side.
If we produce an index that is bigger than the dimension of the board there is no problem - modulo and remainder are the same when both arguments are positive.
But what if we produce an index that is negative?
We have to handle this as a special case, because we are going to access a completely different array index, probably even memory that is outside the bounds.
Formally this operations is called a _remainder_, the stuff that did not fit into our division.
And this is a big revelation because everybody - even myself - calls it the modulo operator.

So what is the modulo division?
First of all, sign of the result is the same as the sign of the divisor (the one we want to *divide by*).
This does not produce the same special case as above because, size of the board is positive, so we are always going to produce a positive value, even if the produced index is negative.
Okay, so what is the mathematical formalization of this operation?
If the divisor and divisible have the same sign, the result is the remainder division.
Meanwhile if they have opposite signs, the result is the remainder division plus the divisor.

I didn't want to introduce math, but some formalization for those who want to dig a little deeper.
In [here](https://en.wikipedia.org/wiki/Modulo_operation) the operation that the C language is doing uses the truncated division, while the Python uses floored division.
You can implement both variants are follows:

```python
import math

def remainder_divison(a, b):
    return a - b * math.trunc(a, b)

def modulo_divison(a, b):
    return a - b * math.floor(a, b)
```

And for those who want to use the modulo division in C, feel free to copy paste this:

```c
int imod(int a, int b)
{
    return ((a % b) + b) % b;
}
```

## [Preventing the Collapse of Civilization](https://www.youtube.com/watch?v=pW-SOdj4Kkk)

Do you save the best for the last?
Because I did.
I really don't know how to start and what to say about this.
A genius talk that I think about almost once a week.
We, a species of upright monkeys has only one real enemy, ourselves.
Now more than ever we rely on technology to keep us informed, fed and alive.
But we behave like this technology is here to stay forever and ever.
Andrzej Dragan in the talk from the first link says that a smartphone is something so complex that no one alive knows everything about it.
Systems so complex, sprawling and dense we need specialists for separate components like the screen, camera, processor, memory, OS and so on and so forth.
Camera software may even be called alien technology by this point thanks to the powering it AI.
Do humans know what those matrices mean, what does this 0.2 stand for in this particular row and column.
I don't want to come off as ignorant and discredit people responsible for this just by saying "We don't know how it works, so they don't know what they're doing".
If we knew what it was doing we'd skip building dedicated matrix multipliers like the [ANE](https://en.wikipedia.org/wiki/Apple_A11#Neural_Engine), Google's [Coral TPUs](https://en.wikipedia.org/wiki/Tensor_Processing_Unit#Edge_TPU) or NVIDIA's [Tensor Cores](https://developer.nvidia.com/tensor-cores) and produce the algorithm using ifs and loops.

But coming back to the topic at hand, there are things that people need to specialize for.
Specialization is the future, but one should try to produce the simplest design that there is.
So that even a person from a different field is able to understand the core concept behind it.
Programmers like to say they are *pragmatic*, when in reality the amount of dogmas they believe is so high it should be recognized as a religion!

Don't believe in dogma.
Give this talk a listen, and build your own opinion.
Even if you disagree with this talk, it's telling a gripping story.

# Antoni

## [Roman Abramovich will sale Chelsea F.C.](https://www.chelseafc.com/en/news/2022/03/02/statement-from-roman-abramovich)

I am not going to hide it, I used to be a big football fan. But with passing time I grew out of it, mostly from two reasons: basketball and worldview. The latter is what really goes under my skin lately. 
The whole mass sport is rotten with money, football championships are being hosted by a very questionable countries when it comes to human rights. Olympic games are being hosted by countries which have very little in common with the whole "olympic spirit". It is really causing a lot of negative emotions inside of me and makes me question where does our European values vanish in such situations. In the world that I know you can get a punishment for talking too loud during classes, but misbehavior of biggest authorities can be in some circumstances "forgotten" or "overlooked".

Yet, today something stroke me when I read this message ~ "Russian billionaire sells his beloved club". The action from this individual reminded me that we should not focus too much on single, personal, isolated case but look on a bigger picture and focus on system that traps humans in very narrow "profitable" cell. I deeply believe that almost every human being has a good heart but it is a collective misalignment at the moment that is causing us the most pain. 

We are all hunting some imaginary goal and think that everyone else are there to get us. The whole idea of maximizing competition maximizes the output is draining our society of the most valuable resource, our good will. How many truly remarkable situations happen on a daily basis. How many of us are able to resist the temptation of what our environment tells us thats right for us. Who has the courage to do what he feels that is right. Do we really want to be remembered as people that sell football clubs when the country we have ties with strikes missiles on neighbors? Are we really that weak so our only solution is just waiting for the tipping point, for the fire to put down, for the crisis to solve. Why can't we notice what's right when the negative consequences of our decisions are not yet visible.

I am very often voiceless, scared to say something that I feel should have been said, just because I don't want to hurt nobody's feelings and shake the order of reality that I live in. I think most of us also feel this way. How is it possible that we all at personal level feel what is right but nobody is able to voice it? Where do we hurry so much that we are not able to take a step back and repair what is broken when there is still a time. 

> **Fail fast, fail forward is heading us into the blind alley.** *Piano, piano, chi va piano, va sano e lontano*  



