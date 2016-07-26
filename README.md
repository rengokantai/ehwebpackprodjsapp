#### ehwebpackprodjsapp
######polyfill promises for webpack2
add user agent
```
?ua=Mozilla/5.0%20(Windows;%20U;%20MSIE%209.0;%20WIndows%20NT%209.0;%20en-US))
```

######12 Initialize a webpack project with karma for testing
```
npm install --save-dev karma karma-chrome-launcher mocha karma-mocha
```
karma.conf.js
```
module.exports = function(config){
  config.set({
    basePath:'',
    frameworks:['mocha'],
    files:[
      'src/js/**/*.js'
    ],
    exclude:[],
    preprocessors:{},
    reporters:['progress'],
    port:9876,
    colors:true,
    logLevel:config.LOG_INFO,
    autoWatch:false,
    browsers:['chrome'],
    singleRun:false,
    concurrency: Infinity
  })
})
```
