# npm

- It does not stand for Node Package Manager.
- It is a repository for all packages.

# package.json

- It is a configuration file for our npm repository.
- It keeps track on version of every package present inside the app.
- It keeps the approx version of the package, that's why it contains ~ and ^.

# Dependencies

- There are two types of dependencies, dev dependencies and normal dependencies.
- Dev dependency is required in development phase.
- Normal dependency is also used in production phase.

# Caret (^) and Tilde (~)

- It is present before version of any package in package.json.
- Bundler automatically updates the version in which there is a very minor update in case of ^.
- Bundler automatically updates the version in which there is a major update in case of ~.
- It's always better to upgrade the minor versions than major versions as it can break the code.

# package-lock.json

- It keeps the track of exact version of ther dependency.
- It does not contain ~ and ^.
- It contain information of packages, and contains one key called integrity.
- Integrity contains hash code which is unique, and it should match development mode with production mode, otherwise the code can break.
- It keeps track of all transitive dependency versions.

# node_modules

- It contains code which is present inside npm.
- It contains all the packages which are required to run the app.
- It is like a DB which contains all the code required for our app.

# Transitive dependency

- It is a dependency which is dependent on other dependencies for it's working.
- It creates a dependency tree that's why node_modules is bulky.

# npm vs npx

- npm is used to install, delete and update packages.
- npx is used to execute a package.

# cdn link vs npm package

- CDN links are costly because we have to make a network call to a remote server to fetch a package.
- When we install any pacakge using npm, we already have that package in our node_modules, which is easier to use.
- If any version upgrade happens in our package, we have to change the CDN url.
- Whereas, package.json takes care of the version upgrade in case of npm.

# Module Bundler (Webpack, Parcel, Vite, Vercel, Rollup, Browserify)

- It creates a dev build for our app.
- It hosts our app on a local server.
- HMR (Hot Module Replacement) - When you make a change, it automatically updates your code in the browser, no page reload necessary.
- HMR is implemented using File Watching Algorithm which is written in C++.
- Caching - It gives you faster builds because of caching.
- Image Optimization - The most expensive operation is to load an image on a website and module bundler do image optimization.
- Minification - For production build, it will minify all the file code.
- Bundling - It will make bundles of similar files to reduce the folder size.
- Compressing - It reduces the size of the application for production environment.
- Differential Bundling - It makes the app compatible with every browswer, even older browsers as well.
- Code Splitting - It can create multiple bundles that can be dynamically loaded at runtime.
- Error Handling - It does the diagnostics of the app, and provides readable and understable error suggestions when encountered.
- It can convert HTTP to HTTPs when SSL configuration is enabled.
- Tree shaking - It will remove or ignore unused code from your app.
- It creates different builds and bundles for dev and production.
