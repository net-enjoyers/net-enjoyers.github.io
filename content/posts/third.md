---
title: "Link collection: 3"
date: 2022-03-14
draft: false
---

# Mateusz

## [Wide-band WebSDR](http://websdr.ewi.utwente.nl:8901/)

Electromagnetic radiation is a spectrum so incredibly attached to today's humans it's hard to imagine life without it.
From radio, WiFi, Bluetooth, 4G/5G, TV, Roentgen pictures and to the most important - visible light.
It's all around us, thanks to it, you are able to read these words.
But such a high number of these is invisible to us it might actually not exist.
How do so many of these great technologies work, communicating (at the speed of light!) between each other with ease?

Answer: it's waves!
You thought you can escape them, I thought I can escape them.
The wave equation, nightmare of my physics course, I dread even thinking about it.
Sadly the truth is that, it's all a wave.
Thanks to Joseph Fourier we know that any signal is just a collection of different sinusoids.
Skipping over some bits, using that knowledge we can transmit our desired sinusoid and still be able to pull out just the one we want at the receiver.
The medium that will allow all of this to propagate is the aforementioned electromagnetic radiation.
Anybody with a flashlight is creating a field of it around them.
It's so easy to create and receive it might as well be the reason we are at this current technological level.

Well, if we have a high level of technology, and we heavily used radio to get to it shouldn't we combine the two?
As always if you think that you had an original, once in a lifetime thought, someone already had it years before.
Same here, the field of **Software Defined Radio** (SDR) is spreading it's wings and it's doing it fast.
For 20-40$ you can get a USB dongle that will allow you to receive any signal starting from 24MHz and going up to 1.7GHz with a bandwidth of around 3MHz.
If you think about it, it's insane, you can without problem receive multiple AM radio stations **at once**.
If you do not want to pony up the cash to see if it even is for you, try having some fun with this website.
You have unlimited access to 0Hz-30MHz which allows you to listen to radio stations, military requests and some hobbists that are licensed.
I highly recommned checking out the chat page, where people share the exact frequency and modulation scheme of some interesting broadcasts. 

## [A history of NVidia Stream Multiprocessor](https://fabiensanglard.net/cuda/index.html)

Things should be as simple as possible, but not simpler.
Is a nice way to describe what NVidia had thought to them selves after unleashing Streaming Multiprocessor (SM) model into the world. 
Going back, think how would you create a graphics core that is responsible for a tightly defined number of things and needs to be fast.
First things first, single purpose is **always** faster over generic.
Well, if you know that you're going to be the bottleneck in any system then just create single purpose hardware sections that are going to be responsible for different stages of 3D graphics.
Create an ASIC for triangulation and pixel filling with all the modes you need to support (remember that OpenGL did not support shaders until version 3).
Sweet!
Now you all need to do every two years is increase VRAM size and introduce more ASICs into the GPU.

Well, it's not so simple.
You can't just dream in your imagined land and say that your performance benchmarks rip and tear when the customers and seeing something completely different.
Not all 3D scenes are the same, some are going to require mostly triangulation while needing only a simple pixel fill, while others are going to be completely opposite to that.
Now game companies have to play into your hand and pray for you to keep the same ratio of performance between triangulation and pixel shaders in newer editions of cards to extract 100% from the hardware.

What if you ditch the ASICs and all of the ratios between different stages?
Just create processors that are generic enough to be competent at all stages and you have no problem with ratios.
You are always going to use 100% of your card, because cores that are not doing triangulation can become pixel filling machines.
That is what NVIDIA has done and what is so masterfully described and visualized in this blog post.
I don't want to introduce confusion so I'm going to recommend you read it now if you're interested.

## [Apple M1 Ultra](https://www.apple.com/newsroom/2022/03/apple-unveils-m1-ultra-the-worlds-most-powerful-chip-for-a-personal-computer/)

Apple is on a mission to pull the pants of all modern x86 processors.
Their new processor M1 Ultra is just a page from AMD's book and they glued their best processor effectively creating a [R9 295x2](https://en.wikipedia.org/wiki/Radeon_Rx_200_series#Radeon_R9_295X2) of CPUs.
The claims are out of this world and it makes me so happy and so terrified at the same time it's making my head whirl.

Why happy?
We are stuck.
Stuck on an ISA that was created on a whim and thrust into the stratosphere as the de-facto standard by IBM.
I like x86 but is it Stockholm Syndrome?
Maybe...
The fact that ARM is reaching performance levels so high is so encouraging because it means there is a different way to this CPU business.
Also, another player on the duopoly market that we had for basically 20 years is fantastic.

Why then terrified?
It's Apple.
I and you know they have some skeletons in their closet.
They are fiercely anti-consumer and try to integrate everything into oblivion.
When my AMD/Intel CPU breaks, I'll just get a new one.
In the case of Apple silicon CPUs it's a high speed ticket to "Purchase a new machine".
RAM is not upgradeable, [SSDs are questionable](https://nitter.net/marcan42/status/1494213855387734019#m) and the overall hackability of this platform is the lowest of them all.

All and all, it's an achievement that I want to follow.
I'm eagerly waiting to see what kind of performance they managed to create.
Probably 2x is maximum that it's possible to achieve in the baseline from MacBook Pro's.
And even that is a stretch because the connector they use is a bottleneck.
I know that they say that it's amazing - well because they have to, it's their PR talk.
History of AMD showed us that if you can you want to get rid of the high speed bus between the cores as fast as possible.
I want to get rid of this stale market even faster and experiment with all the new and creative uses of silicon.
Let the Moore's law never die.

# Antoni

## [Who stole my focus?](https://www.vox.com/vox-conversations-podcast/2022/2/8/22910773/vox-conversations-johann-hari-stolen-focus?ref=refind)

Why is that we all know the current problems and have the ideas to solve them but actually nobody is doing anything. And when someone is doing so, getting people onboard is the biggest struggle? Why are we worrying so much, discussing it but when it comes to execution the initiatives phase out because of lack of interest?

Take for example buying local products. Why small companies have such a hard life when they offer a)better quality b)lower prices c)more environment friendly business model? Why always the answer is "they don't market themselves, people don't recognize them"? Why people buy worse products at higher prices just because they are being sold under "The Brand X" logo.
And when trying to solve this problem we are making marketing campaigns "Buy Local Products". Why nowadays everything has to be sold to us, gave in front of our eyes, whispered in the ear? Why we cannot just be informed, reason about the problem and take actionable steps?

I have a pretty bold thesis **that the problem is not with ourselves**. Current digital world has been constructed in such a way to make us unable to take action. We are only being fed with **illusion of action called click**. 

I know it sounds evil, but actually nobody (probably) is being evil. Only the system is broken. It promotes exploit of other human being. It starts a loop where consuming more distracting content makes content more distracting. But what if at some point everyone become distracted. And what if it happened already? How could we know?

> We need to just say that a business model premised upon discovering the weaknesses in your attention in order to hack it and sell it to the highest bidder is fundamentally immoral and inhuman like leaded paint, and we will not allow it.

> It’s like we’re having itching powder dumped on us all day and then we’re being told, “You know what, buddy, you might want to learn how to meditate, then you wouldn’t scratch so much.” We need to get out of this psychology and remind ourselves that we’re not medieval peasants begging at the court of King Zuckerberg for a few little crumbs from his table. 

**Ban the “surveillance capitalism” now.**

## [What am I willing to struggle for?](https://www.youtube.com/watch?v=jrVvwnh9eKA)

When you become great at something what you remember about the process? For me it is those little moments during which I had thoughts to give up but decided otherwise and **keep on struggling**.

I have been having such thoughts about life lately, that it is composed mostly out of struggle. Living a proactive life is just a decision whether you want to struggle for something. And a very important idea is that our **struggle-power** is limited, so we have to choose our values wisely.

But why to define own life in such a negative manner? Have I forgotten about positive psychology? No, I have just redefined my world perspective. Instead of looking at events in the manner of good and bad, positive or negative, I look at action and inaction. Something happened or did not happen. And that is our biggest constraint, we are not physically able to make everything happen. We have to choose. And the good choice is indeed the hidden gem of it all. If we decided to do something which is inline with our goals we will unleash a lot of our **struggle-power**. 

Does **struggle-power** makes us constantly happy? NO.<br>
Happiness is just a part of the whole process, not the end goal. As it is said in a famous Polish song "W życiu piękne są tylko chwile".

So what differentiate accomplishments from failures? **Struggle Power** (and a bit of luck ;-D)

