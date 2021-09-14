# React - 3

### Next.j - Assets, Metadata, and CSS

1. Assets
    Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

    The public directory is also useful for robots.txt, Google Site Verification, and any other static assets. Check out the documentation for Static File Serving to learn more.
    * Image Component and Image Optimization
        * Next.js also has support for Image Optimization by default. This allows for resizing, optimizing, and serving images in modern formats like WebP when the browser supports it. This avoids shipping large images to devices with a smaller viewport. It also allows Next.js to automatically adopt future image formats and serve them to browsers that support those formats.

       * Automatic Image Optimization works with any image source. Even if the image is hosted by an external data source, like a CMS, it can still be optimized.
    * Using the Image Component
        * Instead of optimizing images at build time, Next.js optimizes images on-demand, as users request them. Unlike static site generators and static-only solutions, your build times aren't increased, whether shipping 10 images or 10 million images.
2. Metadata
3. CSS Styling.
    * Writing and Importing CSS:
        *Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.

    * Using popular CSS libraries like Tailwind CSS is also supported.


## React context

<br>

### What is React context?
React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

In other words, React context allows us to share data (state) across our components more easily.

<br>

### When should you use React context?
React context is great when you are passing data that can be used in any component in your application.

These types of data include:

Theme data (like dark or light mode)
User data (the currently authenticated user)
Location-specific data (like user language or locale)

<br>

### What problems does React context solve?
React context helps us avoid the problem of props drilling.

Props drilling is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.

Here is an example of props drilling. In this application, we have access to theme data that we want to pass as a prop to all of our app's components.

<br>

### How do I use React context?
Context is an API that is built into React, starting from React version 16.

This means that we can create and use context directly by importing React in any React project.

There are four steps to using React context:

Create context using the createContext method.
Take your created context and wrap the context provider around your component tree.
Put any value you like on your context provider using the value prop.
Read that value within any component by using the context consumer.