My Project
---

Welcome.

Usage
---

Start the development server with this command:

```
npm start
```


Setup
---

```
npm install
```

Compile
---

```
npm run compile
```


_______________________________________________________________________________

http://andrewhfarmer.com/build-your-own-starter/#0-intro

Build Your Own Starter:

      Have you ever been overwhelmed by a React starter project? Too many dependencies that you don't understand?

      Put that all aside. This tutorial will walk you through the process of building your own React starter project... from scratch.

      How it works
      In each step, you'll add one feature or dependency to your starter project.

      When you're done, you'll have a starter project exactly like ahfarmer/minimal-react-starter.

      If you use that starter on future projects, you'll understand every line and be able to easily add additional dependencies.

      Step structure
      Each step has some discussion at the top, and below a list of directions to follow.

      On the right side is the file structure, with a display similar to your IDE. Files that are new for the current step show up in green. Files that have changed are orange.

      Prerequisites
      Before beginning this tutorial, you should have the following:

      Basic knowledge of JavaScript, CSS, and HTML.
      Basic knowledge of the terminal. We'll tell you what to type but you should know how to open your terminal and how to navigate directories within it.
      Node and npm should be installed on your computer.

Git:

      Tracking your work in git is a good habit. git makes it easy to back up your work on a remote server (usually Github). If you make a mistake, you can easily revert your project to a previous step.

      I won't go into the details of git here, but I will show you the git commands you'll need to save your work at the end of each step.

      Every git project should have a README, so we also create the README.md file in this step. The notes you add to your README will be invaluable for reminding you how your project works later on.

      Open up your terminal, run the following commands, and create the following files. Then click Next to move on to the next step.

npm:

      In this step we add a package.json file to record our npm dependencies.

      Everything we add in subsequent steps will be an npm package: Babel, Webpack, React, etc.

      Creating the package.json file is as simple as running the npm init command shown below.

      We also add a .gitignore file in this step. That file only has one line: node_modules. This tells git to ignore the node_modules folder. We don't need to store it in git because it can be auto-generated.

      Notice that the README has changed. Since this is now an npm project, the npm install command can be used to install all dependencies. That's worth noting in the README.

Babel:

      Babel transforms the ES6 JavaScript that we will be writing into ES5 JavaScript that current browsers can understand.

      Babel is particularly important for React developers because of JSX. JSX is a succinct way to write out the layout of a React component.

      To use Babel we need to install Babel itself, as well as two additional packages for configuring Babel for use with ES6, ES7 and React.

      The .babelrc file configures Babel to use the presets that we just installed.

Webpack:

      Webpack bundles all your JavaScript together into a single file. This includes each JavaScript file that you write as well as your npm packages.

      Why Bundle?
      A single .js file is easier to deploy and will usually download faster than multiple small files.

      Webpack will work with Babel to convert your code from ES6/ES7 to ES5 while we work. Webpack can also minify your .js file for production.

      Webpack Config
      The main addition in this step is the webpack.config.js file.

      You will set a few configuration options in this file. Here is the breakdown for each one, along with a link to the relevant portion of the Webpack docs:

      context: This is the path to your client-side JavaScript folder. This must be an absolute path.

      entry: This is the entry point for your application.

      loaders (module.rules): This section specifies how each file should be processed before it is combined into your bundle. We only have one loader: Babel. This converts your ES6 + JSX JavaScript into ES5 before merging it into your bundle.

      resolve: Where Webpack should look for files referenced by an import or require() statement. This makes it so that you can import npm packages in your code.

Compile:

      In the last step you added Webpack, but you didn't actually get to use it yet.

      In this step you'll add an npm script called compile to your package.json. The script runs Webpack.

Express:

      A React development environment needs some way to show your app in a browser. That means you'll need a server. In this step you'll be setting up Express as your server.

      The main file added here is server.js. That file will run an Express server, which will run Webpack. Webpack will re-run any time you change one of your JavaScript files.

      server.js is server-side JavaScript. You can run it with the node server.js command. In this step you will also add a start script to run the server.

      You will create www/index.html as your first web page. Express is configured to serve all the files in that folder.

React:  

      In this step you'll add the React npm package and one simple component.

Review:

      Hurray! Here's what you've accomplished:

      You learned how to integrate multiple tools together.
      You put together a starter project, from scratch.
      You now have a starter project that you can use on future projects.
      Next time you start a project, use ahfarmer/minimal-react-starter. It is exactly like the starter project you just built, so you understand every single line.

      What can I do with it?
      You can build a full-fledged React project with just these tools.

      Then next step is to start writing React components.

      If you are still learning, I strongly encourage you to start your project with a minimal starter like this one.

      Even if your project requires more tools, try to build the first few React components simply. Use hard-coded data if you have to. Skip Flux at the beginning. This way you will make progress towards your goal without overwhelm.

      What's missing?
      A bunch of stuff you may or may not need:

      CSS processor(s)
      HMR / Auto Reload
      Routing
      Flux/Redux/MobX
      Server-side rendering
      Database
      AJAX / Networking
