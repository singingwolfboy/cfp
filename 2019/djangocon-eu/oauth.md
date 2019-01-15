# Title

Taming OAuth

# Abstract

This talk is about OAuth: how it works, why it's so complicated,
and how to use it effectively with Django and/or Flask.

# Description

In this talk, I'll go over the basics of OAuth: what it is, how to use it,
and why developers should care. (Developers should care about OAuth because
they need it if they want to use APIs from Google, Twitter, Facebook, GitHub,
and hundreds of other API providers.)

I'll also go over how to use OAuth in Django, using the popular
`python-social-auth` package. If there's time, I will deploy a
pre-written Django application that uses `python-social-auth`,
set up OAuth keys, and show that application can authorize against
an OAuth-protected API.

# Outline

- Introduction [5 min]
  - Who am I?
  - Experienced software developer
  - Many years building webapps
- What is OAuth? [5 min]
  - A system that allows users to grant third-party applications access to
    their user data on a website
  - Involves three different parties: user, provider, consumer
  - Securely communicating between these parties makes the protocol difficult
    to understand
- Intro to Python Social Auth [5 min]
  - A pluggable library that allows you to write simple OAuth consumer apps
  - Works with Django, as well as other Python web frameworks
  - Simple to get started, powerful and flexible to allow advanced use-cases
- Deploying a simple OAuth app [15 min]
  - Walk through the code for a pre-written Django app that uses OAuth
  - Get API tokens and put them into place
  - Verify that it works correctly
  - If live-deploy fails, show a video of the process completing successfully instead
- Questions?

# Additional Notes

I am an accomplished speaker at technical conferences. Here is a summary of the presentations I've done before: https://www.davidbaumgold.com/presentations/

I am the author of Flask-Dance, which is a similar library for OAuth
support with Flask. I am happy to make this talk about Flask-Dance
instead of Python Social Auth, or compare to the two during the talk,
but since this is Djangocon, I figured the audience would be more
interested in solutions that work with Django.
