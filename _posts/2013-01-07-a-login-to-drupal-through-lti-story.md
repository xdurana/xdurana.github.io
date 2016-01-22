---
layout: post
title: A login to Drupal through LTI story
date: 2013-01-07
category: libtechnotes
---

We are developing our new library website in [Drupal](http://drupal.org/) and we need to allow our users to log in through their Campus username and password. Our [Drupal](http://drupal.org/) installation has no loaded information about our users, so it will rely on the user data that Campus application (our [LMS](http://en.wikipedia.org/wiki/Learning_management_system)) gives to it. First of all, an user will log in the Campus application and then the user data will be passed to [Drupal](http://drupal.org/) through an [LTI](http://developers.imsglobal.org/) call. Here's the tutorials on [how LTI tools work](http://developers.imsglobal.org/tutorials.html).

> Learning Tools Interoperability ([LTI](http://developers.imsglobal.org/))™ is a specification developed by [IMS Global Learning Consortium.](http://www.imsglobal.org/) The principal concept of [LTI](http://developers.imsglobal.org/) is to establish a standard way of integrating rich learning applications (often remotely hosted and provided through third-party services) with platforms like learning management systems, portals, or other educational environments.

For this purpouse we have been developing a [Drupal](http://drupal.org/) module for log in through [LTI](http://developers.imsglobal.org/) by adapting a [basic LTI tool provider](http://developers.imsglobal.org/phpcode.html). The basic flow of this Basic [LTI](http://developers.imsglobal.org/) module is that the [LMS](http://en.wikipedia.org/wiki/Learning_management_system) launches the tool with a number of POST parameters that are signed [OAuth](http://oauth.net/) with a secret shared by both the [LMS](http://en.wikipedia.org/wiki/Learning_management_system) and the LTI module. When the LTI module receives the user data in form of POST parameters, it logs in the Drupal user with its username, previously creating a new Drupal user if it doesn't exist yet. As the library website user roles are different from that in the Campus, a role mapping is previously made through a conversion table.

This is an [example of a LTI consumer](http://www.imsglobal.org/developers/LTI/test/v1p1/lms.php) we have been using to perform our initial tests to our [Drupal](http://drupal.org/) module.

UOC has contributed with some tools to the [catalog](http://developers.imsglobal.org/catalog.html) of LTI tools certified by [IMS Global](http://www.imsglobal.org/), and some of them are available on the [Learning Apps store](http://www.learningappsstore.org/).

---

##### About this post

This post was first published on [LibTechNotes](http://labs.biblioteca.uoc.edu/), a blog from the Library team at the [Universitat Oberta de Catalunya](http://www.uoc.edu/) to share our everyday findings, solutions and inspirations.

![by-nc-sa](http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png)