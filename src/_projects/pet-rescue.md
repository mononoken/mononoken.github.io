---
layout: project
title: "Pet Rescue"
description: An open-source project for linking adopters with pets. Built using Ruby on Rails.
url: https://github.com/rubyforgood/pet-rescue
order: 1
---

I joined this project in January 2024. After working on a few issues, I noticed the authorization throughout the application was inconsistent and even missing in some areas. I volunteered to implement an authorization framework for the entire app to address these issues.

The resulting work took a little over a month and can be found in this PR [Authorization framework with Action Policy #466](https://github.com/rubyforgood/pet-rescue/pull/466).

I opted to use [Action Policy](https://actionpolicy.evilmartians.io/#/) for the framework after enjoying using it for other personal projects. I created policy classes for every controller that existed in the app up to this point. This involved having to quickly onboard myself to the codebase to figure out what kind of permissions were necessary for every controller action.

I wrote unit tests for every policy class created and also created tests for the controllers to make sure they utilized these policy objects properly. Rather than write integration tests for every different possible user context, I tested the user context's in the speedy unit tests and then simply tested the controller called the correct policy check in the controller action.

After working on the app significantly, I was asked to join the project as a collaborator and member of the lead team to further help the project. I am continuing to work with the rubyforgood/pet-rescue team and having lots of fun doing so!
