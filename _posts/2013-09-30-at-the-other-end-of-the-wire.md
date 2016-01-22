---
layout: post
title: At the other end of the wire
date: 2013-09-30
category: libtechnotes
---

At the beginnig of the year I was faced with a big challenge. Our team was developing a brand new online classroom, based on the activity rather than on the materials. And we wanted to know from the beginning what was happening inside.

Although the classroom is one of the most important pieces on our learning platform puzzle, there are many satellite applications that also play a role: blogs, microblogs, wikis and forums are just a sample of them. So the reporting system might be distributed, being aware of what is happening in every application or platform. And the learning information should be centralized, in order to analyze the processes wherever they happen.

As I said in a previous post named [First steps to a learning analytics experience](http://labs.biblioteca.uoc.edu/blog/?p=3490), a de facto standard was being developed. [ADL](http://www.adlnet.gov/), the keepers of [SCORM](http://www.adlnet.gov/scorm/) were defining the [Tin Can API](http://scorm.com/tincanoverview/), a next-generation e-learning specification that would allow to gather information from different e-learning platforms to a single [Learning Record Store](http://tincanapi.com/learning-record-store/).

I’ve been implementing a subset of this standard, the [statement](http://tincanapi.com/statements-101/) API, just to report the learning experience inside the classroom. There’s a long way ahead to cover all the contexts where the learning is happening and to make decisons out of the analysis, but we’ve put the first stone.

---

##### About this post

This post was first published on [LibTechNotes](http://labs.biblioteca.uoc.edu/), a blog from the Library team at the [Universitat Oberta de Catalunya](http://www.uoc.edu/) to share our everyday findings, solutions and inspirations.

![by-nc-sa](http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png)