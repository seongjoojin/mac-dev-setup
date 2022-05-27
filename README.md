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
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

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

##### java 설치

https://adoptium.net/?variant=openjdk8&jvmVariant=hotspot

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

zi(zsh 플러그인 매니저) 설치
https://github.com/z-shell/zi/

추천 플러그인 설치
```
zi light zdharma/fast-syntax-highlighting
zi light zsh-users/zsh-autosuggestions
zi light zsh-users/zsh-completions
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


## 프로그램

- [Hidden Bar](https://apps.apple.com/kr/app/hidden-bar/id1452453066?mt=12)
- [Dato](https://apps.apple.com/us/app/dato/id1470584107?mt=12)
- [Rocket Fuel](https://apps.apple.com/kr/app/rocket-fuel/id1114196460?mt=12)
- [AppCleaner](http://freemacsoft.net/appcleaner/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Google Chrome](https://www.google.co.kr/chrome/index.html)
- [Mozilla Firefox Developer Edition](https://www.mozilla.org/ko/firefox/developer/)
- [Slack](https://slack.com/)
- [virtualbox](https://www.virtualbox.org/) -> https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/
- [ridibooks](https://ridibooks.com/support/app/download)
- [MindNode 5](https://itunes.apple.com/app/mindnode-5/id1289197285?l=en&mt=12&ign-mpt=uo%3D4)
- [Magnet](https://itunes.apple.com/us/app/magnet/id441258766?mt=12)
- [Foldery](https://apps.apple.com/kr/app/foldery/id815333099?mt=12)
- [Bandizip](https://apps.apple.com/kr/app/반디집-압축-및-압축해제-프로그램/id1265704574?mt=12)
- [Trello](https://itunes.apple.com/us/app/trello/id1278508951?mt=12)
- [docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac)

참고 : https://github.com/iCHAIT/awesome-macOS

## 구글 확장 프로그램

- TrafficLight
- Wappalyzer
- React Developer Tools
- Redux DevTools
- The Marvellous Suspender (탭 관리)
- 파파고 번역 (Papago for Chrome)
- Bitwarden

## node-gyp 오류시 해결 방법

https://github.com/nodejs/node-gyp/blob/master/macOS_Catalina.md

```bash
$ sudo rm -rf $(xcode-select -print-path)
$ xcode-select --install
```

## Visual Studio Code 추가 설정

- [EditorConfig](https://editorconfig.org) 설정 - https://gist.github.com/seongjoojin/7c664b2fd78aa526924c1d746df52ab3
- typescriptreact snippet - https://gist.github.com/seongjoojin/c0d9220c371dde09f92c0610be52ba76

## ETC

#### git commit

- https://gitmoji.carloscuesta.me/
- https://github.com/ngryman/cz-emoji
- https://github.com/commitizen/cz-cli

#### 디자인 툴

- [figma](https://www.figma.com/)
- [adobe xd](https://www.adobe.com/kr/products/xd.html)
- [sketch](https://www.sketch.com)

