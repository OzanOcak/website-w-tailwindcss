```console
npx tailwindcss init
mkdir build src
touch build/index.html src/input.css
```

initializing tailwindcss npm package will create tailwind.config.js file, we need to
**'./build/\*.html'** in content key of object

````javascript
module.exports = {
  content: [],
  theme: {
    extend: {},
  },
  plugins: [],
};
```
input.css

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
````

- go setting , type full reload and check Live server to be able to use it
- install inline-fold and tailwindcss intelligence extensions

```console
npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch
```

will create css folder and style.css file within and we can click go live
