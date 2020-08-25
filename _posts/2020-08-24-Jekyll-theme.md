---
layout: post
title:  깃허브 페이지에 Jekyll 테마 적용시기키
comments: true
category: Blog
tags: jekyll theme github.io github
---

jekyll 테마를 깃헙페이지에 적용시키는 방법을 알아 보겠습니다.  
 * 운영체제는 윈도우에서 진행 하였습니다.

## 1. Jekyll 설치하기
 + 터미널을 실행시킨다  

 + repository 폴더를 만들 위치로 이동한다

 + reopsitory 를 클론해준다  

```java
    git clone (자신의 repositiory url)

```    

<img src="https://switch-coder.github.io/public/imgs/jekyll_install1.JPG" class="img">   
<!-- 터미널  사진 -->

 + clone이 완료됬으면 해당 폴더로 들어간다.  
 ```java
    cd 자신이 만들 repository 이름

```  
<img src="https://switch-coder.github.io/public/imgs/jekyll_install2.jpg" class="img">   

 + 이제 jekyll을 설치한다   


 ```java

    ruby -v
    //루비 버전을 확인해본다. 2.3 버전 이상이면 가능하다

    gem install jekyll

    jekyll new ./ --forece

    jekyll serve
    // Server address: http://127.0.0.1:4000/

 ```    


 + 여기까지 완료 됐으면 크롬에 http://127.0.0.1:4000/ 입력해 들어가본다

<img src="https://switch-coder.github.io/public/imgs/jekyll_install4.jpg" class="img">   

+ 위 화면이 나온다면 jekyll 성공적으로 설치된것을 확인할 수 있다

## 2. 테마 적용시키기

+ 우선 적용시킬 테마를 찾아야 하는데 나는 [Jekyll Theme](http://http://jekyllthemes.org/“Jekyll theme”)에서 찾았다. 

<img src="https://switch-coder.github.io/public/imgs/jekyll_theme1.JPG" class="img">   
<img src="https://switch-coder.github.io/public/imgs/jekyll_theme2.JPG" class="img">   
 
+  내가 선택한 테마는 위 테마이다.   

+ 본이이 원하는 테마를 찾았다면 다운 받고 압축을 풀어준 후 아까 clone한 폴더에 풀어준 내용물들을 넣어준다.  

+ 그러면 아래와 같이 보인다면 이제 거의 끝났다.   

<img src="https://switch-coder.github.io/public/imgs/jekyll_theme3.JPG" class="img">    

+ 깃허브에 올리기 전 .gitignore , _config.yml 파일을 수정해줘야 한다

```t
#Ignore docs files
vendor

# Jekyll stuff
/_site/
_site/
.sass-cache/
.jekyll-metadata
.jekyll
Gemfile
Gemfile.lock
.jekyll-cache

```  
+ .gitignore 파일에는 위와 같이 코드를 추가해준다

<img src="https://switch-coder.github.io/public/imgs/config_yml.JPG" class="img">    
+ _config.yml 파일에는 위에 빨간 동그라미안에 true 에서 false 로 사진과 같이 변경해주면 된다

+ 추가하고 저장했으면 
+ 다시 터미널로 돌아가 코드를 입력해준다  


```t
    git add *
    
    git commit -m "jekyll 테마 카피"

    git push

```  

+ 깃허브 페이지 들어가 제대로 작동하는지 확인한다.  

+ 만약 적용되지 잘 적용되지 않았다면 url / css 경로등이 정확하게 입력 되었는지 확인해봐야 한다.  

+ 여기까지 jekyll 설치와 테마적용 방법에 대해 알아봤다.  
+ 수정 확인
