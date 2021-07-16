<h2>An introduction to the npm package manager</h1>


TABLE OF CONTENTS
Introduction to npm
npm is the standard package manager for Node.js.

In January 2017 over 350000 packages were reported being listed in the npm registry, making it the biggest single language code repository on Earth, and you can be sure there is a package for (almost!) everything.

It started as a way to download and manage dependencies of Node.js packages, but it has since become a tool used also in frontend JavaScript.

There are many things that npm does.

Yarn and pnpm are alternatives to npm cli. You can check them out as well.

Downloads
npm manages downloads of dependencies of your project.

Installing all dependencies
If a project has a package.json file, by running

-->npm install
it will install everything the project needs, in the node_modules folder, creating it if it's not existing already.

Installing a single package
You can also install a specific package by running

-->npm install <package-name>
Often you'll see more flags added to this command:

--save installs and adds the entry to the package.json file dependencies
--save-dev installs and adds the entry to the package.json file devDependencies
The difference is mainly that devDependencies are usually development tools, like a testing library, while dependencies are bundled with the app in production.