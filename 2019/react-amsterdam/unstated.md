# Title
Taming State with Unstated

# Summary
Managing state with React is deceptively tricky. You can use the built-in `setState()` function, but that doesn't let you keep state outside of a component. You can use Redux, but that quickly becomes a mess of boilerplate code. The [Unstated](http://unstated.io/) library presents a middle path: a way to maintain state outside of components, using a simple, familiar interface that is based on the `setState()` function you already know how to use. In this talk, you'll learn how to use Unstated, and how it can dramatically reduce your Redux boilerplate -- or eliminate it entirely!

# Structure

- Intro [2 min]
  - Who am I?
  - My experience with React
- The Problem [3 min]
  - React apps deal with a lot of state
  - Some state needs to be globally accessible (cached API responses)
  - Some state needs to be locally scoped (components should be separated)
  - How do you manage this?
- The Options [5 min]
  - built-in `setState()`: good for local state, bad for global
  - Redux: powerful and extensible, but often overcomplicated and overused
  - Even the creator of Redux says you probably don't need it! https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367
- Introducing Unstated [10 min]
  - http://unstated.io/
  - A library for using `setState()` to manage global state
  - Based on the React Context API
  - Essentially, allows you to create state containers that your components can subscribe to and update as necessary
  - Show a few examples
  - Using Unstated in lifecycle methods
- When to use Unstated? [5 min]
  - Use local component state when possible
  - Use specialized libraries for specialized state, such as Final Form or Formik for form state
  - Optionally, use the React Context API yourself
  - If none of these work, *then* use Unstated
  - Use the right tool for the job
- Testing with Unstated [5 min]
  - Simpler code means simpler tests
  - Unstated supports dependency injection
  - Testing state containers

# Bio

David "DB" Baumgold is a freelance fullstack web developer who specializes in React on the frontend and Python/Flask on the backend. He's an American who moved to Amsterdam in 2017, and he's found a wonderful developer community in Europe. As an avid contributor to open source, he enjoys teaching and learning, and also does technical training courses for companies interested in leveling up their developers. Find him during the conference if you want to chat about code, community, board games, or abstract philosophy.
  