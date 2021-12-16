---
title: Git 초기 설치 및 설정
date: 2021-12-17 03:16:01
tags: Git
---
이번에는 Git의 설치 방법과 기초 설정을 알아보도록 합시다.

## 설치

설치하는 패키지 매니저를 이용해서 설치하도록 하겠습니다.

### Windows (Winget)

Windows는 최근에 새로 출시된 패키지 매니저인 `Winget`를 이용해서 설치하도록 합시다.
Winget은 윈도우에 기본 설치되도록 되어있습니다.

다음 커맨드를 이용해서 설치하면 됩니다.

{% codeblock Shell lang:shell %}
winget install --id Git.Git
{% endcodeblock %}

Windows 버전의 Git은 Git LFS, Git Flow를 포함하고있어 따로 설치해줄필요는 없다.

만약 Winget이 작동하지않는다면 이 [링크](https://gitforwindows.org/)를 이용해서 설치하시면됩니다.

### macOS (Homebrew)

macOS는 기본으로 Git이 설치되어있지만 구버전이니 최신버전을 다시 설치합시다.

macOS는 macOS에서 주로사용되는 패키지 매니저인 `Homebrew`를 이용해서 설치하도록 합시다.
Homebrew설치는 이 [링크](https://brew.sh/index_ko)를 참고하여 설치하도록 하면됩니다.

Homebrew를 설치하고 다음 커맨드를 이용해서 설치하시면 됩니다.

{% codeblock Shell lang:shell %}
brew install git git-lfs git-flow
{% endcodeblock %}

자기 OS에 맞게 설치한 뒤에 아래 커맨드를 이용해서 제대로 최신버전이 설치되었는지 확인합시다.

{% codeblock Shell lang:shell %}
git --version
{% endcodeblock %}

## 기초 설정

(추가 작성 예정...)
