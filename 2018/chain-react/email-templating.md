# Title

Sending Email with React

# Short Summary

Rendering templates is slow, and sending transactional email means rendering a LOT of templates. Instead, we built a system to handle rendering and sending email templates using AWS Lambda and server-side React. Now, our backend can simply call an API, and let Lambda handle the complicated part.
Check out how we did it, and how you can offload expensive rendering processes
to Lambda as well.

# Talk description and abstracts

- The Problem
  - Rendering HTML is slow
  - Backend was taking too long, causing delays in processing jobs
  - Expensive AWS bills
- The Solution
  - AWS Lambda!
  - Perfect for running short tasks, infinitely scalable, cheap
  - React for rendering HTML: that's what it does best
- Implementation
  - One Lambda function per template: one for invitation emails, one for
    reminder emails, one for confirmation emails, etc
  - Used react-html-email for HTML templates, ES6 template strings for text
    templates
  - Used Apex for deployment onto Lambda (bonus: continuous deployment
    via CircleCI!)
  - Backend calls Lambda via Ruby AWS gem
- Problems
  - Mismatched interfaces. We accidentally merged changes to our
    email templating system that changed the API, without corresponding
    changes to how the backend *called* the API
  - Timeouts on Lambda (5 sec maximum)
  - Finding the right number of emails to send in one Lambda function
  - Monitoring and reporting errors correctly
- Wins
  - Backend load went down
  - Non-developers were able to make pull requests to change the text of our
    emails. Much more readable code!
  - Automated tests
  - Date/time localization, using react-intl
  - Validation for HTML email client support, using react-html-email
- Future Plans
  - Rendering PDFs using headless Chrome
  - Open source codebase
- Questions?

# Previous talks

- DjangoCon 2017: Django vs Flask
  - Video: https://youtu.be/UY2JMZjQspY
  - Slides: https://archive.org/details/djangocon-us-2017-django-vs-flask
- PyCon 2017: Looping Like a Pro in Python
  - Video: https://youtu.be/u8g9scXeAcI
  - Slides: https://archive.org/details/pycon-2017-looping
- PyDX 2016: Advanced Git
  - Video: https://youtu.be/ZdIuFuIM3dM
  - Slides: https://archive.org/details/AdvancedGit
- PyGotham 2016: Advanced Git
  - no video available
  - Slides: https://speakerdeck.com/singingwolfboy/advanced-git-2
- PyCon 2016: Prototyping APIs in Flask
  - Video: https://youtu.be/6RdZNiyISVU
  - Slides: https://speakerdeck.com/singingwolfboy/prototyping-apis-with-flask
- PyCon 2016: Get Started with Git
  - Video: https://youtu.be/Qthor07loHM
  - Slides: https://speakerdeck.com/singingwolfboy/get-started-with-git
- PyCon 2015: Advanced Git
  - Video: https://youtu.be/4EOZvow1mk4
  - Slides: https://speakerdeck.com/singingwolfboy/advanced-git

# Country and City

Amsterdam, Netherlands

# Picture of me

https://www.davidbaumgold.com/static/images/headshot.jpg

# Bio

David Baumgold is a senior web developer specializing in React and Python.
He is an avid contributor to open source software, and he enjoys travel,
teaching, learning, and working together with others. He currently lives
in Amsterdam and works for Impraise.


