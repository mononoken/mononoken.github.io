---
layout: project
title: "Fae Scribe"
description: A note taking app for tabletop RPG players. Built using Ruby on Rails.
url: https://github.com/mononoken/fae-scribe
order: 1
---

This app was created as an alternative to [The Odin Project's Rails final project, building a Facebook clone](https://www.theodinproject.com/lessons/ruby-on-rails-rails-final-project). The note creation system behaviors similarly to the postings for a social media site.

Notes are input using Markdown syntax and rendered as HTML. The [Redcarpet](https://github.com/vmg/redcarpet) gem was utilized for this functionality, and I wrote some extensions to the renderer to allow for more custom syntax conversions.

Much of this site was designed using BDD (behavior-driven development) methodologies. I created a user flow diagram to start. I used Github issues to organize what features and improvements I would want to add throughout the project. When a new feature was being tackled in an issue, I would typically start with writing system tests for the feature using RSpec and Capybara with a selenium webdriver. Unit test and integration tests would also be created as needed until the feature was fully implemented and all tests passed. This project has had over 80% test coverage as reported by Simplecov throughout its progress so far.

This project also included many other learning opportunities. I implemented Websocket connections for the note pages and comments. This project was also the first project where I used Tailwind for styling.
