---
layout: post
title: First steps to a learning analytics experience
date: 2013-04-22
category: libtechnotes
---

Learning Analytics is defined as a “field associated with deciphering trends and patterns from educational big data, or huge sets of student-related data, to further the advancement of a personalized, supportive system of higher education” on the [2013 Horizon Report](http://net.educause.edu/ir/library/pdf/HR2013.pdf).

For this purpose, the [Advanced Distributed Learning Initiative](http://www.adlnet.gov/), best known as the stewards of [SCORM](http://en.wikipedia.org/wiki/Sharable_Content_Object_Reference_Model), have been working on a new specification named the [Experience API](http://experienceapi.com/) to facilitate the recording of all the learning events.

![Tin Can API](http://cdn.tincanapi.com/wp-content/uploads/2012/05/tin-can-api.jpg)

---

[SCORM](http://en.wikipedia.org/wiki/Sharable_Content_Object_Reference_Model) has been the de facto e-learning standard for packaging e-learning content to be delivered to [LMS](http://en.wikipedia.org/wiki/Learning_management_system) but has some drawbacks that the new specification tries to improve. The [Experience API](http://experienceapi.com/) (also known as the Tin Can API) defines a more flexible way to record the learning experiences. That is, taking the elearning out of the browser like on native mobile apps, a solid security using [OAuth](https://en.wikipedia.org/wiki/Oauth) or the ability to track games, simulations or even real world experiences, among other improvements.

This API captures data, in the form of statements, about a person or group’s activities from many technologies. Then a central [Learning Record Store](http://tincanapi.com/learning-record-store/) (LRS) stores learning records from different platforms, and the data stored can be accessed by [LMS](http://en.wikipedia.org/wiki/Learning_management_system), reporting tools, or other LRS to be processed and analysed properly.

Many companies and products, such as [Blackboard](http://www.blackboard.com/) or [Sakai](http://www.sakaiproject.org/), have adopted this de facto standard already. So we’ll have an eye on it.

---

##### About this post

This post was first published on [LibTechNotes](http://labs.biblioteca.uoc.edu/), a blog from the Library team at the [Universitat Oberta de Catalunya](http://www.uoc.edu/) to share our everyday findings, solutions and inspirations.

![by-nc-sa](http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png)