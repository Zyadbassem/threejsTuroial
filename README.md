# Three.js Tutorial

Hey there, my name is Zyad, and I'm starting to learn Three.js! I thought it would be a great idea to share my learning journey. I'm using the official Three.js documentation.

## First Lesson

In this lesson, we're going to go step by step through the installation of Three.js and starting a project.

- Create a folder called `threejsTutorial` (or whatever you like).
- In that folder, create two files:
  1. `index.html`
  2. `main.js`
  
- Copy and paste this code in the `index.html` file:

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>My first three.js app</title>
      <style>
        body { margin: 0; }
      </style>
      <script type="importmap">
        {
          "imports": {
            "three": "https://cdn.jsdelivr.net/npm/three@v0.149.0/build/three.module.js",
            "three/addons/": "https://cdn.jsdelivr.net/npm/three@v0.149.0/examples/jsm/"
          }
        }
      </script>
    </head>
    <body>
      <script type="module" src="/main.js"></script>
    </body>
  </html>
- copy and paste this code into `main.js` 
    ``` js
    import * as THREE from 'three';
    import { OrbitControls } from 'three/addons/controls/OrbitControls.js';
    import { GLTFLoader } from 'three/addons/loaders/GLTFLoader.js';

    const controls = new OrbitControls( camera, renderer.domElement );
    const loader = new GLTFLoader();  
### download the required libraries 
- open your terminal in the main directory of your project copy and paste these commands

```
npm init
npm install --save three
npm install --save-dev vite
npx vite
npx vite build
npx serve .
```
now you should see in your terminal a link `http://localhost`
with this we're done with our first lesson