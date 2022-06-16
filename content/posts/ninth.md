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

# Antoni

## [Trying too hard](https://www.collaborativefund.com/blog/trying-too-hard/?ref=refind)

> McCrae later wrote that he actually felt fortunate for having never heard of the rare disease.

Having experience is a great power and with great power comes great responsibility. What is even more important than experience is the awareness of your experience, so every time you are starting to solve a problem you are aware of certain possibilities because of your experience. But, never, ever, be certain about the solution and rethink it appropriately. To be precise, I am not talking about small problems like which toothpaste to buy or whether to put logic inside a constructor. My focus is on more complex problems, non-linear, where there is no the best solution and you have to make a tradeoff. I don't want to become a person who when shown a complex problem sees a solution immediately. And when I become one please slap me in the face.

This is a very important mindset in communication. Every one of us has a certain experience in life and has met multiple people. We often fail short of a fallacy to immediately evaluate someone based on our experience. We think that we have seen it before and we know the *correct* solution. That is the biggest fallacy in our perspective on communication, that there is an ideal solution, no there is not. Every situation is different and we should thrive to put mental processes when they are needed. To be more precise I am not talking about a situation such as arguing whether we gave back money to someone or if yesterday was raining. I am talking about bigger ideas like social media usage and whether they are helpful. My personal experience is that I cannot use them but at the same time I see multiple use cases when they can be helpful provided that you spent enough time on tuning what u see and read. I never want to be the person that tells someone to not use it without explanation or rethinking. I don't want to be close-minded

> A truth that applies to almost every field is that it’s possible to try too hard, and when doing so you can get worse results than those who knew less, cared less, and put in less effort than you did.

I had this feeling multiple times, that I worked hard, spent so much time on something, and at the end of the day comes someone and solves the problem in a few minutes. This for a very long time was irritating for me and I was thinking bad about the others, that they are stupid and they don't know what they are doing and got lucky to find the solution. But what came to my realization lately is that most solutions are really simple and should be. What differs is the process it took to find it. What took me days for some it would take minutes. Every mind works differently and has unique triggers and properties.

At the same time, I do not want to be the person from the previous paragraph, who acknowledges the situation. I want to be the person that is proactive in this matter and tries to find the simplest solution and not "walić głową w ścianę". I want to have the awareness when my mind is too tangled up and my thoughts lead me to the no man's land. I want to have the courage by myself to admit that I was wrong and move on. Don't treat me and everything so seriously, but rather treat it as a mystery that should be seen, doesn't matter how you solved it and how many times you failed.

Now comes the scary part, the behavior I have described before is being systematically enforced on people. Yes, we made it to ourselves.

> Being an expert from an era that no longer exists

Something didn't work in your era and you think it cannot work at all. But is very far from the truth and can lead you to a very closed mind. The quote from Henry Ford compelled me *"I am not particularly anxious for the men to remember what someone else has tried to do in the past, for then we might quickly accumulate far too many things that could not be done."* I also remember the quote from my English teacher that told me about a boy that heard a super-fast guitar song and managed to learn to play it. When the author found out about it he had to see it with his own eyes because it was impossible. He made the song by digitally tuning it to sound faster and thought it is impossible for a human being to play that fast.

What these stories teach us is that we have to allow other people to make mistakes. That is the only way they can surprise us positively and make a change, invent, and create. It can seem counterintuitive, to have the best outcome you have to allow to produce the worst outcome. I want to be the person that allows others, including myself, to make mistakes because only out of mistakes do truly interesting things happen. 

I am really angry at the current educational system because that is exactly the opposite of my words. But this is not the place for this elaborate. I will do my best to save my kids and hopefully the next generation from this piece of crap.

> Career incentives can push complexity in a field where simplicity leads to the best outcomes.

This is the direct outcome of our current educational system. Falsely building authorities and making people listen to them. Creating rules and making people dumbly obey them, what is more, punish if you don't. Social pressure to be like everyone else. Yes, you do not have to look anymore, doctor giving you the wrong prescription is being deceived by the same mental model that he learned at school. To be able to repeat, does not matter what.

## [How doctors choose to die](https://www.theguardian.com/society/2012/feb/08/how-doctors-choose-die)

Coming back to a happier topic, death. Yes, some perceive it as a happy one, the doctors. They are not afraid of it and want to optimize the process of dying. What struck me is how little treatment they undergo, because they see it only as prolonging suffering. It is better to leave the world by your rules, happily, and be remembered in a way that you want to.

> "Promise me that if you find me like this you'll kill me." They mean it. Some medical personnel wears medallions stamped "NO CODE" to tell physicians not to perform CPR on them.

It turns out that most life-saving techniques we are aware of are not necessarily the best for the patient. The part with CPR amazed me, I was not aware of it, that it does more harm than good, wow. 

> He went home the next day, closed his practice, and never set foot in a hospital again. He focused on spending time with his family and feeling as good as possible.

Doctors see the death as it is, they know the risks, the options, and the pain that comes with it. So they make cold calculations and focus on personal well-being. That is counter to our culture which shows us on every corner to do everything possible to save a life. To make an emotional explosion when life is on the line. You can surely imagine a movie scene where the family is crying when someone does not agree to chemotherapy. We are seeing death differently than the doctors, should it be this way? 

We have this basic instinct written in our minds, to do everything to save someone, but maybe that should not be the default. Maybe we should look at death as part of life and not get so emotional and panic, reconnect our society with death again. I bet in the past people talked about it as a normal thing, not it became a taboo which you want to avoid to not make others stressed out, which is plain old stupid. The more we avoid being uncomfortable now the worse we will come when it finally comes.

I have some fresh personal experience regarding this topic and I can assure you that people that talk about possible death and are aware of it are the ones ready for it. Others that avoid the topic are caught off guard and start to panic, and behave unreasonably. To be precise, I am not talking about the people dying, because when someone is dying he should be treated as partly unconscious. I am talking about the people around the dying human. There are two possibilities currently:
1. the person before his illness communicated how to treat him in such a situation
2. we don't know, we panic, we want to save him/her and do everything possible, because otherwise, we will feel guilty

Unfortunately, currently constructed public debate and awareness about death do not include the third option:

3. we all have common sense about dying and listen to the doctors, so we can optimize an ill person's last days to be comfortable for him/her

I encourage you to think about your death, and how would it be, because that is the missing point of our debate. We taboo the topic not because it is uncomfortable for others, but because it is uncomfortable for us, we don't want to think about our death. That makes us unable to think about other people's death and we treat it as the worst thing that can happen, so we lose our heads, panic, and act unreasonably. 

Don't think about your death now, don't force it, but if the time comes don't be afraid. If someone around is dying don't change the topic but discuss it as you would do normally with other things. I think that is a great emotional investment to think about now, so later you can make better decisions, and feel better in such a situation.

I want to end this with big words of respect for the doctors who are doing their work as they think is best and don't fall into an emotional rollercoaster because that is the ride when no one wins. The job of a doctor is almost impossible for me to imagine, the level of shit that you see. The level of sadness, panic, irrationalities, and stupidity that you see on daily basis. You are like a guard for people where you guard them against themselves. Thank you.
## [Doing less bothers me](https://radreads.co/80-20-rule/?ref=refind)

Lately, I am having these discomfort thoughts from time to time. That I am not doing enough, that there are so many options and I am passing on them. I know so many people but I am seeing only a small fraction of them. So many interest areas but I am focusing only on a few. This feeling is very very uncomfortable and many times makes me wonder whether I am lazy, conformist, or passive.

I am aware of it and after some analysis, I am deeply sure that this feeling is good for me. I am changing my world perspective. I am changing how I was educated and brought up. I am changing my personal preferences and temper. In broader time scope it finally allows me to accomplish things that were impossible for me. Before I was making plans to learn something e.g. programming. I thought, yeah, this summer I will learn it. In my mind it was like I have to work super hard, I have to make astronomical steps at a time, and learn it all in one night. And it overwhelmed me, I was afraid to even start. What is more, I was bragging to myself about inaction, I viewed myself as lazy, unproductive, and unable, it didn't help me. Toxic ambitions indeed.

Now my perspective changed a bit, I am doing less, but consistently. That is a great realization. Although I heard it many times it took some time for me to truly understand it. I do not know when I truly realized it but I am thankful for it. Now I am more grounded in my goals, I know how much it takes to achieve them and that it will take many small steps instead of a few big ones. And small steps are easy.

So I feel like every day I am doing easy things, so I am not progressing, but at the same time if I look back I see tremendous progress. Very interesting feeling and I am still learning it. I hope with time, every day I will be aware of the importance of small steps and how they fit into the bigger picture. So the doubts will sound funny in my head.

In Poland, we have a saying "z Korwina się wyrasta", which means you grew out of certain things. My thesis is that we do not grow out but the thoughts about certain things just start to feel funny and unreasonable. We look through them. Spot false actors. Maybe growing up is like becoming a lie detector for ourselves?



