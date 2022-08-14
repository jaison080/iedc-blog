---
title: "Hello World ✨"
date: 2022-08-13T14:53:07+05:30
Description: "Reflections on the technical and non-technical aspects of the blog project by the CTO of IEDCMEC"
Tags: ["tech-team", "behind-the-scenes", "project"]
Categories: []
DisableComments: false
authors:
  - name: "Aldrin Jenson"
    about: "CSB, MEC'23 | CTO of IEDC MEC"
    website: "https://www.linkedin.com/in/aldrinjenson/"
---

Behind the scenes view into the making of IEDCMEC blog project, told by the CTO of IEDC-MEC. Maybe a bit long, but read on if you are interested about project management or the technical aspects of how the blog platform is made.

## Introduction

The IEDCMEC Blog platform in which you are reading this article right now is an initiative started this year by the tech team of IEDC-MEC. This article lists out the approach we took to build the blog, the features it has and some of the challenges we faced.

## Why we built the blog

A blog is a great medium to showcase the thoughts and literary works of the members of an organization of community and hence the blog idea was something I held very close to my heart. Every great organization had a blog site - be it technical or non-technical.

While most clubs or communities usually depend upon blogging platforms like Medium, Blogger, Blogspot etc, IEDC MEC, with it's awesome tech team (More on the IEDC teams in a later blog maybe) and a firm follower of FOSS technologies, decided to have the blog platform built in-house by our students ✨.

## Features of the blog

Major features we now have of the blog are:

- Support of both dark and light themes
- Comment feature with github auth for preventing spam
- Clap feature using [applause-button](https://github.com/ColinEberhardt/applause-button)
- Page view Analytics
- RSS Feed support (try adding blog.iedcmec.in/post/index.xml) to your RSS reader ✨
- Emoji support✌️
- Transitions effects and mobile responsiveness
- Version control (bro, we have git)
- Syntax highlighting and support for code blocks
- Extreme UI customisability
- Collaboration, proof reading and review features using git and github
- Feature for multiple authors to write articles
- Feature to show separate description and LinkedIn urls of authors (Ohh yes, beat that Medium👊)

Features for making development workflow easier are mentioned at a later section as well.

Building these many features were not a one-man effort. They were not easy as well. Read on to know more!

## How this was made

<!-- ### 1. The planning -->

#### Technical side - Deciding on Hugo:

As CTO, I had the initial say in decisions. I wanted a blog framework which didn't involve much learning curve, but also was flexible enough to be customized to our needs and be easily maintainable in the future.

Having had experience with blog frameworks like [Gatsby](https://www.gatsbyjs.com/), [Hugo](https://gohugo.io/) etc in the past, I felt like Hugo would be a safe and easier option to consider. I also had a senior Pranav Sridhar recommending me this as well.

In a nutshell, you give an article as a markdown file(more on this later) as input to hugo, and it builds out HTML blog pages based on the theme and customisations you've set. The tricky part is the customisability. I've know people who've dropped the whole idea of a blog just because this part took a long time for them to figure out.

Once the framework was decided, next step was setting up the team and providing the training.

### The Training

None of the team members had heard about Hugo before or most folks didn't initially even have much idea about why use a framework for a blog at all. So the initial part of the challenge was organizing a training session to get them up to speed.

A great help to me in this task this was [Allen Phillipose](https://github.com/alanphil2k01). He had had some experience with [GoLang](https://go.dev/) before and when I proposed to him the idea of a blog framework written in Go(Hu**Go**), he was ready to jump in.

I sent him Hugo docs and my own [personal blog](https://aldrinjenson.me/) I had made earlier where I had a [post](https://aldrinjenson.me/posts/hosting-hugo-sites-on-gh-pages/) about hosting Hugo with gh-pages as an example.
He found Hugo very interesting and within two weeks, showed me a sample blog he made.

We organized a workshop on building blogs with Hugo for the tech team. The session was taken together by Alan Philipose and me.
**[Here's](https://alanphil2k01.github.io/intro_to_hugo/)** the initial blog Alan made as training material, but was immensely useful during the session and even as a reference to the attendees afterwards. It was also shared in Tech group and I'm told that those who couldn't attend the blog also found it useful for them to try out later.
(Note to self: Remind someone to take photos of all the future workshops we conduct.)

I wanted everyone in the tech team to attend, but due to series exams for first years conflicting and the previous 2 weeks being filled with other events, we weren't able to bring in as many number of participants as I initially wanted. Ahh the troubles of organizing an event.. Event managers, I feel your pain! 🥲

One thing that comforted me was the feeling that those who attended the workshop found it immensely useful. We gave them instructions and the participants (majority of them atleast) managed to create a blog following them and have it deployed through github pages by the end of the workshop!

Next step was to **form an official team.**

### Team formation

Now, it was time for recruiting. Alan Philipose built the initial base version of the blog by choosing [Anatole](https://github.com/lxndrblz/anatole/) theme. It came pre built with some configs which would help us satisfy many of the above features without much extra coding. He added the IEDC MEC logo and gave some touch ups to make everything match nicely.

I put up a message in the IEDC Tech team Whatsapp group, inviting those interested in CSS works to join in and 6 folks signed up pretty soon. (Pretty sure we could've got even more members if it wasn't for the exams coming soon, but the small number turned out to be favorable as recruiting many without ensuring that there were enough tasks for everyone to try out may not have been a great idea.

### The team

So far the blog team consists of 7 members with the team headed by [Amal Dev](https://github.com/amaldevcd) and Alan.

We have 2 second years, 4 first years and one third year excluding me, AmalDev, Allen and Lisa(Tech subhead✨)

Special mention goes to [Jason Dennis](https://github.com/jaison080/) and [Gokulnath](https://github.com/gokz1119/) whose enthusiasm to make PRs and add features to the blog so quickly, surprised me greatly. And boy, was I happy!

You can check out our blog repository [here](https://github.com/IEDCMEC/iedc-blog) to discover the team members.
P.S. We're open to contributions as well :)

### Next Step

Once the team was formed, I made up my mind to ensure that everyone who signed up should be getting atleast one chance to work on the blog. If they were interested and ready, we could find some more tasks for them.

The base version of blog was shown to a few folks outside the blog team and an initial set of feedback was received. Based on this, Alan made a bit more base customizations like adding the dark theme(much requested, yes) feature. (Hey, does Medium have a dark mode? No, only SEO features? okay. Cool)(Sorry, I [don't like](ttps://news.ycombinator.com/item?id=20115037) Medium; can't help taking a dig at it🙈).

Some challenges I faced at this stage was:

1. How to divide and assign features to a team effectively while ensuring that none gets overworked but gets something cool and interesting to try out
2. How to follow up and manage the tasks efficiently.

Amal Dev from Tech Core team had shown interest to help out with the project, even though this was his first time in a managerial kinda role. With short time, we worked up an arrangement between us and tasks were being assigned in an okay manner.

One thing I took great care was that everyone who worked on the blog got sufficient help and mentorship when and if they got stuck with the development works. This wasn't easy as those who could mentor for the blog were just Alan and me.
But again, our team was great and we pulled off implementing features successfully.

## Regarding deployment

The blog is deployed via `github pages`. We've set up a **github action** which runs each time a new Pull Request is merged to main branch to have the blog built to a `gh-pages` branch which automatically gets deployed.

I've added a CNAME record and have it configured in our registrar godaddy.com to have the github pages url point to blog.iedcmec.in (P.S. Thank you [Aadi](https://www.linkedin.com/in/adithyaanilkumar)(IEDC MEC COO) for clearing out the doubt I had with A-records)

We have also added a deploy previews setting using Vercel to get an instant preview url whenever a new pull request is made so that we could review the changes without it being merged to production or having to clone the branch locally to test changes.

## Current status

The blog went through several iterations where it was shared with the Tech team core members who gave some valuable suggestions. It was shown later to [Pranav](https://medium.com/@prnvsan) who talked about several features of Medium. I immediately made up my mind to have atleast some features of it be implemented in our blog as well:)
Finally it was shared to the IEDC Execom for suggestions and feedback.

Boy, we followed Agile. Yes [Razeen](https://www.linkedin.com/in/muhammed-razeen-298815190) (IEDC CEO), you should be proud😁.

Right now the blog is in a state where majority of the suggestions have been addressed and there are a few features on which the blog team members are still working on as I'm writing this.

## Future plans

Initially the Blog workshop using Hugo was conducted just for the tech team members and was not publicized elsewhere as this was the very first workshop by the new Tech team and I wanted to have it run in a small team before opening it up to a very large group.

We now have plans to conduct this workshop at a larger scale and open it up to all MEC-ians who wants to get a taste of blogs and how easy it is to build and create a personal blog to showcase their thoughts and works.

We are also thinking of conducting a workshop on writing with Markdown. The awesome syntax which you might have seen in github readMe or github editor is how each article in the blog is written. Right now, as it's the starting phase, it's good old Amal Dev converting the article in Google Doc to Markdown. We want to change that by introducing Markdown syntax and various Markdown based editors to increase the productivity of budding writers in MEC✨.

## Personal challenges, learnings and afterthoughts

For me personally, this whole endeavour was heartwarming while being stressful at the same time. We managed to pull off the whole blog - right from the planning, training, developing and deployment all within one month and that too in between series and Semester exams!

While I have led technical teams before, never before did I face such a challenge of managing multiple projects running parallelly(MEC Collab coming soon✨) than in this CTO role at IEDC. In between I had to go to Bangalore, meet personal commitments, do my Mom's e-Filing(boy, the time this can take...)

The project taught me that you can't make something great by just telling people to do it. If a project has to be successful, you'd have to put in sufficient efforts from your part. It may not always be easy, but the satisfaction you get at the end is worth it. ✨

I've been fortunate enough to study in MEC where I've seen a lot of talented folks. I've known developers who could read about Hugo and replicate a whole blog like this a few days.
But what I'm proud of right now is the workflow the blog team have set up - No dependence on any single person. Like clockwork (cue Razeen), we now have a system set up to handle new blog articles to be published, or new features to be developed.

Like Napolean Said:

> If you want to go fast, go alone.
>
> If you want to go far, go together

Reminds me of an answer by [Kailash Nadh](http://nadh.in/)(CTO of Zerodha) when I asked him during IndiaFoss (read about IndiaFoss and IEDC [here](https://blog.iedcmec.in/post/indiafoss/)), his thoughts on the challenges of being in a technical leadership position, his answer was something along this: "Being in a technical leadership position is 90% about things other than writing code. Deal with the boring parts as well to be a great technical leader. Be diligent and curious." ✨

P.S. His answer not exactly like this, but what struck my mind was something along these lines. Don't quote me please.

With placements looming overhead, other IEDC projects running parallally, personal commitments and exam pressure, this whole processes of talking up initiative for the Blog project which involves talking to team members, clearing doubts, setting up workflows and a large number of other small small actions were really challenging.

If it wasn't for the constant support of Adithya(Adi) and the dear tech subhead Lisa VC, I'd have probably burnt out earlier. But, with the blog being launched and the with really great positive feedback received, I have to say, there's quite the joy in seeing the team you've brought together and trained, doing something great(Razeen and Adi, if you're reading this, now I know how you guys feel🙂). It fills you with pride and makes your eyes glow with optimism for the future possibilities.

Kudos to the tech team. 🥂

To even more great adventures✨
