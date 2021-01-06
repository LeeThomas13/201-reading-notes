[NextJS](https://nextjs.org/learn/basics/create-nextjs-app)

React Nuances:
Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
You need to do production optimizations such as code splitting.
You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
You might have to write some server-side code to connect your React app to your data store.

Next.js provides a solution to all these issues. it inclues intuitive page based routing system, prerendering, static generation and server side rendering, automatic code splitting for faster page loads. client side routing with optimized prefetching, built in CSS support, API routes to build api endpoints with serverless functions, and it is fully extendable.

We recommend using Static Generation (with and without data) whenever possible because your page can be built once and served by CDN, which makes it much faster than having a server render the page on every request.

You can use Static Generation for many types of pages, including:

Marketing pages
Blog posts
E-commerce product listings
Help and documentation

Next.js has two forms of pre-rendering: Static Generation and Server-side Rendering. The difference is in when it generates the HTML for a page.

Static Generation is the pre-rendering method that generates the HTML at build time. The pre-rendered HTML is then reused on each request.
Server-side Rendering is the pre-rendering method that generates the HTML on each request.


[Video: Why I'm Using Next.js in 2020](https://www.youtube.com/watch?v=rtgbaKBhdkk)

Next.js is a framework built on top of react, and it simplifies react. allows either serverside rendering, and clientside rendering on a page by page basis.

performance is cleaner, because it abstracts alot of the performance conundrums away from you.

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)