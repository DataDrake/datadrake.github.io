---
title: Solace in Solus
date: 2023-03-23
tags:
    - announcement
params:
    author: Beatrice T. Meyers
    color: red
summary: |
    It has been a long time since anyone has heard me talk publicly about my involvment in Solus. Let's get you all up to speed and let you know where things are headed. 
---

It has been a very long time since I spoke publicly about my involvement in Solus. Some of you have known me for years and others may not even know that I ran the project all of last year. In light of that, let's take a little trip down memory lane.

### Beginnings

It's Summer '16, I just defended my thesis and finally had free time. I was looking for a new Linux distro and checked back in on a project I had been following for quite some time: Evolve OS. Their Budgie Desktop was a breath of fresh air in a sea of desktop environments that felt stagnant or disconnected from the users. Surprisingly, the project had rebranded as Solus and now had semi-regular livestreams called "Hack Fests". During those streams, I started becoming more involved in their IRC circles. I installed Solus on my poor little E350 box (lovingly referred to as "masochist"), and was amazed at how well it ran on such anemic hardware.

By July, I was contributing patches to the bug tracker and packaging the software I regularly used on Solus. Crazy things like printer drivers and LaTeX distributions. Solus had very few games in the repos, so I challenged myself to package those too. I had the idea to stream working on packages and testing them out as I went. This lead to unofficial Solus Game-Fests where Josh and I would worked together to get those games added to the repos ASAP. And it was due to work like this that I was invited to join the Solus Core Team in late 2016.

As a Core Team member I could push packages directly and "cut out the middleman", getting more done in less time. I slowly became more involved in the new Phabricator Dev Tracker and helped triage issues and patches. We adopted Differential to handle patches and things really started to hum along. Offline, I started my PhD program of study and Solus became something I really looked forward to after a long day of classes or research.

### Middles

In 2018, life took another turn for Solus as we scrambled to rebuild our infrastructure. "Drake & Josh" became the duo running Solus. Josh focused on user experience, especially GUI applications, and I became deeply embedded in tooling as Tech Lead. Advances in our packaging process enabled us to expand the Solus Team greatly and create the Global Maintainers. This dedicated group was empowered to take a load off our shoulders, so that Josh and I could focus more on development and less on maintenance.

Several times over the next few years my personal life became more difficult. Be that suddenly needing to move to a studio apartment, exceedingly long hours doing research, or my internal struggle with mental health. Solus became more than just a side-project for me during those times: it was a place where the world made sense, where people appreciated the work I did, and where I could take a break from life's troubles. But it was undeniable that my mental health was on the decline and COVID was the final straw.

### Ends?

Throughout 2021, my mental health was slowly chipped away and I suddenly had much less time and energy for Solus. This increased friction between myself and the team, unfortunately leading to a schism. Mind you, it was never my desire to run the project in the slightest. I have always felt that I work better when I can focus on the next big problem and rely on others to take care of the day-to-day. I was suddenly running Solus by myself, while having to cope with my mental health. I didn't really want this, but it was that or end the project.

It was undeniable that I was spending less and less time working on Solus. True, I could point to changes in my personal life and employment status taking up much more of my time in 2022. But the reality was, burn-out had set in years ago and I was pushing myself to breaking. It meant delegating more and more of Solus to other team members; spending less time on our forums and dev tracker; livestreams stopped. Our team grew as I invited more people to join and take on bigger responsibilities for Solus. But that was not enough. And then came the infrastructure outage at the start of 2023.

I still don't have a clear picture of what caused the outage. I know that it was a network issue with the Xen network drivers, but root cause wasn't important in light of a continued lack of service. Unfortunately, the next few months were full of trials and tribulations offline. Everyone in my family unit was either sick, getting surgeries, or taking care of everyone else. And the stress of knowing the outage was ongoing and that I was powerless to do anything about it? That broke me.

So it should be no surprise that in April, the team asked me to step back and let other folks take a bigger role in running the project. I won't lie, that was hard to hear. It took a couple of days for me to process and reflect on what I actually wanted. And that's where this gets hard. Really hard.

It's time for me to leave Solus.

I want to thank everyone for their support over the years. Solus is so much more about the users than any one of us. I am proud of what we accomplished together. Solus has been a second home to me. I've met many wonderful people, had countless conversations stretching into the wee hours of the night, and have felt so lucky to be part of it all. But it is time for Solus to go on without me.

I am resigning, effective immediately.
{ .text-center }

### What's Next

By now, many of you know I have a passion for open-source software and that Linux is where I am most comfortable. Through many Friday night livestreams, you have seen me work on anything from hardware design to video games. And that's not really something I want to give up. But what I do want to do is take some time to re-center and plan my own path forward.

I would also like to set healthier boundaries and habits when it comes to working on those projects. This will mean focusing on one thing at a time and working at a pace that is both reasonable and healthy. There will be times when I don't stream and others where I use streams to take a break from the chaos of life and just hang out with folks. This will mean that things will take longer than people may be used to, but I have always advocated for the slow and steady march of progress.

Here are some things to expect from me in the future:

**Back to Livestreaming**

No matter what I decide to do next, I hope to return to Twitch and spend time with all of you. Sometimes that may be catching up with people and playing video games. Sometimes I'll sprint through my current software project. Or I might even be returning to my hardware roots and working on embedded systems.

**Updated site with more blog posts**

Just in case this 1.5k+ word entry wasn't clear enough: I want to keep documenting and discussing what I am working on. To start, I will take a few things I learned from working on the Solus site and apply them to my own. Eventually, I will resume development of static-cling , making it easier to update my site. But what I would most like to happen, is much more frequent content.

**Library Development**

There are a great many software projects that I have started and have yet to create. To that end, my development efforts will first focus on a core set of libraries for writing applications. First, I will be finishing my rewrite of cli-ng for its v3 release: overhauling the command structure to allow for more than one group of subcommands, building a robust option parser, and moving to Go templates for man pages and help text. Second, is a new Go library called stateless to make it fully generic to define stateless configurations. Third, I will be implementing a Go DBus library that will take cues from cli-ng to avoid having to write much of the boilerplate for introspection and the like.

**Software Development**

As I've already mentioned, I'd like to wrap up work on static-cling so that I can use it to more rapidly update my site. But there are many applications I'd like to revisit and others I'd like to start. One of the first will be a fresh look at todo where I'll clean up some of the code and make it more reliable. sup will get ported to the stateless library to make theming even better. I'd like to revisit my haste-it-server implementation and release something that people will actually want to use. There are other things I'd like to work on as well, but I'm not ready to talk about those yet.

**Distro Development**

It should be no surprise that my passion for Linux goes on and that I still feel like I have much to give. While I won't be working on Solus, I have learned a ton from doing so and would like to bring that all full circle. I'm not ready to announce what that will look like, but I will say that I am not going to compete with other distros. My goal is to simply continue pushing for a technically excellent base for building and distributing Linux environments. That may result in a distro that is more research than providing loads of options, but time will tell.

**Hardware Design**

No worries, I haven't forgotten about picodeck. I will return to that and other projects as soon as electronics supplies become more stable and I have the financial means to fund those projects.

This is hardly a comprehensive list, but I really want all of you to have a good idea of what I am up to next. And I hope you will stick around and follow my progress. I love being able to share what I'm working on, to educate, and to have fun hanging out with like-minded folks.

### Closing

This one got a bit longer than I expected, but thank you so much for reading to the end. It means a lot to me that there are people out there that are interested in the things I want to do. To say nothing of how your support gives me the motivation to keep going. I am grateful to you all. This is me signing off for now, but keep an eye on my social media because I am not going anywhere!

Cheers,  
*— Beatrice*
