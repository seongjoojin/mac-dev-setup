# Mac 환경 설정 모음

#### 맥 초기화 방법

https://support.apple.com/ko-kr/HT204904

- command(⌘)-R : 이후 버전으로 업그레이드하지 않고 Mac에 설치되어 있던 최신 macOS를 설치합니다.
- option-command-R : Mac과 호환되는 최신 macOS로 업그레이드합니다
- shift-option-command-R: Mac과 함께 제공되는 macOS 또는 현재 사용할 수 있는 macOS 중 최신 버전을 설치합니다.

##### 자주 사용하는 프로그램 설치는 Homebrew 사용

```
# Homebrew 설치
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# wget 설치
brew install wget

# git 설치
brew install git

# node 설치
brew install node

# yarn 설치
brew install yarn
```

## 폰트

- [D2 Conding](https://github.com/naver/d2codingfont) : 코딩시 사용 (에디터 폰트설정) 

## 터미널

- [iTerm2](https://www.iterm2.com/)
- iTerm2 Color Scheme - [Adventure Time](https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/schemes/AdventureTime.itermcolors)
- zsh

```
# zsh 설치
brew install zsh

# 기본 터미널 zsh로 변경
chsh -s `which zsh`
```

- oh-my-zsh

```
# oh-my-zsh (wget) 설치
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

## 커맨드라인 인터페이스 도구

- [nvm](https://github.com/creationix/nvm) : 노드 버전 관리
- [n](https://github.com/tj/n) : 노드 버전 관리
- git

```
git config --global user.name "Seongjoo Jin"
git config --global user.email "qpyou1234@naver.com"
```

## 언어

- Vue CLI

```
yarn global add @vue/cli
```

## 프로그램

- [AppCleaner](http://freemacsoft.net/appcleaner/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Google Chrome](https://www.google.co.kr/chrome/index.html)
- [Mozilla Firefox Developer Edition](https://www.mozilla.org/ko/firefox/developer/)
- [Dash](https://kapeli.com/dash)
- [Postman](https://www.getpostman.com/)
- [TunnelBear](https://www.tunnelbear.com/)
- [SourceTree](https://www.sourcetreeapp.com/)
- [Sequel Pro](https://www.sequelpro.com/) - MySQL
- [Slack](https://slack.com/)
- [KeepingYouAwake](https://github.com/newmarcel/KeepingYouAwake)
- [itsycal](https://www.mowglii.com/itsycal/)
- [virtualbox](https://www.virtualbox.org/) -> https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/
- [ridibooks](https://ridibooks.com/support/app/download)
- [monosnap](https://www.monosnap.com/welcome)
- Evernote
- Popclip
- Magnet
- Foldery
- Bandizip
- Allkdic
- Boom3d(예정)
- [Bartender(예정)](https://www.macbartender.com/) : 메뉴바 정리 앱

참고 : https://github.com/iCHAIT/awesome-macOS

## 구글 확장 프로그램

- TrafficLight
- Vue.js devtools : https://kr.vuejs.org/v2/api/index.html#devtools (app.js 설정)
- Wappalyzer
- CSS3 Generator
- Site Palette
- React Developer Tools
- JavaScript Errors Notifier
- CSS Peeper
- CSSViewer
- Evernote Web Clipper
- Pixlr Today
- The Great Suspender
- Awesome Screenshot

## Visual Studio Code 확장프로그램

- [Vue Development Extension Pack](https://marketplace.visualstudio.com/items?itemName=changjoo-park.vscode-vue-devpack)
- [Reactjs code snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.ReactSnippets)

## ETC

#### 스타일 가이드

- [awesome-style-guide](https://github.com/kciter/awesome-style-guide)

#### 라이브러리들

- [XEIcon](https://xpressengine.github.io/XEIcon/)
- [Font Awesome](https://fontawesome.com/)
- [Moment.js](https://momentjs.com/)
- [awesome-vue](https://github.com/vuejs/awesome-vue)
- [awesome-nuxt](https://github.com/nuxt-community/awesome-nuxt)

#### 기타

- [CSS 방법론](https://gomdoreepooh.github.io/notes/smacss-bem-oocss)
- [Vue + ES6](https://joshua1988.github.io/es6-online-book/)
- [HEX to RGB Converter](https://www.webpagefx.com/web-design/hex-to-rgb/)
- [Webpack](https://d2.naver.com/helloworld/0239818)
- [React Developer Roadmap](https://github.com/adam-golab/react-developer-roadmap)
