## Basic TailwindCSS setup

[Reference](https://medium.com/@mitchwd/creating-a-project-with-tailwind-123a2960e1fa) Total credits to the author (Mitch)  

1. Create a new project: `mkdir myProject && cd myProject`

2. Initiate the project: yarn init .

3. Install tailwind, postcss (for processing) and autoprefixer (adds vendor prefixes to your code):
```sh
yarn add tailwindcss postcss postcss-cli autoprefixer`  
```

4. Create a tailwind config file (tailwind.config.js): `yarn tailwind init`  

5. Create a postcss.config.js file, and copy the exports from below¹: `touch postcss.config.js`  

6. Create a the tailwind css file & directory, and copy the includes from below²:
```sh
$ mkdir css && touch css/tailwind.css
```

7. Add a build script to package.json: "build": "postcss css/tailwind.css -o public/build/tailwind.css"  

8. Build the files: yarn build  

Create your build/index.html file, and include the built css:

```html
<head>
  <link rel="stylesheet" href="tailwind.css">
</head>
```
