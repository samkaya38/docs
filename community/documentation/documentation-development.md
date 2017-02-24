---
title: "Documentation Development"
space: "Community"
category: "Documentation"
---

## 1 Introduction

<div class="alert alert-info">

The information provided here is in development and can change over time.

</div>

The documentation we provide is created using what is called a static page generator. The source code of this project can be found on [Github](http://github.com/mendix/docs) and automatically build. This document provides information about the techniques behind the documentation.

## 2 Techniques

### 2.1 Static page generator

Mendix Documentation runs on [Jekyll](http://jekyllrb.com). This is a static page generator build on top of Ruby. Such generators use templates, combined with content, to generate a static HTML website. In our project we use Jekyll to generate the pages, the sitemap and JSON files for the menu. The menu is eventually generated client-side using Javascript

### 2.2 Gulp

To automate the development, we use [Gulp](http://gulpjs.com/). Gulp is a task-runner, built on top of Node.js.

## 3 Running documentation locally

### 3.1 Prerequisites

To run the documentation, you will need to have the following things installed:

  * Ruby & rubygems
    * This is needed to install [Bundler](http://bundler.io/)
  * [Node.js](https://nodejs.org/en/)
    * Install Gulp client in your terminal: `npm install gulp-cli -g`

### 3.2 Setup

 * Download or checkout the repository
 * Open a terminal and run the following commands:
  * `bundle install`, this will install Jekyll and other dependencies
  * `npm install`, this will install all the Gulp dependencies

### 3.3 Running it locally

Run `gulp help`
