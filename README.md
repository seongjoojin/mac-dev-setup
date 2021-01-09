# Mac 환경 설정 모음

#### homebrew 권한 문제 해결 gist

https://gist.github.com/irazasyed/7732946

#### 개발자를 위한 OS X(>= Catalina) 설정

https://www.sangkon.com/osx-setting-for-developer/

#### 맥 초기화 방법

https://support.apple.com/ko-kr/HT204904

- command(⌘)-R : 이후 버전으로 업그레이드하지 않고 Mac에 설치되어 있던 최신 macOS를 설치합니다.
- option-command-R : Mac과 호환되는 최신 macOS로 업그레이드합니다
- shift-option-command-R: Mac과 함께 제공되는 macOS 또는 현재 사용할 수 있는 macOS 중 최신 버전을 설치합니다.

https://pqrs.org/osx/karabiner/
키보드 맵핑 변경

##### dns 설정

- Cloudflare https://1.1.1.1/ko-KR/dns/
- Google https://developers.google.com/speed/public-dns
- IBM https://www.quad9.net/apple/

##### 자주 사용하는 프로그램 설치는 Homebrew 사용

```
# Homebrew 설치
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# 이 저장소 클론
git clone https://github.com/seongjoojin/mac-dev-setup
cd mac-dev-setup

# Brewfile 실행
brew bundle
```

만약 Brewfile가 제대로 설치되지 않는다면 아래 명령어로 추가

```
# wget 설치
brew install wget

# git 설치
brew install git

# yarn 설치
brew install yarn
```

## 폰트

- [D2 Conding](https://github.com/naver/d2codingfont) : 코딩시 사용 (에디터 폰트설정)
- [FiraCode](https://github.com/tonsky/FiraCode)

## 터미널

- [hyper](https://hyper.is/) => [awesome-hyper](https://github.com/bnb/awesome-hyper), 저장소 `.hyper.js` 참고
- [iTerm2](https://www.iterm2.com/)
- iTerm2 Color Scheme - [Adventure Time](https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/schemes/AdventureTime.itermcolors)
- fish

```
# fishshell 설치
brew install fish

# 기본 터미널 fishshell로 변경
echo "/usr/local/bin/fish" | sudo tee -a /etc/shells
chsh -s /usr/local/bin/fish
```

- starship

https://starship.rs/guide/#🚀-installation

- oh-my-fish

```
# oh-my-fish 설치
curl -L https://get.oh-my.fish | fish
```

- fish shell config 파일 작성

`sudo vi ~/.config/fish/config.fish`

- oh-my-zsh

```
# oh-my-zsh 설치
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

https://github.com/ohmyzsh/ohmyzsh

oh-my-fish 테마 설정
https://github.com/oh-my-fish/oh-my-fish/blob/master/docs/Themes.md

추천 테마 powerlevel10k
https://github.com/romkatv/powerlevel10k

zinit(zsh 플러그인 매니저) 설치
https://github.com/zdharma/zinit

추천 플러그인 설치
```
zinit light zdharma/fast-syntax-highlighting
zinit light zsh-users/zsh-autosuggestions
zinit light zsh-users/zsh-completions
```

zsh plugin 설정
https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins

.zshrc 설정

```
ZSH_THEME="powerlevel10k/powerlevel10k"

plugins=(git
  adb
  brew
  docker
  docker-compose
  iterm2
  flutter
  pod
  python
  node
  react-native
  xcode
  yarn
  gradle
  gem
  npm
  npx
  vscode)
```

oh-my-zsh 테마 설정
https://github.com/robbyrussell/oh-my-zsh/wiki/Themes

powerlevel10k

https://github.com/romkatv/powerlevel10k#oh-my-zsh

- zsh shell config 파일 작성

`sudo vi ~/.zshrc`

## 유용한 커맨드 라인 도구

- [bat](https://github.com/sharkdp/bat)
- [exa](https://github.com/ogham/exa)

## 커맨드라인 인터페이스 도구

- [nvm](https://github.com/creationix/nvm) : 노드 버전 관리
- [n](https://github.com/tj/n) : 노드 버전 관리
- git

```
git config --global user.name "Seongjoo Jin"
git config --global user.email "evanjin8@gmail.com"
```

## mysql 설정

설치 : `brew install mysql@5.7`

서비스 시작 : `brew services start mysql@5.7`

비밀번호 설정 : `mysql_secure_installation`

mysql 실행 : `mysql -u root -p`


## mongodb 설정

설치 : `brew install mongodb-community`

실행 : `brew services start mongodb/brew/mongodb-community`

## heroku

https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up

## 언어

- Vue CLI

```
yarn global add @vue/cli
```

## 추가 설치 프로그램

- [docker](https://hub.docker.com/?overlay=onboarding)
- [postgresapp](https://postgresapp.com/downloads.html)
- [pgadmin](https://www.pgadmin.org/download/)

## 프로그램

- [Bear](https://apps.apple.com/kr/app/%EB%B2%A0%EC%96%B4-%EC%9E%91%EB%AC%B8-%EB%B0%8F-markdown-%ED%8E%B8%EC%A7%91%EC%9E%90/id1091189122?mt=12)
- [Dato](https://apps.apple.com/us/app/dato/id1470584107?mt=12)
- [gitkraken](https://www.gitkraken.com/git-client)
- [AppCleaner](http://freemacsoft.net/appcleaner/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Google Chrome](https://www.google.co.kr/chrome/index.html)
- [Mozilla Firefox Developer Edition](https://www.mozilla.org/ko/firefox/developer/)
- [Postman](https://www.getpostman.com/)
- [TunnelBear](https://www.tunnelbear.com/)
- [Slack](https://slack.com/)
- [virtualbox](https://www.virtualbox.org/) -> https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/
- [ridibooks](https://ridibooks.com/support/app/download)
- [MindNode 5](https://itunes.apple.com/app/mindnode-5/id1289197285?l=en&mt=12&ign-mpt=uo%3D4)
- [Evernote](https://itunes.apple.com/us/app/evernote/id281796108?mt=8)
- [Magnet](https://itunes.apple.com/us/app/magnet/id441258766?mt=12)
- [Foldery](https://apps.apple.com/kr/app/foldery/id815333099?mt=12)
- [Bandizip](https://apps.apple.com/kr/app/반디집-압축-및-압축해제-프로그램/id1265704574?mt=12)
- [things3](https://culturedcode.com/things/mac/appstore/)
- [Trello](https://itunes.apple.com/us/app/trello/id1278508951?mt=12)
- [Bartender](https://www.macbartender.com/) : 메뉴바 정리 앱
- [docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac)
- [miniconda](https://docs.conda.io/en/latest/miniconda.html)
  - 설치 : `$ bash Miniconda3-latest-MacOSX-x86_64.sh`
  - 터미널에서 실행 : `export PATH="$HOME/miniconda3/bin:$PATH"`

참고 : https://github.com/iCHAIT/awesome-macOS

## 구글 확장 프로그램
- TrafficLight
- Vue.js devtools : https://kr.vuejs.org/v2/api/index.html#devtools (app.js 설정)
- Wappalyzer
- React Developer Tools
- Octotree (깃허브 소스 보기)
- Great Suspender (탭 관리)

## node-gyp 오류시 해결 방법

https://github.com/nodejs/node-gyp/blob/master/macOS_Catalina.md

```bash
$ sudo rm -rf $(xcode-select -print-path)
$ xcode-select --install
```

## Visual Studio Code 추가 설정

- [EditorConfig](https://editorconfig.org) 설정 - https://gist.github.com/seongjoojin/7c664b2fd78aa526924c1d746df52ab3
- typescriptreact snippet - https://gist.github.com/seongjoojin/c0d9220c371dde09f92c0610be52ba76

## Visual Studio Code 테마

- [Snazzy Operator](https://marketplace.visualstudio.com/items?itemName=aaronthomas.vscode-snazzy-operator)
- [Shades of Purple](https://marketplace.visualstudio.com/items?itemName=ahmadawais.shades-of-purple)

## ETC

#### git commit

- https://gitmoji.carloscuesta.me/
- https://github.com/ngryman/cz-emoji
- https://github.com/commitizen/cz-cli

#### 디자인 툴

- [figma](https://www.figma.com/)
- [adobe xd](https://www.adobe.com/kr/products/xd.html)
- [sketch](https://www.sketch.com)

#### 스타일 가이드

- [awesome-style-guide](https://github.com/kciter/awesome-style-guide)

#### 라이브러리들

- [XEIcon](https://xpressengine.github.io/XEIcon/)
- [Font Awesome](https://fontawesome.com/)
- [Moment.js](https://momentjs.com/)


#### 기술 블로그

- [kakao 기술 블로그](http://tech.kakao.com/)
- [우아한형제들 기술 블로그](http://woowabros.github.io/)
- [Naver D2 개발 블로그](https://d2.naver.com/home)
- [줌인터넷 기술블로그](https://zuminternet.github.io/)
- [티몬 개발블로그](https://tmondev.blog.me/)
- [Meetup : NHN TOAST](http://meetup.toast.com/)
- [조대협의 블로그](http://bcho.tistory.com/)
- [조인석의 브런치](https://brunch.co.kr/@insuk)
- [jojoldu](http://jojoldu.tistory.com/)
- [소용환의 생각저장소](http://www.sauru.so/)
- [Wisoft Lab.](http://wisoft.tistory.com/)
- [개발 책추천](http://blog.ngelmaum.org/category/%EB%AC%B8%ED%99%94%EC%9D%B4%EC%95%BC%EA%B8%B0)
- [기발자](https://brunch.co.kr/@brunch92ny)

#### 기타

- [CSS 방법론](https://gomdoreepooh.github.io/notes/smacss-bem-oocss)
- [Vue + ES6](https://joshua1988.github.io/es6-online-book/)
- [HEX to RGB Converter](https://www.webpagefx.com/web-design/hex-to-rgb/)
- [Webpack](https://d2.naver.com/helloworld/0239818)
- [더 나은 웹](https://github.com/0vv/betterweb.kr)
