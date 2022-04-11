# Building blocks of a web application

1. **User Interface** - how users will consume and interact with your application

2. **Routing** - how users navigate between different parts of your application

3. **Data Fetching** - where your data lives and how to get it

4. **Rendering** - when and wehre you render static or dynamic content.

5. **Integrations** - what third-party services you use (CMS, auth, payments, etc) and how you connect to them.

6. **Infrastructure** - where you deploy, store, and run your application code(Serverless, CDN, Edge, etc).

7. **Performance** - how to optimize your application for end-users.

8. **Scalability** - how your application adapts as your team, data and traffic grow.

9. **Developer Experience** - your team's experience building and maintaining your application.

For each part of your application, you will need to decide whether you will build a solution yourself or use other tools such as libraries and frameworks.

Part of React's success is that it is relatively unopinionated about the other aspects of building applications. This has resulted in a flourishing ecosystem of 3rd party tools and solutions.

As a result, developers need to spend time configuring tools and reinventing solutions for common application requirements.

Next.js is a React framework that handles the tooling and configuration needed for React, and provides additional structure, features, and optimizations for your application.

# Different stages

1. The environment where your code runs: Development vs Production.

2. When your code runs: Build Time vs Runtime

3. Where rendering happens: Client vs Server

# Setup

> package.json
> {

}

npm install react react-dom next

# How Next.js works

1. **From Development to Production** - Development is optimized for dev and their experience building the application. It allows you to use Typescript, ESLint, Fast Refresh and more. In production, it is optimized for end-users and their experience using the application. It aims to transform the code to make it performant and accessible.

2. **Compiling** - taking code in one language and outputting it in another language or another version of that language. In this case, modern versions of JS need to be compiled into JS before browsers can understand them.

3. **Minifying** - removes comments, spaces, multiple lines, indents. Improve the app performance by decreasing file sizes.

4. **Bundling** - Dev break up app into modules, components and functions. Exporting and importing these internal modules, as well as external 3rd party packages create a complex web of file dependencies. This is the process of resolving the web of dependencies and merging(or packaging) the files (or modules) into optimized bundles for the browser with the goal of reducing the number of requests for files when user visits a web page.

5. **Code Splitting** - Devs usually split their applications into multiple pages that can be accessed from different URLs. Each of these pages become a unique entry point into the application. This is the process of splitting the application's bundle into smaller chunks required by each entry point. The goal is to improve the application's initial load time by only loading the code required to run that page. Each file inside your pages directory will be automatically code split into its own Js bundle during build step. Any code shared between pages is alos split into another bundle to avoid re-downloading the same code on further navigation.

6. **Build Time vs Runtime** - transforms your code into production-optimized files. Runtime refers to request-time, time when your application runs in response to a user's request.
