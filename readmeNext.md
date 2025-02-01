# Next.js
## What is Next.js?

Next.js is a React framework that enables server-side rendering, static site generation, and routing. It simplifies building React applications with optimized performance.

## What is SSR (Server-Side Rendering) in Next.js?

SSR allows rendering React components on the server rather than in the browser, improving initial load performance and SEO.

## What is SSG (Static Site Generation) in Next.js?

SSG allows pages to be pre-rendered at build time and served as static HTML files. It’s ideal for static content that doesn’t change often.

## What is ISR (Incremental Static Regeneration) in Next.js?

ISR allows static pages to be re-rendered after deployment without rebuilding the entire site, enabling pages to be updated after a set time interval.

## How do you create dynamic routes in Next.js?

You can create dynamic routes by using square brackets in the file name, e.g., pages/[id].js.

## What is the getServerSideProps function?

getServerSideProps is used to fetch data server-side on each request, enabling server-side rendering for a page.

## What is the getStaticProps function?

getStaticProps is used to fetch data at build time for static site generation.

## What is getStaticPaths in Next.js?

getStaticPaths is used alongside getStaticProps to specify dynamic routes that should be pre-rendered at build time.

## How do you handle routing in Next.js?

Next.js uses a file-based routing system. Pages are created in the pages directory, and each file corresponds to a route in the application.

## What is the useRouter hook in Next.js?

useRouter is a React hook that gives access to the Next.js router object, which can be used to navigate programmatically, access the current route, etc.

## What is the Link component in Next.js?

The Link component is used to enable client-side navigation between pages in Next.js without full page reloads.

## What is the Head component in Next.js?

The Head component allows you to modify the <head> section of the HTML document (e.g., to add meta tags, titles, or links to external resources).

## How do you implement API routes in Next.js?

API routes can be implemented in the pages/api directory. Each file in this directory is treated as an API endpoint.

## What is automatic static optimization in Next.js?

Next.js automatically optimizes pages by statically rendering them if no blocking data fetching methods (like getServerSideProps) are used.

## What is the default method for data fetching in Next.js?

The default method is static site generation (SSG) using getStaticProps.

## What is the next/image component used for?

next/image is an image optimization component that automatically optimizes images for performance (e.g., lazy loading and resizing).

## What is the next/head component?

The next/head component is used to add elements to the <head> section of the HTML document (e.g., for SEO purposes, or setting the document title).

## What is next/link used for in Next.js?

next/link is used to create client-side navigation links between pages in a Next.js application.

## How do you manage global styles in Next.js?

Global styles can be managed by importing a CSS file in the _app.js file.

## What is next/export used for in Next.js?

next export is used to export a Next.js app as a static site, generating static HTML files that can be deployed to any static file server.

