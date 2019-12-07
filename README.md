# yohobuy

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


# 配置vant
>- 安装vant: npm i vant --save
>- 配置vant按需引入: npm i babel-plugin-import --save-dev
```javascript
//在babel.config.js写入以下内容
module.exports = {
  plugins: [
    ['import', {
      libraryName: 'vant',
      libraryDirectory: 'es',
      style: true
    }, 'vant']
  ]
};
```
>- 配置rem: npm i postcss-pxtorem lib-flexible -D
```javascript
//在postcss.config.js写入以下内容
module.exports = {
  plugins: {
    'autoprefixer': {
      browsers: ['Android >= 4.0', 'iOS >= 7']
    },
    'postcss-pxtorem': {
      rootValue: 37.5,
      propList: ['*']
    }
  }
}
```