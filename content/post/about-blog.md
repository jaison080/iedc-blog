---
title: "About this IEDC Blog"
date: 2022-08-13T14:53:07+05:30
Description: "A few thoughts on the technical and non-technical aspects of the IEDC blog by the CTO of IEDCMEC"
Tags: ["tech-team", "behind-the-scenes", "project"]
Categories: []
DisableComments: false
---

## Introduction

The IEDC Blog you are looking at right now is an initiaitve started this year by the tech team of IEDC MEC. This blog lists out the approach we took to build the blog, the features it has and some of the challenges we faced. Read on if you are interested for a behind the scenes overview of the blog project.

- why this blog as a whole
- who's the target audience
- what you can gain from following the blog
- why this article
- what you can gain from reading this

## About the IEDCMEC Blog

The blog idea was something I held very close to my heart after being the CTO of IEDCMEC. Every great organization I knew of had a blog site be it technical or non-technical. The blog is a great medium to showcase the thoughts and literary works of the members of an organization of community.

While most clubs or community depended upon third party blogging platforms like Medium, Blogger, Blogspot etc, IEDC MEC, with it's awesome tech team ))More on the IEDC teams in a later blog) and a firm follower of FOSS technologies, decided to have it built in house by our students ✨.

## Features of the blog

Major features we now have of the blog are:

- Support of both dark and light themes
- Comment feature with github auth for preventing spam
- Clap feature using [applause-button](https://github.com/ColinEberhardt/applause-button)
- Page View Analytics
- RSS Feed support (try adding blog.iedcmec.in/post/index.xml) to your RSS reader ✨
- Emoji support✌️
- Transitions effects and mobile responsiveness
- Extreme customisability

Features for making development easier are added below as well.

<!-- ## How this was made -->

### The planning

#### Technical side:

As CTO, I had the initial say in decisions. I wanted some framework for blogs which didn't involve much learning curve, but also was flexible enough to customize to our needs and easily maintain in the future.

Having had experience with blog frameworks like Gatsby, [Hugo](https://gohugo.io/) etc in the past, I felt like Hugo would be the best of the two which met both the conditions above.

Next step was the training process.

### The training

Majority of the people in the team hadn't heard about Hugo or didn't know why even need to write a blog. So the initial part of the challenge was training and getting them up to speed.

We conducted a workshop on building blogs with Hugo. It was taken by Alan Philipose and me.
Here's the initial blog Alan made as training material, but was immensely useful during the session and even as a reference to the attendees afterwards.

I wanted everyone in the tech team to attend, but due to series exams for first years conflicting and a hackathon by another club in the previous week, we weren't able to bring in the sufficient number of participants as I initially wanted. Ahh the toubles of organizing an event.. Event managers, I feel your pain!🥲

One thing that comforted me was the feeling that those who attended the workshop found it immensely useful. We gave them instructions and the participants (majority of them atleast managed to create a blog and have it depllyed throught github pages by the end of the workshop)!

Afterwards, it was time for recruiting. Alan Philipose built the initial base version of the website by choosing [Anatole](https://github.com/lxndrblz/anatole/) useful.
I put up a message asking those interested in CSS works to join in and 5 folks signed up. (Pretty sure we could've got more members if it wasn't for the exams coming soon, but I initially didn't want to recruit more folks without making sure that there were enough tasks for everyone to try out and get mentorship.

### The team

So far the blog team consists of 7 members with the team headed by @Amal Dev. You can see all the team members here.

## Regarding deployment

The blog is deployed via github pages. I've added a CNAME record and have it configured in our registrar godaddy.com to have the github pages url point to blog.iedcmec.in (P.S. Thank you Adithya for clearing out the doubt I had with A-records)

We have also added a deploy previews setting using Vercel to get an instant preview url whenever a new pull request is made so that we could review the changes before quickly without it being merged to production or having to clone the branch locally.

## Current status

The blog went through several iterations where it was shared with the Tech team core members who gave some valuable suggestions. It was shown later to some folks in the content team and then finally to the IEDC Execom group from there also we received several suggestions. Right now the blog is in a state where majority of the suggestions has been addressed and there are a few features on which the team members are still working on as I'm writing this.

## Future plans

Initially the Blog workshop using Hugo was conducted just for the tech team members and was not publicized elsewhere as this was the first workshop by the new Tech team and I wanted to have it run in a small group before opening it up to a very large group.

We now have plans to conduct this blog workshop at a larger scale and open it up to all MEC-ians who wants to get a taste of blogs and how easy it is to build and create a personal blog to showcase their thoughts and works.

We also have plans to conduct a workshop on writing with Markdown. The awesome syntax which you might have seen in github readMe or github editor is how each blog is written. Right now, as it's the starting phase, it's good old Amal Dev converting the article in Google Doc to Markdown. We want to change that by introducing Markdown syntax and various Markdown based editors to increase the productivity of budding writers in MEC✨.

## Conclusions and personal Afterthoughts

Right now, the blog is set and each member of the team has worked on some feature to make the whole thing great. Plannings for the future sessions have also been going well. Since the blog is pretty stable rn, the members of blog team can easily take up any other projects of the tech team.

## Challenges and afterthoughts

For me personally, this whole endeavour was heartwarming while stressful at the same time. We managed to pull off the whole blog - right from the planning, training, developing and deployment all within one month and that too in between series and Semester exams!

While I have led technical teams before, never before did I receive a challenge of managing multiple projects running parallelly ))MEC Collab coming soon✨).

Reminds me of an answer by Kailash Nadh))CTO of Zerodha) when I asked him during IndiaFoss ))read about IndiaFoss and IEDC here ))) ), his thoughts on being in a technical leadership possition, his answer was this: Being in a technical leadership position is 00% about things other than writing code. Deal with the boring parts as well to be a great CTO. Just be diligent and curious.

Yep, with placements looming overhead, personal commitments and exam pressure, this whole processes of talking to team members, clearing doubts and taking up the blog project forward was really challenging. If it wasn't for the constant support of Adithya and the dear tech subhead Lisa VC, I'd have probably burned out earlier. But, with the blog being launched and the feedback received from the team, I have to say, there's quite the joy in seeing the team you've brought together and trained, doing something great. It fills you with pride and make your eyes glow with the future possibilies.

Kudos to the tech team. 🥂

To even more great adventures✨
