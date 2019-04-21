# demo

> Work giving to Kevin

The task is as follows

Using nuxt (https://nuxtjs.org/) , vuetify (https://vuetifyjs.com/en/) and start a server side rendering project.
Create a dynamic profile page based on the URL for example http://localhost:3000/user/ben-zhang
In the page, it should show an h1 tag of the name Ben Zhang. The page meta tag should have dynamically title tag based on URL and description based on URL.

** This is done in /pages/user/_id.vue

Assuming URL is /user/firstname-lastname-number

** This is done in /pages/user/_id.vue

The page content should show h1 tag Firstname Lastname, and a content of user id: number

** This is done in /pages/user/_id.vue

Make sure the page is SSR. We will check the source code, not the browser rendering, like Google crawling the site.

** Spent 1hr (and extra on github).

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).
