# Webpack-template-basic

## Package Install

```bash
npm i -D webpack webpack-cli webpack-dev-server@next
```

package.json
```
"scripts": {
    "dev": "webpack-dev-server --mode development",
    "build": "webpack --mode production"
  },
```
- dev : 현재 개발 모드
- build : 제품 모드
- webpack : bundler가 동작하기 위한 핵심 package
- webpack-cli : Command Line Interface 지원
  - parcel은 자동 지원
- webpack-dev-server : dev를 통해 server를 open 할 때 바로 새로고침하기 위해서 사용

## webpack.config.js

webpack은 브라우저에서 동작하는 것이 아닌 Node.js 환경에서 동작한다.

## npm run build

= npm run dev

## 개발 서버 오픈

```bash
npm i -D html-webpack-plugin
```

webpack.config.js -> plugins 추가