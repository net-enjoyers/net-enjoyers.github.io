---
title: "Link collection: 1"
date: 2022-02-16
draft: false
---

# Mateusz

## [Efficiently Generating a Number in a Range](https://www.pcg-random.org/posts/bounded-rands.html)

You never thought about your random number generator.
It _just worked_ and you never noticed it to be off - except maybe for it's slow performance.
Meanwhile this posts proves that there are people that are thinking about this like it's the basis of computing.
Going over every little detail from correctness (!) and speed, and still one upping each-other on their implementation.
The absolute madness to actually observe that doing the fast and simple...

```c
int random_var = rand() % range;
```

...is biased is beyond me, but it's so obviously wrong, I'm embarrassed not noticing it earlier.
Overall a good read and some easy algorithms to maybe take with you on an embedded journey.

## [Performance Speed Limits](https://travisdowns.github.io/blog/2019/06/11/speed-limits.html)

More of a source of knowledge rather than a blog post to read but interesting nonetheless.
Going from the simplest statement.

>CPU can execute only a maximum number of operations per cycle

And ending up in memory bandwidth, data dependency chains, reorder buffer size and imperfections in the physical scheduler of the CPU.
Reading even a third shows sheer complexity and at the same time explains why you can't no longer say that some CPU is faster in every way compared to another.
Seeing that even the CPUs that we assume are "toys" are actually faster than supercomputers were in the 1995 is staggering.
That might me taken as an achievement but it's actually a sad thing that computers that simulated nuclear reactions in 1995 can now fit in your pocket and still take a couple of seconds to send more then a kilobyte of text.

## [GPS](https://ciechanow.ski/gps/)

Do you know where on the planet earth you're situated at this given moment?
Probably yes...
In the odd case that the answer is no, you can pin point your location using GPS.
But how does it even work, you just enabled something and you can in real-time monitor street turns as they pass you, but _how_?
This blog post - although long - gives the best explanation through trying to develop such a system from the ground up.
The interactivity provided is stunning and I dread every time I look at it because it had to take a long time to make.
I adore how some thing in this are posing a big problem - like clock sync - but in the end it just all nicely collapses into a plain and simple thing.
It's like this wants to be created, like a math equation that is just waiting to be discovered. 
