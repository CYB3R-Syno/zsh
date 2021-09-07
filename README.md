# 1. brew

zsh 를 설치하기 위해서는 brew를 먼저 설치를 해야합니다.

mac에서 제공하지 않는 패키지들을 brew를 통하여 설치하 수 있습니다.

우선 Terminal을 실행시켜줍니다.

<img width="792" alt="Screen Shot 2021-09-07 at 2 00 35 PM" src="https://user-images.githubusercontent.com/84657474/132286849-08edd81e-3246-48dc-a351-98804f8fafe9.png">

실행된 터미널에 다음과 같은 명령어를 입력해줍니다.
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

brew 사용법은 다음과 같습니다.
```
brew install Package
```

이렇게 brew 를 간단하게 설치하시 수 있습니다.

# 2. ZSH 

- [oh my zsh](https://ohmyz.sh)
- [oh my zsh github](https://github.com/ohmyzsh/ohmyzsh)
- [zsh](https://www.zsh.org)

mac은 기본적으로 __bash__ 를 사용합니다.

__zsh__ 는 터미널의 테마를 변경하여 색상을 변경하는 것도 가능하고 brew를 사용하여 다양한 패키지 설치도 가능합니다.

__oh my zsh__ 경우에는 더 많은 자료를 가지고 있으며 테마, 플러그인 등  엄청나게 많은 수를 제공하고있습니다.

터미널에 다음과 같은 명령을 실행하면 zsh 버전을 확인하 수 있습니다.
```
zsh --version
```

다음 명령을 실행하게되면 zsh 설치가 가능합니다.
```
brew install zsh
```

__진행 중 비밀번호를 입력하게 되는데, 사용하시는 mac에 비밀번호를 작성하시면 됩니다.__    

다음 명령어를 통하여 oh my zsh 설치가 가능합니다.
```
curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```

설치된 oh-my-zsh을 사용하도록 설정을 하면 zsh를 사용하기 위한 모든 작업이 종료됩니다.
```
chsh -s zsh 경로
```

zsh 경로는 다음 명령어르 통하여 확인이 가능합니다.
```
which zsh
```

<img width="1158" alt="Screen Shot 2021-09-07 at 2 15 43 PM" src="https://user-images.githubusercontent.com/84657474/132288029-82ca81c7-9371-486c-8374-ad3e224ccb8f.png">


# 3. zsh theme 설정
zsh 에 테마를 설정해주셔야합니다 !

oh my zsh에서 사용가능한 테마 목록들이 나열되어있습니다. (하단 url 참조)

맘에 드는 Theme를 선택해서 설정을 할 수 있습니다.

[oh my zsh theme](https://github.com/ohmyzsh/ohmyzsh/wiki/External-themes)

터미널에서 다음의 명령어를 입력하여 설정을 변경합니다.

vi에 익숙하실 경우에는 다음 명령어를 입력하여 수정하시면 되고,
```
vi ~/.zshrc
```

vim 명령어 사용이 어려우신 분은 다음 명령어를 입력해주세요.
```
open ~/.zshrc
```

파일을 열면 다음의 문구를 볼 수 있습니다.

ZSH_THEME=”테마명” 을 입력해주시면 됩니다. 

만약 어떤 것을 선택해야 할지 모르신다면 __random__ 을 입력하여 실행시마다 다른 테마를 맛볼 수 있다고 합니다.

```
# Set name of the theme to load.
# Look in ~/.oh-my-zsh/themes/
# Optionally, if you set this to "random", it'll load a random theme each
# time that oh-my-zsh is loaded.
ZSH_THEME="robbyrussell"
```

[참고]

사용자의 이름을 지정하지 않으면 ~ 앞에 사용자 이름이 표시됩니다.

.zshrc에 추가하려면 다음과 같이 추가해주시면 됩니다.

```
DEFAULT_USER="$(USER)"
```


저는 passion 을 사용하였습니다.

저장하고 터미널을 다시 실행합니다.

<img width="1158" alt="Screen Shot 2021-09-07 at 2 32 05 PM" src="https://user-images.githubusercontent.com/84657474/132289487-684c2da5-09e0-4247-826d-cf988760f752.png">

위 사진과 같이 테마가 적용된 부분을 보실 수 있습니다.
