---
title: "Link collection: 9"
date: 2022-06-14
draft: false
---

# Mateusz

## [Backblaze B2](https://www.backblaze.com/b2/cloud-storage.html)

For a long time now I knew that I'm asking for trouble storing all the files that I care about on my main and only hard drive.
If it breaks all my files that are close to me are just gone.
It's sort of a weird trick that the mind is playing on you.
You do not need all those files, they are not crucial, your life does not depend on them.
People from [r/DataHoarder](https://teddit.net/r/DataHoarder/) will tell you otherwise.
That storing all your shows that you will watch once on your sever is something that you have to do.
But come on, if you have a server that can store all of that you have an internet connection that will be able to support downloading 4K video on the fly.
But back to the point.
I believe that most of these files that I want to save are not important, but some are and I want to keep them safe without must hustle.

I've seen Backblaze B2 recommended over on HackerNews and tech Reddits alike.
At first it did not appeal to me, $5/TB/month - but I only want to store like 100GB at max currently.
Paying for 10% of the capacity is not desirable - and then it hit me.
They actually charge you for what you use.
So for me (having uploaded 40GB) the cost per month is 40GB * $0.005/GB/month = $0.2 or 20 cents.
Come one, 20 cents is nothing and the files are safe!
I do not want to store my files on Google Drive as much as I trust that they wont disappear.
The thing I do not trust is Google itself, relaying on them for this will pull me back in to their walled, camera infested garden. 

Right now the solution is not perfect, it's not 100% catastrophe proof.
But if the servers of Backblaze will no longer be able to run then are my stupid files even something I care about?
There is a romanticized idea of self-hosting a backup in form of a HDD strapped to a Raspberry Pi.
But at the time of writing Raspberry Pis are in a worse state than graphics cards when it comes to stock.
And before anybody even thinks of "Just buy a Dell Optiplex and you are going to have more performance and more SATA...".
Just stop.
My home is not suited for a stray steel box that is going to be running of power 24/7.
Just take the Backblaze route, it's cheaper and more reliable - you'll most likely pay less for Backblaze monthly then for the electricity of your stupid Dell Optiplex.

## [rr: record and replay](https://rr-project.org/)

I do not have much to say about this expect that I've used this for two days and all I have to say is: wow.
First of all, the installation is not as clean as I would like it to be but the usage makes up for it.
The basic interface that will allow you to get all you need is

```
$ rr record <your program>
$ rr replay
```

And boom, your are inside GDB where you are always debugging the same run.
If your bug is something that happens once in a blue moon then this is the way to catch it.
The ability to reverse step is nice but let me get to the best feature of this right now.
Read/Write breakpoint on a variable and reverse continue.
If that does not ring a bell then you won't be impressed by this.
The ability to see where the variable was set all of it's call frames and debug it like nothing happened is god power.
You can debug thing that would take you quite some time in a complex system that you are not that familiar with and or is poorly designed in minutes.
If you work in any compiled language like C/C++/Go/Zig/Rust give this a try.

## [Benchmarking Malloc with Doom 3](https://www.forrestthewoods.com/blog/benchmarking-malloc-with-doom3/)

Do you know how `malloc` works?
I thought I did but apparently there are many things that are still not understood by my brain.
After reading the blog post I was like: why, how, the big gap???
All I want to do on a quiet Sunday afternoon is start reading and understanding some of these allocators to get the insight.
You know you are never going to use that knowledge, but it's going to help you make better decisions in the future.
