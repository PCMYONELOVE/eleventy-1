# Мой блог (base on Eleventy)

<p align="center">
  <a href="#"><img src="preview.png?raw=true" alt="Главная страница"></a>
</p>

⚡️ Built with [Eleventy](https://www.11ty.dev)

### Requirements

- Node.js and npm

### Project structure

```
.
├── public             # Static files
│   └── assets
│       └── images     # Images not needed by Webpack
└── src
    ├── _data          # Eleventy data folder
    ├── _includes
    │   └── layouts    # HTML layout files
    ├── assets         # Assets folder that needs to be processed by Webpack
    │   ├── images
    │   │   └── posts  # Images used in your blog posts (will be compressed by Webpack)
    │   └── styles     # Your blog CSS files
    └── posts          # Your blog posts
```

### Customization

You can easily configure Eleventy Starter Boilerplate. Please change the following file:

- `public/assets/images/logo.png`: your blog logo
- `public/apple-touch-icon.png`, `public/favicon.ico`, `public/favicon-16x16.png` and `public/favicon-32x32.png`: your blog favicon, you can generate from https://favicon.io/favicon-converter/
- `src/_data/site.json`: your blog configuration
- `src/_includes/layouts`: your blog HTML layout
- `src/assets/styles/main.css`: your blog CSS file using Tailwind CSS

### Deploy to Netlify

Clone this repository on own GitHub account and deploy to Netlify:

[![Netlify Deploy button](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/ixartz/Eleventy-Starter-Boilerplate&stack=cms)

### Remove Netlify files and Netlify CMS

If you don't use Netlify, you can easily remove all Netlify related files:

- `public/admin`, the entier folder
- `src/_includes/layouts/base.ejs`, the loaded script `netlify-identity-widget.js` and the inline script `if (window.netlifyIdentity) { ...`
- `netlify.toml`, the entire file

### License

Licensed under the MIT License, Copyright © 2020

See [LICENSE](LICENSE) for more information.

---
