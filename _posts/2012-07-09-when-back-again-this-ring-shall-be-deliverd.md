---
layout: post
title: When back again this ring shall be deliver'd
date: 2012-07-09
category: libtechnotes
---

[![](http://imgs.xkcd.com/comics/compiling.png)](http://xkcd.com/303/)

One of the typical scenarios in many [Drupal](http://drupal.org/) projects is to have a production, a staging, an integration and a development environment. When our site is in production, users create a lot of content everyday, while additional features (as content types, fields and others) and [modules](http://drupal.org/project/Modules) are being added to the site in the development environment. As in Drupal configuration and modules are stored in the same database as content data, when it comes the day to move the upgraded site to production, the upgraded site is out of synch with user data in production.

This is known as the [Drupal staging problem](http://dominiquedecooman.com/blog/drupal-staging-problem), and there’s no magic solution for this. Every approach to the solution passes through capturing every development change from the database into code. Some tools can make our life a little bit easier to help tracking the changes and automating the deployment. With the following bunch of tools, at any point we can virtually [rebuild a fully functional site](http://wiredcraft.com/blog/drush-make-and-install-profiles-drupal-7) by simply using an installer script.

> 
> A working software application can be usefully decomposed into four components: executable code, configuration, host environment and data.
> 
> 
> 
> _Jezz Humble, David Farley in Contiunous Delivery_
> 
> 

**Features**

[Features](http://drupal.org/project/features) is a module that allows us to export data structures deep in the database into code. It not only aisles the changes implemented in our development environment but also allows us to use version control tools to track the changes. A feature is defined as a collection of Drupal entities which taken together satisfy a certain use-case.

** Drush**

[Drush](http://drupal.org/project/drush) is a command line shell and scripting interface for Drupal. It allows to script many actions that would normally be done on the administration interface, such as installing Drupal and modules, and updating the configuration. Using some of the [core Drush commands](http://drush.ws/) avoids many clicks and helps to automate tasks, including the deployment of the application.

**Drush make**

[Drush make](http://drupal.org/project/drush_make) is an extension to drush that can create a ready-to-use drupal site, pulling sources from various locations. It does this by parsing a flat text file (similar to a drupal .info file) and downloading the sources it describes. In practical terms, this means that it is possible to distribute a complicated Drupal distribution as a single text file.  There's some tools to help making this make file, like [Drush make generator](http://drushmake.me/).

**Feeds**

On creating content automatically, this module imports or aggregates data as nodes, users, taxonomy terms or simple database records from RSS, Atom or CSV [feeds](http://drupal.org/project/feeds/). This is a way to import the data of a production site to another with new features.

**Profiler**

Finally this [profiler](http://drupal.org/project/profiler/) module is used to tell Drupal how to install things up, what modules to enable, or what values to apply to settings.

This is only one of the solutions, among [many](http://www.slideshare.net/libsys/drupalcamp-12987192) [others](http://www.slideshare.net/eaton/drupal-deployment-presentation), to make Drupal development and deploy less confusing.

---

##### About this post

This post was first published on [LibTechNotes](http://labs.biblioteca.uoc.edu/), a blog from the Library team at the [Universitat Oberta de Catalunya](http://www.uoc.edu/) to share our everyday findings, solutions and inspirations.

![by-nc-sa](http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png)