# Flowmazon E-Commerce App

## Description

I built this app following the excellent [Next.js E-Commerce Tutorial from freeCodeCamp](https://www.youtube.com/watch?v=K4ziF0MhbLc&t=15076s). I followed this tutorial in order to learn to use TypeScript, as well as to build my knowledge of server components in Next.js. Although the vast majority of this project was built by coding along with the tutorial, I still needed to troubleshoot and debug certain issues.

## Key Learning

This app has given me a much greater understanding of TypeScript, particularly using Interfaces to specify the types of props in React/Next.js components. Going into this project, I was fairly unclear on the benefits of TypeScript, however I have come to really appreciate the autocomplete and error handling it provides.

I had not used Prisma before, previously using Mongoose to interface with MongoDB. I like the way that it handles foreign keys and enables easier updating of related models, as well as its very clean layout of schemas.

I was also particularly impressed with the way server components and client components are very carefully utilised in this project, to take advantage of Next.js's caching features. I had tried to use this in a previous project, Venturo, and found it quite challenging to understand how client components could interact with server components, and how to manage user interactivity within server components.

I also like how this project uses url parameters to handle state with search queries and pagination. This is not something that had previously occurred to me and is something that I intend to take forward in future projects of my own.

## Challenges

The main challenge that I encountered with this project was implementing Next-Auth. The tutorial suggested exporting the ``authOptions`` object in the Next-Auth route.ts file, to ensure that these could be used in other components. However, this is no longer possible and TypeScript threw an error at build time saying that this was not a valid object to export. I got around this by creating a separate ``authOptions`` library, exporting the object from there, and importing it into the route.ts file instead.
