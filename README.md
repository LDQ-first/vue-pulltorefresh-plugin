# vue-pulltorefresh-plugin

> A pull to refresh plugin of Vue.js 

[Demo](http://ldqblog.me/vue-pulltorefresh-plugin/dist/#/)

[more detail of use](https://github.com/LDQ-first/vue-pulltorefresh-plugin/tree/master/src/views/show.vue)

## Use

``` javascript
/*-- npm --*/
npm install --save vue-pull-to-refresh
```
  
``` javascript
/*-- main.js --*/
import Vue from 'vue'
import VuePullToRefresh from 'vue-pull-to-refresh'
Vue.use(VuePullToRefresh)
```

                
```
<!--html-->
<pull-refresh :next="pullRefresh" >
    <div slot="list">
        Your code
    </div>
</pull-refresh>

```

## Param

``` javascript
/*
    pull to touch off this function
    must return promise 
*/
next: {
    type: Function,
    required: true
},
/*
   chinese or english can set default tip
   other language can't set default tip but you can set tip by yourself and also don't have to set language
*/
language: {
    type: String,
    required: false
},
/*
    set pullTip
*/
pullTip: {
    type: String,
    required: false
},
/*
    set releaseTip
*/
releaseTip: {
    type: String,
    required: false
},
/*
    set loadingTip
*/
loadingTip: {
    type: String,
    required: false
},
/*
    set pullDistance
*/
pullDistance: {
    type: Number,
    required: false
},
/*
    set releaseDistance
*/
releaseDistance: {
    type: Number,
    required: false
},
/*
    set maxDistance
*/
maxDistance: {
    type: Number,
    required: false
}

```

## Dependencies

* SASS


## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
