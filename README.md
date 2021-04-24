<p>
    <a href="https://tailwindcss.com/" target="_blank">
      <img alt="Tailwind CSS" width="350" src="https://refactoringui.nyc3.cdn.digitaloceanspaces.com/tailwind-logo.svg">
    </a><br>
    A utility-first CSS framework for rapidly building custom user interfaces.
</p>

<p>
    <a href="https://travis-ci.org/tailwindcss/tailwindcss"><img src="https://img.shields.io/travis/tailwindcss/tailwindcss/master.svg" alt="Build Status"></a>
    <a href="https://www.npmjs.com/package/tailwindcss"><img src="https://img.shields.io/npm/dt/tailwindcss.svg" alt="Total Downloads"></a>
    <a href="https://github.com/tailwindcss/tailwindcss/releases"><img src="https://img.shields.io/npm/v/tailwindcss.svg" alt="Latest Release"></a>
    <a href="https://github.com/tailwindcss/tailwindcss/blob/master/LICENSE"><img src="https://img.shields.io/npm/l/tailwindcss.svg" alt="License"></a>
    <a href="https://codecov.io/gh/tailwindlabs/tailwindcss"><img src="https://codecov.io/gh/tailwindlabs/tailwindcss/coverage.svg?branch=master" alt="Code Coverage"></a>
</p>

------

## Documentation

For full documentation, visit [tailwindcss.com](https://tailwindcss.com/).

## Community

For help, discussion about best practices, or any other conversation that would benefit from being searchable:

[Discuss Tailwind CSS on GitHub](https://github.com/tailwindcss/tailwindcss/discussions)

For casual chit-chat with others using the framework:

[Join the Tailwind CSS Discord Server](https://discord.gg/7NF8GNe)

## Contributing

If you're interested in contributing to Tailwind CSS, please read our [contributing docs](https://github.com/tailwindcss/tailwindcss/blob/master/.github/CONTRIBUTING.md) **before submitting a pull request**.


## Installálás

Node package manager segítségével
npm init -y
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest postcss-cli@latest cssnano@latest onchange@latest
npx tailwindcss init

src mappa létrehozás és benne egy tailwind.css

Majd a fenti fájlba
@tailwind base;
@tailwind components;
@tailwind utilities;

És a package.json -ba kell script is
```javascript
"scripts": {
    "build": "postcss css/tailwind.css -o public/build/tailwind.css"
    "watch": "postcss css/tailwind.css -o public/build/tailwind.css --watch"
}
```

Majd public mappába index.html

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="build/tailwind.css" />
  </head>
  <body>
    <h1 class="text-4xl font-bold text-center text-blue-500">First taste of tailwind</h1>
  </body>
</html>

https://www.youtube.com/watch?v=bxmDnn7lrnk
