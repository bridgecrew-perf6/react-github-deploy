1. Install `gh-pages`
- This package helps us to deploy code to gh-pages branch, which will host our app in Github Pages.
```sh
➜  react-github-deploy git:(master) npm install gh-pages --save
```

2. Add Two Keys to `package.json`
```sh
"scripts": {
    "start": "DEFAULT SET",
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
    "build": "DEFAULT SET",
    "test": "DEFAULT SET",
    "eject": "DEFAULT SET"
  },
  ```

  3. Add `homepage` key to `package.json`
  - React uses it figure out root url in the built in html file.
  ```sh
  {
  "name": "react-github-deploy",
  "homepage": "https://singh-sumit.github.io/react-github-deploy",
  "version": "0.1.0",
  "private": true,
  /...
  }
  ```