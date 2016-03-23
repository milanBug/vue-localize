# vue-localize

> Localization plugin for vue.js based applications with Vuex and VueRouter

## Lnks

- Webpack
- VueRouter
- Vuex

## Functionality and features
- Easy integration in your application in just two places
- Current language is a Vuex state changed only via mutations
- Saving selected language in local storage
- Fallback language support
- Automatic routes localization: ```/about ===> /en/about, /ru/about,...``` only with official VueRouter
- Wrapper for route name for using in v-link for proper navigation: ``` v-link="{name: $localizeRoute('about')}" ```
- Translating page title
- Route path translating tool: ``` $translateRoutePath($route.path, $route.name, lang) ```
- Option for excluding language part from route path for default language
- Option for custom name of the key in local storage
- Global mixin for getting current language in Vue components via Vuex getter "currentLanguage"
- Translating phrases via Vue filter: ```{{ phrase | translate }}```
- Translating phrases via direct call of plugin method: ``` {{ $translate(phrase) }} or v-text="$translate(phrase)" ```
- Translating phrases via Vue directive: ``` v-localize="{path: 'header.nav.home'}" ```
- Injection of custom variables into translations: ``` {{ $translate(phrase, objVars) }} ```
- Translating to exact language regardless of current selected: ``` {{ $translate(phrase, null, 'en') }} ```
- Reactive UI translating via language selector
- Flexible context-based translations structure
- Language selector inplementation tutorial
- Separate NPM package

## Installation

In your project folder (where is package.json)

```bash
$ npm install vue-localize --save
```

## Integration

Plugin importing and Vuex module registration

## Configuration options and config tutorial

## Translations file tutorial

## Automatic routes localization


