---
title: "마크다운 문법 정리 1"
excerpt: "마크다운에 대해 알아봅시다;)"
categories: 
  - Blog
tags:
  - [Blog,Jekyll,github.io,Markdown]
toc: true
toc_sticky: true
date: 2021-12-22
last_modified_at: 2021-12-28
---
<div style="line-height:150%;"><br></div>
# 마크다운(Markdown)

README.md는 Github을 사용하는 사람이라면 한 번쯤은 본 문서입니다. 바로 이 문서가 마크다운 문법으로 작성된 파일입니다. 지킬 블로그 또한 markdown을 이용합니다. 처음에는 마크다운 문법이 어렵게 느껴질 수 있으나, 익숙해지면 오히려 더 편하다는것을 알 수 있습니다.    

이 포스트에서는 마크다운 문법의 기본을 설명하려합니다 :)

# 1. 마크다운이란?   
> 마크다운이란 텍스트 기반의 마크업언어의 일종으로, 2004년 존그루버에 의해 만들어졌다. 마크다운 언어는 읽기도 쉽지만 쓰기도 쉽다는 장점이 있다. 확장자는 .md를 쓴다.

즉, 마크다운은 텍스트를 HTML로 변환하는 언어이자 도구입니다.   
마크다운에 대한 자세한 사용법은 [아래링크] 를 참조하기 바랍니다.   
- <http://daringfireball.net/projects/markdown>   

[아래링크]: http://daringfireball.net/projects/markdown


<div style="line-height:200%;"><br></div>

## 2. 마크다운 문법

## 2.1 문단(Paragraph)
문장의 집합을 문단이라고 한다. 한 문단과 다음 문단 사이는 빈 줄로 구분된다. 
 
------

## 2.2 제목(Header)
  - #의 갯수를 통해 제목을 나타낼 수 있습니다.    
  - \<h1>부터\<h6>을 통해 제목을 표현할 수 있습니다.   
  - 수가 커질수록 글씨는 작아집니다.   

```markdown
# 제목1	
## 제목2	
### 제목3	
#### 제목4
##### 제목5	
###### 제목6	
```
------


## 2.3 강조(Emphasis)
  - 볼드체(굵은글씨), 이탤릭체(기울림), 밑줄, 취소선을 나타낼 수 있습니다.   
  - \<strong>, \<em>, \<u>, \<del> 태그를 통해 나타낼 수 있습니다.

```markdown
1. 볼드체는 **별표** 혹은 __언더바__ 를 사용합니다.   
2. 이텔릭체는 *별표* 혹은 _언더바_ 를 사용합니다.   
3. ***이텔릭체* 와 두껍게**를 함께 사용할 수 있습니다.   
4. 취소선은 ~~물결~~을 사용합니다.   
5. <u>밑줄</u>은 `<u></u>`를 사용하세요.   
```

### 실행화면
1. 볼드체는 **별표** 혹은 __언더바__ 를 사용합니다.   
2. 이텔릭체는 *별표* 혹은 _언더바_ 를 사용합니다.   
3. ***이텔릭체* 와 두껍게**를 함께 사용할 수 있습니다.   
4. 취소선은 ~~물결~~을 사용합니다.   
5. <u>밑줄</u>은 `<u></u>`를 사용하세요.   

-----

## 2.4 목차(List)
  - 숫자나 문자를 통해 목차를 나타낼 수 있습니다.   
  - \<ol>,<ul> 태그를 이용하면 목차를 나타낼 수 있습니다.
  - 부호를 섞어서 사용하는 것도 가능합니다.

```markdown 
1. 순서 필요  
  - 순서가 불필요(서브)    
  - 순서가 불필요(서브)    
1. 순서 필요    
  1. 순서 필요(서브)     
1. 순서 필요   

- 순서가 필요하지 않은 목록에 사용 가능한 기호   
  - 대쉬(hyphen)   
  * 별표(asterisks)   
  + 더하기(plus sign)   
```

### 실행화면
1. 순서 필요  
  - 순서가 불필요(서브)    
  - 순서가 불필요(서브)    
1. 순서 필요    
  1. 순서 필요(서브)     
1. 순서 필요   

- 순서가 필요하지 않은 목록에 사용 가능한 기호   
  - 대쉬(hyphen)   
  * 별표(asterisks)   
  + 더하기(plus sign)   

-----


## 2.5 링크(Link)
  - \<a>로 링크를 나타낼 수 있습니다.   
  - [참조 링크] (실제 링크 url)로 나타냅니다.

```markdown
[GOOGLE](https://google.com)   
[NAVER](https://naver.com "링크 설명")   
[상대적 참조](../users/login)    
[GitHub][1]   

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

꺾쇠 괄호`< >`안의 URL은 자동으로 링크를 사용합니다.    
구글 홈페이지: https://google.com   
네이버 홈페이지: <https://naver.com>

[1]: https://github.com
[참조 링크]: https://naver.com "네이버!"
``` 	
### 실행화면   
[GOOGLE](https://google.com)   
[NAVER](https://naver.com "링크 설명")   
[상대적 참조](../users/login)    
[GitHub][1]   

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

꺾쇠 괄호`< >`안의 URL은 자동으로 링크를 사용합니다.    
구글 홈페이지: https://google.com   
네이버 홈페이지: <https://naver.com>

[1]: https://github.com
[참조 링크]: https://naver.com "네이버!"

-----


## 2.6 이미지(Image)
  - \<img>로 변환됩니다.
  - 링크과 비슷하지만 앞에 !가 붙습니다.

```markdown
![대체 텍스트 입력](https://ww.namu.la/s/980f49b2e0e9a61cffb43784f3e1794948170c230483639e351e1583a194130b2df40055e720be7b60885d1daf7a518d60c61d75d7d5d642c506c61fcb8d56a11cee44ec8ca63d64a2a5e0c90debc9282e263f75d1ef2f6362dc777f4795751e "링크 설명(title)")  

![Kayak][logo]

[logo]: https://w.namu.la/s/931ab90adf490022a84d162cff2b6235b5e7c5f3004f395ada954e17e9dab42b5f729ac87a0e49c6f071af32b09fcab4e9b268924722a9a01ae189844c7e4fb961cdec8d0a4da64b721c0f3d306931eaa481e7501f32637d9abd20ad823cf9aa6389e4d59b69b542b49776a28051a62f "Cute Minions"  
```
### 실행화면   
![대체 텍스트 입력](https://ww.namu.la/s/980f49b2e0e9a61cffb43784f3e1794948170c230483639e351e1583a194130b2df40055e720be7b60885d1daf7a518d60c61d75d7d5d642c506c61fcb8d56a11cee44ec8ca63d64a2a5e0c90debc9282e263f75d1ef2f6362dc777f4795751e "링크 설명")

![Kayak][logo]

[logo]: https://w.namu.la/s/931ab90adf490022a84d162cff2b6235b5e7c5f3004f395ada954e17e9dab42b5f729ac87a0e49c6f071af32b09fcab4e9b268924722a9a01ae189844c7e4fb961cdec8d0a4da64b721c0f3d306931eaa481e7501f32637d9abd20ad823cf9aa6389e4d59b69b542b49776a28051a62f "Cute Minions"