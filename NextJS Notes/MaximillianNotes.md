# React Refresher

- What is React ?
  - React is a JS Library for building User Interfaces
    - Client Side JS Library
    - To build modern, reactive UI
- Angular and Vue.js are alternatives

## Create a new React Application
- `npx create-react-app application-name`
- `package.json` contains all the dependencies of the project

# What is NextJS ?

- The React Framework for Production
- NextJS solves common problems 

# Key features of NextJS

- Server Side Rendering
  - Render content in server instead of at client
  - Useful for SEO Optimization and initial load
- File-based routing
  - Define routes from files and folders
  - Less managed routes in code
  - Nested routes supported
- Fullstack capabilities
  - Easily add backend code to Next /React apps

# Create the NextJS Application

- In the terminal run `npx create-next-app`
  - Interactive way to create a new NextJS Application
- `npm install` to install all the dependencies required
- `npm run dev` to run the project


# Folder Structure of the created project

- styles 
- public
  - contains publically accessible resources by the application
- pages 


# File-based routing
- Under the pages directory we can create folders which act as routes
- the `index.js` is a file which acts as a base file to be rendered when we hit that url endpoint
- `[id].js` acts as file which is dynamic parameter like an id for thet route
- In the component `import {userouter} from next/router` i.e the `useRouter()` hook gives access to the slug using `router.query`
- `[...slug].js` catches all the routes as array of strings
- To link to another page
  - `import Link from "next/link"`
  - `<Link href='/blog/100'>Blog</Link>`
  - Alternative way :
    - `<Link href={{pathname:"/blog/[id]", query:{id:100}}}>`
- Programatically navigate to another link
  - `const router = useRouter()`
  - `router.push('/blog/2023/01')`
    - we can go back in the navigation 
  - `router.replace('/blog/2023/01')`
    - we cannot go back in navigation
- 404 Page
  - In root level of `pages` folder create a `404.js` file





