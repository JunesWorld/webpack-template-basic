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

컴파일 + 링크 : 분석한 소스코드로 실행 가능한 프로그램을 만듦</br>
package.json에서 build 스크립트 부분이 실행되고, 여기에 webpack이 있다면 실행되는 원리

## 개발 서버 오픈

```bash
npm i -D html-webpack-plugin
```

webpack.config.js -> plugins 추가 -> ```npm run dev```

## Favicon 설정(정적 파일 연결)

```npm i -D copy-webpack-plugin```

## module(CSS파일 읽게 하기)

```npm i -D css-loader style-loader```

## SCSS

```npm i -D sass-loader sass```