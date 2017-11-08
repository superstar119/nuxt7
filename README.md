<p align="center">
    <img src="https://github.com/pi0/nuxt7/raw/master/.assets/nuxt7.png" alt="Nuxt7">
</p>

<p align="center">
<a href="https://david-dm.org/pi0/nuxt7">
    <img alt="" src="https://david-dm.org/pi0/nuxt7/status.svg?style=flat-square">
</a>
<a href="https://npmjs.com/package/nuxt7">
    <img alt="" src="https://img.shields.io/npm/v/nuxt7/latest.svg?style=flat-square">
</a>
<a href="https://npmjs.com/package/nuxt7">
    <img alt="" src="https://img.shields.io/npm/dt/nuxt7.svg?style=flat-square">
</a>
<a href="https://circleci.com/gh/pi0/nuxt7">
    <img alt="" src="https://img.shields.io/circleci/project/github/pi0/nuxt7/master.svg?style=flat-square">
</a>
<a href="https://standardjs.com">
    <img alt="" src="https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square">
</a>
</p>

<p align="center">
Full Featured iOS & Android <strong>PWA</strong> Apps with <a href="https://nuxtjs.org">Nuxt.js</a> and <a href="https://framework7.io">Framework7</a>
<br>
</p>

<a href="./CHANGELOG.md">📖 Release Notes</a>

Nuxt7 integrates universal nuxt.js applications with [Framework7](https://framework7.io/)[-Vue](https://framework7.io/vue)
to rapidly create efficient and feature-reach [PWA](https://developers.google.com/web/progressive-web-apps) mobile applications with help of [pwa-module](https://github.com/nuxt-community/pwa-module). Production builds can be statically hosted or running offline.

## ✨ Features

- Fully compatible with framework7 2.x
- Development mode with hot reloading
- Optimized production builds suitable for 100% static hosting
- Fully PWA compatible out of the box
- Page based router for Framework7
- Use vuex store in your apps
- Familiar nuxt.js development experience with a super easy learning curve

## ⚔️ Quick Start

Using starter template for is recommended. Use the command below to create a new app:

```cmd
npx sao nuxt-community/nuxt7 nuxt7-app
```

## 👉 Demo
Latest version is always published here: https://nuxt7.cf

🔦 Lighthouse tests: [Mobile Regular 3G](https://www.webpagetest.org/result/171108_XA_8a8f20e7c71b24cb17e3c269cb5d8a5c)

## Module options

Add options as `framework7` key inside `nuxt.config.js`.

Option          | Type         | Default   |  Description
----------------|--------------|-----------|--------------------------------------------------------------
`css`           | Boolean      | `true`    | Include Framework7 css (disable to provide a custom build)
`rtl`           | Boolean      | `false`   | Enable RTL layout
`f7Icons`       | Boolean      | `true`    | Include Framework7 Icons (IOS)
`mdIcons`       | Boolean      | `true`    | Include MD Icons
`routes`        | Object       | `true`    | Route overrides (see below)
`mode`          | String       | `hash`    | Router mode. Can be `hash` or `history`
`view`          | Object       | <!-- -->  | Options passed to root view of framework7

### routes override
Routes are auto generated using pages directory structure.
However if you need to make more customization (Like adding routable tabs) this option may be used.

Example: (**nuxt.config.js**)

```js
framework7: {
    routes: {
      'tabs-routable': {
        tabs: [
          { path: "/", id: "tab1" },
          { path: "/tab2/", id: "tab2" },
          { path: "/tab3/", id: "tab3" },
        ]
      }
    }
}
```

## 🍳 Development

```bash
> yarn dev
```

## License

MIT - Nuxt Community - Pooya Parsa
