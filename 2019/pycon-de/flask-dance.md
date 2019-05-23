# Title

Taming OAuth with Flask-Dance

# Abstract

Learn how OAuth works, and how to use it to access popular APIs. We'll also use the Flask-Dance library to write a demo app that can authenticate with OAuth-protected APIs.

# Abstract as Tweet
OAuth is hard. Learn how it works, and how to make it easy with Flask-Dance!

# Description

Many well-known APIs use OAuth for authentication, including Google, Facebook,
Twitter, and GitHub. OAuth is a notoriously complicated protocol, but you
can't use any of these APIs without it.

In this talk, we'll learn how OAuth works and why it's so complicated.
We'll also use the Flask-Dance library to write a demo application that
can authenticate with an API via OAuth. By the end, you'll be ready to
use any OAuth API you want, and debug authentication failures as well.

# Notes

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
- Intro to Flask-Dance [5 min]
  - A Flask extension that allows you to write simple OAuth consumer apps
  - Simple to get started, powerful and flexible to allow advanced use-cases
- Deploying a simple OAuth app [10 min]
  - https://github.com/singingwolfboy/flask-dance-github
  - Uses the GitHub API, deployed using Heroku
  - Walk through the code
  - Get API tokens and put them into place
  - Verify that it works correctly
  - If live-deploy fails, show a video of the process completing successfully instead
- Diagnosing common OAuth errors [5 min]
  - Authorized redirect URIs
  - Scopes
  - Correctly identifying users
- Questions?

Note: I considered doing a "live-coding" section of the talk, but in my experience, live-coding is almost never a good idea: too many things could go wrong. Instead, this talk has a "live deploy" section -- the code is already written, and all I have to do is walk the audience through how the code works in theory, and then deploy it and show that it works in practice. Still very impressive, but much less error-prone.


# Additional Notes

I am an accomplished speaker at technical conferences. Here is a summary of the presentations I've done before: https://www.davidbaumgold.com/presentations/

I am the author of Flask-Dance, and I have been building and maintaining the
library since 2014.
