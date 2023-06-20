# Scrollable 3D Animation with Three.js

- Watch the [full tutorial](https://youtu.be/Q7AOvWpIVHU) on YouTube
- [Scrollable Three.js Animation](https://fireship.io/snippets/threejs-scrollbar-animation) Snippet

## Usage

```bash
git clone this-repo
yarn install
yarn run dev
```

## CI/CD

This project runs on the GitHub Pages [using gh-pages JS lib](https://yarnpkg.com/package/gh-pages) to keep it simple to use.

After installing the lib with
```bash
yarn install 
```
go to your `package.json` file and paste this inside you `scripts` key

```json
"scripts": {
    "dev": "vite code_folder/",
    "build": "vite build code_folder/",
    "serve": "vite preview code_folder/", //<< don't forget the comma ','
    "deploy": "gh-pages -d code_folder/" //<< paste this line and use the folder in which your code is in, if it's on the root folder your in, just use '.' as your folder name
  }
```

When deploying your project, you must run:

```bash
yarn run build
yarn run deploy
```

[Here you find more information on how to configure it correctly](https://github.com/tschaub/gh-pages)

## References
~~As we need to be up on the shoulder of giants, we need to give them their credits, right?~~ :thinking:

[Book "Discover Three.js" with a great step by step developing of a great scene with a good code design to keep all of your code universe(sorry for that) under control.](https://discoverthreejs.com/book/first-steps/animation-system/)

[Markdown documentation, used to know how to produce HTML code blocks equivalent to what we have on Markdown but without the Markdown interpreter](https://daringfireball.net/projects/markdown/syntax#precode)
