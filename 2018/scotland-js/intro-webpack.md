# Title

Introduction to Webpack

# Description

Webpack is a flexible, powerful system for compiling Javascript, but it's also complex and intimidating. In this talk, you'll learn the basics of what Webpack does (and doesn't do), and build a basic Webpack config from scratch. It's not at hard as you think!

# Description

- What is Webpack?
  - JS-to-JS compiler
  - Write code that is well-organized, modular, and maintainable. End up with code that is highly-optimized for the web.
- What does Webpack do?
  - By default, nothing at all
  - Modular, plugin-based system to handle just about any web-related task
  - JS and JS-flavored languages (JSX, TypeScript, Flow, etc)
  - CSS and CSS-flavored languages (Sass, LESS, etc)
  - Image optimiziation
- The simplest Webpack config
  - Pull together Javascript modules into a single file
  - Only includes code that is actually imported
- ES6 & Babel
  - Use the latest Javascript features, target older browsers
  - `babel-loader` library
  - Also works for JSX (for React)
- CSS
  - Import CSS from your JS, dynamically apply styles
  - `css-loader` and `style-loader` libraries
  - Use `extract-text-webpack-plugin` to extract CSS to a separate file
  - Organize your CSS files next to the JS that uses them!
- Images
  - Let Webpack compress images for you, and handle cache URLs
  - `file-loader` library
  - Output files with content hash in name, for long-lived caches
  - Import files from JS!
- Wrap Up & Questions
