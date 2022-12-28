# Class 32
## Intro to Next.js & Tailwind CSS

### Next.js

* When building a React app from scratch there are many things to consider;
  - The code has to be bundled with a bundler like webpack and transformed by a compiler like babel.
  - Production optimizations like code splitting might be necessary.
  - Some pages when pre-rendered staticly might be better for performance and SEO.
  - There might be some server-side code to connect the React app to a data store.
* Using a framework can solve these problems but it must have the right level of abstraction, and it needs to have a good developer experience.
* The React framework of relevance today is Next.js.
* Next.js aims to solve the previous problems as well as having;
  - An intuitive page-based routing system
  - Pre-rendering for both static generation and server-side rendering
  - Automatic code splitting
  - Client-side routing
  - Built in CSS support
  - Development environment with Fast Refresh support
  - API routes for endpoints with serverless functions
  - Extendable

* Next.js is used by thousands of production-facing websites including some of the world's largest brands.
* In Next.js, when navigating between pages, the <a> tag is wrapped in a Link component.
* Next.js code splits automatically, where each page only loads what's necessary for that page.
* Next.js can serve static assets from a top-level directory called public.
* You can also use Third-Party JS with Next.js

### Tailwind CSS

* This approach allows us to implement a completely custom component design without writing a single line of custom CSS.

* Now I know what you’re thinking, “this is an atrocity, what a horrible mess!” and you’re right, it’s kind of ugly. In fact it’s just about impossible to think this is a good idea the first time you see it — you have to actually try it.

* But once you’ve actually built something this way, you’ll quickly notice some really important benefits:

  - You aren’t wasting energy inventing class names. No more adding silly class names like sidebar-inner-wrapper just to be able to style something, and no more agonizing over the perfect abstract name for something that’s really just a flex container.
  - Your CSS stops growing. Using a traditional approach, your CSS files get bigger every time you add a new feature. With utilities, everything is reusable so you rarely need to write new CSS.
  - Making changes feels safer. CSS is global and you never know what you’re breaking when you make a change. Classes in your HTML are local, so you can change them without worrying about something else breaking.
* When you realize how productive you can be working exclusively in HTML with predefined utility classes, working any other way will feel like torture.

* Some synstax:

  - Tailwind’s flexbox and padding utilities (flex, shrink-0, and p-6) to control the overall card layout
The max-width and margin utilities (max-w-sm and mx-auto) to constrain the card width and center it horizontally
  - The background color, border radius, and box-shadow utilities (bg-white, rounded-xl, and shadow-lg) to style the card’s appearance
  - The width and height utilities (w-12 and h-12) to size the logo image
  - The space-between utilities (space-x-4) to handle the spacing between the logo and the text
  - The font size, text color, and font-weight utilities (text-xl, text-black, font-medium, etc.) to style the card text