# Gulp 세팅

## 선행

### `Node.js` : v20.15.0

> Node.js는 Chrome V8 JavaScript 엔진으로 빌드된 JavaScript 런타임 환경으로, 서버 사이드에서 JavaScript를 실행할 수 있게 해줍니다. 이를 통해 비동기적이고 이벤트 기반의 서버 사이드 프로그래밍을 할 수 있으며, 네트워크 응용 프로그램 개발 등 다양한 용도로 활용됩니다. Node.js는 자바스크립트로 서버를 구축하고 관리하는 간단하고 효율적인 방법을 제공합니다.

1. **비동기 이벤트 기반**: I/O 작업을 비동기적으로 처리하여 여러 작업을 동시에 처리할 수 있습니다. 이는 Node.js가 대규모 데이터 처리나 실시간 애플리케이션에 적합하게 만듭니다.
1. **단일 스레드**: 단일 스레드 모델을 기반으로 하되, 이벤트 루프를 통해 여러 작업을 동시에 처리할 수 있습니다.
1. **모듈 시스템**: CommonJS 모듈 시스템을 따르며, 모듈 간의 코드를 재사용하기 쉽게 해줍니다.
1. **간편한 패키지 관리**: npm(Node Package Manager)을 통해 다양한 패키지를 손쉽게 관리하고 사용할 수 있습니다.
1. **확장성**: 비동기적인 자연으로 인해 대규모 애플리케이션에 적합하며, 클러스터링과 로드 밸런싱을 통해 확장성을 높일 수 있습니다.

### `gulp-cli` : v3.0.0

gulp-cli는 Gulp를 터미널에서 편리하게 실행할 수 있게 해주는 유틸리티 도구입니다.

## 사용된 패키지

### `gulp` : v4.0.2

Gulp core. (5버전은 좀 더 지켜보기)

### `@babel/core` : v7.19.3

Babel core.

### `@babel/preset-env` : v7.19.4

브라우저 지원 대상에 따라 필요한 Babel 기능을 정의.

### `@babel/register` : v7.18.9

파일이 로드될 때 즉시 컴파일.

### `gulp-nunjucks-render` : v2.2.3

Nunjucks core.

### `gulp-plumber` : v1.2.1

에러 구문 발생 시 Gulp 먹통 방지.

### `gulp-cached` : v1.1.1

수정되는 파일만 감지하여 빌드.

### `gulp-data` : v1.3.1

json, 데이터베이스 등을 Gulp pipe에 적용.

### `fs` : v0.0.1-security
filesystem 약자. 파일에 접근하여 읽기, 쓰기 등을 수행.

### `del` : v6.0.0

폴더 삭제.

> 최신버전 ESM 이슈로 하위 버전 사용

### `gulp-webserver` : v0.9.1

브라우저 실시간 반영.

### `path` : v0.12.7

디렉토리 경로 추출. (파일 변경 감지용)

### `gulp-sass` : v5.1.0

gulp-sass core.

### `sass` : v1.77.6

Sass 컴파일러.

### `gulp-dependents` : v1.2.5

종속된 SCSS 파일 감지.

### `gulp-postcss` : v10.0.0

Sass 후처리기.

### `autoprefixer` : v9.8.5

PostCSS 플러그인. 벤더 접두사 적용.

> 최신 버전은 아직 지켜봄

### `gulp-sourcemaps` : v3.0.0

SCSS 디버깅.

### `gulp-minify-css` : v1.2.4

CSS 압축.

### `gulp-rename` : v2.0.0

파일명 변경.

### `gulp-minify` : v3.1.0

js 파일 압축용.

### `gulp-imagemin` : v7.1.0

이미지 최적화.

> 애플실리콘 기기(M1~)의 경우 rosetta2 설치 필요<br>
> 최신버전 ESM 이슈로 하위 버전 사용

### `gulp-newer` : v1.4.0

변경된 파일만 파이프라인 통과.

## 과제

- 폴더 삭제 시 실시간 반영이 안됨.
