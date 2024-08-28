---
title: And We're Back
date: 2021-06-28
params:
    author: Beatrice T. Meyers
tags:
    - announcement
summary: |
    Join me for a look at this week's redesign of the site, as well as my future plans for upcoming content. Here we go!
---

This past year was one for the history books. Both for the horrible pandemic that we were all affected by and for the technological marvel of mRNA vaccines that turned what could have been several years of vaccine development into a little over a year. Unfortunately, for my site, this was not a good year either and I'm here to break down why that was and how we are going to turn that around going forward.

### What went wrong?

It is easy to try and point at COVID as the reason I stopped writing on my blog. Indeed, I wish I had such a convenient scapegoat to point at, but the reality is far far less exciting:

1. Adding new content to the site requires modifying many more pages than you might think.
2. These modifications are highly repetitive and error-prone when done manually.
3. The lack of automation means needing to manually test the results of every modification.
4. Any change to common elements of a group or all pages requires manual updating of each and every affected page.

Just to add this new article to the site required modifying no fewer than 10 separate files. All of these modifications could have been automated with a proper templating system. Compiling the sources of the site into an updated version also means manually updating the a build script to reflect any newly created files. Doing something as seemingly simple as adding a new blog series or calendar year, results in modifying all of the blog index pages. All of this has amounted to my not wanting to deal with all of that until the situation changes.

### How do we fix this?

Obviously, you are looking at a brand new site today, so you are probably wondering: what changed?

A few months ago I got fed up with the state of things and started taking steps to find a solution. It is pretty clear that some sort of automated and templated system for content management would be an ideal candidate to solve this problem. These CMS do exist and are typically referred to as Static Site Generators. Naturally, then, the obvious course of action is to find one of these SSGs that meets my need and migrate the site over to it. But that's not what happened.

### Existing Solutions

I examined several popular SSGs, including: Hugo, Middleman, and Jekyll. All of them certainly could be used to generate my site and have more than enough features to accomodate anything I might want to do. But all of them had a few key issues that bad them a bad fit for me:

- Theming content requires either picking from community supplied themes or spending a significant amount of time building out new CSS to accomodate how each system actually generates content.
- Only 1 of the CMS I examined supported HAML for document markup or templates. HAML is much less tedious to write than HTML and has become a huge selling point for my workflow.
- All of these systems enforce strict constraints on how the site project is structured and how templates are specified. If you disagree with any of these constraints, it will become a thorn in your side when updating your site.
- These systems have a ton of additional features that I will never use, but affect build times or complicate other more frequently used features.

### A New Path Forward

It is clear then that none of these systems will be something that I will want to use regularly, so you are probably wondering: what am I going to do? Well, I have developed an approach that I am currently following to resolve all of these issues:

1. Months ago I started planning to build my own static site generator with an emphasis on ease of use while being flexible enough for users.
2. As part of that planning, I developed a project structure for sites that I believe is highly intuitive and requires the least amount of changes to migrate or modify a site.
3. This past week, I developed a new CSS theme for my site to replace suckless.css to allow for a much simpler document structure that is conducive to later writing page templates.
4. As part of developing this new theme, I migrated my entire site to a new source tree which roughly follows the structure that I will use in the site generator.
5. Today, I am deploying this new site so that I can continue to add new content while developing the site generator, but relying on this now simpler document structure to alleviate some of the complexity of manual updates.
6. On Friday, I will be returning to development of static-cling with the goal of that being the next project I complete during my personal development streams.

**Enter static-cling**
{ .text-center }

My new site generator will be following in the footsteps of existing solutions, but I have settled on a few critical constraints and gotchas to avoid:

- No requirement for specific template structure or content formatting
- Clearly defined project structure which is logical and intuitive to the end-user
- HAML and HTML for templating, using the Go text/template markup for programmatic templates
- Multiple content formats, including: HTML, HAML, Markdown, and my own TimberText
- Separation of metadata from content into YAML files
- YAML data sources which may be used by templates when generating pages
- RSS Feeds for new content

I will of course be open-sourcing this generator and hope that it will be useful to other people wanting to author their own sites. Stay tuned!

### What about DataDrake.com?

I am committed to producing regular content moving forward.

I am going to be adding a new series on Solus development, in an effort to document my ongoing development of various tooling for the project. Right now, the focus will be on ypkg 3 , but you can expect that I will revisit other ongoing efforts as time allows. At the very least, I will be producing weekly development logs where I discuss what progress was made on and off stream.

I would also like to start periodically adding articles to the other existing blog Series that I had previously added. I encourage you to check out the newly added descriptions for each Series so that you know what else will be coming in the future.

Additionally, I will be slowly working to build out other parts of the site. I have gone ahead added descriptions to each page to indicate what I would like to do with each section. Go check them out!

Most of my initial focus will be on building out the Projects section so that I can put together development logs for static-cling and all of my other adventures from the Friday night streams.

I know this is a much longer read than you all are used to from me, so I'll just leave things here by thanking you for your patience and expressing my excitement for future content!

Cheers,  
— DataDrake
