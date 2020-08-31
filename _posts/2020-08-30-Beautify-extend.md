---
layout: post
title: vscode 코드정렬
comments: true
category: Blog
tags: vscode Prettier플러그인 자동줄정렬
---

## vscode 자동 코드정렬

- vscode 기본 코드정렬 단축키가 있다

<img src="https://switch-coder.github.io/public/imgs/vscode_sort1.jpg" class="img">

- 위 코드를 정렬해 보겠다. 우선 ctrl + a 를 눌러 전체 선택을 한다.

- 전체 선택이 됐으면 ctrl 을 누른 상태에서 k 를 누른후 f 를 누르면 된다

<img src="https://switch-coder.github.io/public/imgs/vscode_sort2.jpg" class="img">

- 위 그림과 같이 정렬되는것을 확인 할 수 있다

## vscode prettier extension 자동 코드정렬

- 1.prettier 설치

<img src="https://switch-coder.github.io/public/imgs/prettier_extension_install.JPG" class="img">

- 2.prettier 설정

<img src="https://switch-coder.github.io/public/imgs/vscode_setting.png" class="img">

- 왼쪽 하단 톱니바퀴 버튼을 누른후 settings 를 눌러 설정창에 들어간다.

<img src="https://switch-coder.github.io/public/imgs/prettier_setting.JPG" class="img">

- 설정 검색창에 editor format on save 를 검색해서 format on save 부분을 체크해준다.

<img src="https://switch-coder.github.io/public/imgs/prettier_setting2.jpg" class="img">

- 다시 검색창에 json을 입력후 edit in settings.json 클릭한다.그러면 settings.json 파일이 열린다

<img src="https://switch-coder.github.io/public/imgs/prettier_setting3.JPG" class="img">

- editor.formatOnSave 부분이 true 로 되어있는지 확인한다. 만약 false면 true로 바꿔준다.
  이렇게 준비는 끝났고 정렬되는 부분을 보여주겠다.

<img src="https://switch-coder.github.io/public/imgs/prettier_test1.JPG" class="img">

- 위와 같이 테스트 코드를 작성해 보았다. 여기서 ctrl + s (저장) 버튼을 눌러 보았다.

<img src="https://switch-coder.github.io/public/imgs/prettier_test2.JPG" class="img">

- 위와 같이 코드가 자동으로 정렬되는 것을 볼 수 있다.
