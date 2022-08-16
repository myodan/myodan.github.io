---
title: "Git 초기 설치 및 설정"
date: 2022-08-16T01:13:12+09:00
draft: false
---

이번에는 Git의 설치 방법과 기초 설정을 알아보도록 합시다.

## 설치

설치하는 패키지 매니저를 이용해서 설치하도록 하겠습니다.

### Windows (Winget)

Windows는 최근에 새로 출시된 패키지 매니저인 `Winget`를 이용해서 설치하도록 합시다.
Winget은 윈도우에 기본 설치되도록 되어있습니다.

다음 커맨드를 이용해서 설치하면 됩니다.

```shell
winget install --id Git.Git
```

Windows 버전의 Git은 Git LFS, Git Flow를 포함하고 있어 따로 설치해줄필요는 없습니다.

만약 Winget이 작동하지 않는다면 이 [링크](https://gitforwindows.org)를 이용해서 설치하시면 됩니다.

### macOS (Homebrew)

macOS는 기본으로 Git이 설치되어있지만, 구버전이니 최신 버전을 다시 설치합시다.

macOS에서 주로사용되는 패키지 매니저인 `Homebrew`를 이용해서 설치하도록 합시다.
Homebrew 설치는 이 [링크](https://brew.sh/index_ko)를 참고하여 설치하시면 됩니다.

Homebrew를 설치하고 다음 커맨드를 이용해서 설치하시면 됩니다.

```shell
brew install git git-lfs git-flow
```

자기 OS에 맞게 설치한 뒤에 아래 커맨드를 이용해서 제대로 최신 버전이 설치되었는지 확인합시다.

```shell
git --version
```

## 기초 설정

우선 깃 커밋이나 PR등에서 사용될 사용자 이름과 이메일을 설정하도록 합시다.

```shell
git config --global user.name "Your name"
git config --global user.email "Your email"
```

다음으로 GitHub에서 기본 브런치이름이 `master`에서 `main`으로 변경되었습니다.
main으로 변경된 이유가 주종(주인과 노예)관계를 뜻하는 `master`, `slave`를 다른 단어로 대체되기 위해서라고 알고 있습니다.

저도 위 의견에 동의하기 때문에 기본 브랜치 이름을 main으로 변경하도록 하겠습니다.

본래 Git에는 기본 브랜치 변경 설정이 없었지만, `2.28`버전 이후로 업데이트되었습니다.

변경 방법은 아래와 같습니다.

```shell
git config --global init.defaultBranch "Branch name"
```

마지막으로 설정이 제대로 됐는지 확인해보도록 합시다.

```shell
git config --list
```

위 커맨드로 제대로 설정이 적용되었는지 확인해보겠습니다.

```shell
user.name=Your name
user.email=Your email
init.defaultbranch=Branch name
```

설정이 됬으면 Git 설정이 끝났습니다.

여기까지 읽어주셔서 감사합니다!
