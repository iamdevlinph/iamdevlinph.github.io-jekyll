---
layout: article
title:  "React, Redux, Redux-Saga, Ducks Pattern Boilerplate"
date:   2017-12-29 12:29:47 +0800
group: "blog"
comments: true
---
A react, redux, redux-saga, ducks pattern boilerplate.

## Why create a boilerplate
<hr class='divider--fade' />

[Cory House](https://github.com/coryhouse) had a talk about creating a JavaScript starter kit and this is my attempt to it. I'm planning on using this boilerplate for my future projects, as well as integrate some new features along the way.

## What it includes
<hr class='divider--fade' />

* React v16
* Redux
* Redux-Saga
* React Router v4
* Ducks pattern
* SCSS
* Webpack v3
* node-sass-chokidar (add support for sass in create-react-app)
* ES Lint

### React
This project includes the latest react version as of this writing which is `React v16`

### Redux-Saga
I have only known `redux-thunk` aside from `redux-saga` and I've decided to go with the latter because it looked easier.

### Ducks Pattern
Before I've known this pattern, I've been doing the usual way of putting all `actions`, `reducers`, and `actionTypes` into one place. Which breaks the folder by feature aspect that I've trying to follow. And with this `ducks pattern`, all related `actions, `reducers`, and `actionTypes` are put into one file that also makes maintaining easier.

### SCSS
What appeals to me the most is the ability to nest classes that make isolation of styles easier. And also the other features that I rarely use.

### node-sass-chokidar
This boilerplate aims to avoid the use of `npm run eject` and stick with the original config that is provided by `create-react-app`.

## Side effects of not running `npm run eject`
<hr class='divider--fade' />

Not running the eject script also some side effects. The main problem is that we cannot touch the `webpack config` file since it is locked away.
