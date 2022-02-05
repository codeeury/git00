# HTML

## HTML Introduction

- HTML : Hyper Text Markup Language

  - Hyper Text : 하이퍼링크로 연결된 웹 문서 => 웹 문서(페이지)
  - Markup Language : 표시 언어

- HTML 표시 내용

  - Web Page의 Contents
    - Text Contents
    - multimedia Contents : image, video, audio (media contents)
      - Embeded Contents
  - Web Page의 Structure

- 학습내용
  - 문법:
  - 활용:

## HTML Basic

-기본구조
※ ` : backtick

```
<!doctype html>
<html>
  <head>
  웹 문서의 부가정보
  </head>
  <body>
  웹 문서의 내용
  </body>
</html>
```

## HTML Element

-Tag와 Contents로 구성
-Tag는 시작태그와 종료태그로 구성
-contents와 종료태그 없이 시작태그만 있는 요소 : 빈요소(Empty Element)

```
<h1>제목</hi>

<br> => 빈 요소(empty elmement)
```

## HTML Attribute

- HTML Tag의 추가정보
- syntax : name="value"

```
<img src="sakdjf.jpg" alt="사진">
```

## Text Contents Element

### Heading

- 제목
- h(heading)
  - H1 ~ H6

### paragraph

- p (paragraph) : 단락
- hr(horizontal rules) : 수평선 (단락을 구분)
- br(line break) : 강제 줄바꿈
  (※) 강제 공백 ; \$nbsp; - Non breaking space)
  - HTML Text : 줄바굼, 공백 인식
    - 공백 1칸으로 인식

### HTML List

- 순서없는 목록 : ul, li
- 순서있는 목록 : ol, li
- 설명 목록 : dl, dt, dd

※ 포함관계 / 중첩관계 (Nested Element)

- 포함하는 요소: 부모(parent) 조상(ancestor)
- 포함되는 요소: 자식(child) 자손(decendant)
- 이웃하는 요소: 형제(sibling)

### HTML Link

- 하이퍼링크 연결

- a(anchor)
  -href(hypertext reference) attribute : 연결되는 페이지의 주소 정보
  -target attribute : \_black 새탭열기 설정
  target="\_blank"

- Bookmark 기능
  - 목적지에 id attribute을 사용해서 이름 지정
  - a 태그의 href 속성에 "#이름"으로 위치 표시

### HTML Table

- 표를 표시
- table(표의 영역을 표시)
- tr(table row) : 행
- th(table heading) : 열 제목(칸)
- td(table data) : 열(칸)
- table generator
  https://www.tablesgenerator.com/html_tables

## Multimedia Contents

### HTML image

- img : image
- attribute
  - src(source) : 이미지의 파일 경로, ,이름
  - alt(alternative) : 대체 텍스트

## HTML Video

-video tag
-attribute(name만 사용하는 형태)

- controls : 동영상 컨트롤 버튼 표시 여부
- autoplay : 자동 재생
- muted : 음소거
- loop : 반복 재생
- poster:

## semantic element

- 영역을 구분하는 element를 의미있게 사용하는 것

- header : 로고, 로그인/회원가입, 언어변경
- nav(navigation) : 메뉴(GNB-global navigation bar / lnb)
- section : 웹 페이지의 본문 / 영역 구분
- article : 웹 페이지의 본문 / 독립된 글 / 내용
- aside : 부수적인 내용 / 광고 배너
- footer : 웹 사이트의 위치 정보 / 관련 링크
- figure : 다이어그램/ 이미지 시각 요소
- main : 웹 페이지 본문 전체

## URL / File path

- URL (Uniform Resource Locator)

```
https://www.naver.com/video/movie.mp4

=>https://도메인네임/상세경로:포트번호

IP 주소 : Internet Protocol 주소 =>인터넷에서 사용하는 실제 주소

Ex)192.168.0.1: 0에서 255까지의 숫자 4개로 구성

도메인 네임: 영어 단어(줄임말)로 구성되어 있는 식별 이름

도메인 네임 서버(시스템) : 도메인 네임 => IP주소로 변환

```

- 경로 지정 방식
  - root : 해당 경로의 가장 기본 위치
  - 절대 지정 방식
    - 파일 경로의 전체 URL을 표현하는 방식
  - 상대 지정 방식 -현재 페이지를 기준으로 일부 URL을 표현하는 방식
    -root 상대 경로 방식 : root를 기준으로 상대적인 URL 표현

```
domain : www.abc.com

/(root) - html - index.html
        - images - photo.jpg

절대방식 : https://www.abc.com/images/phoo.jpg

상대방식 (현재페이지 : index.html) : (../)../images/photo.jpg

root 상대방식 : /images/photo.jpg
```

## HTML Head

- head element

  - title : 웹사이트 제목 (브라우저 탭에 표시)
  - meta : 웹사이트 관련 정보
  - link : css
  - script : javascript

- meta
  -charset(character set) : 문자 세트 - 글자(문자)를 표시하는 방법 -종류/개수 =>용량

  - bit : 0/1이 저장되는 공간
  - 1 bit가 저장/표현할 수 있는 개수(가짓수): 2
  - 2 _ 2 _ 2 \* 2 => 4 bit => 16개
  - 1 byte = 8 bit (byte < kb < mb <tb <pb) 1000배수

* UTF-8 :글자 표기 방식 중 하나
  -2 byte로 글자를 표시 (65536) : 유니코드 -영문 1byte로 표현, 한글은 2byte로 표현
  -UTF(Universal Coded Character Set + Transformation Format - 8-bit)

* EUC-KR : 한글, 영문 전용 표시 방식

## HTML Block & Inline

- Block -줄바꿈 되어 새 줄에 표시됨 -블럭요소는 너비가 가능한 전체가 채워짐 -줄바꿈 되어 새 줄에 표시됨
  -text, 블럭요소, 인라인요소 모두 포함할 수 있음

- Inline -줄바꿈 되지 않고 한 줄에 표시됨 -너비가 콘텐츠/ 자식 요소에 맞춰짐
  -text, 인라인요소 포함할 수 있음()

- div(division)

  - 단순히 영역을 구분하거나 그룹핑을 하는 컨테이너 요소
  - 블럭요소

- span -단순히 영역을 구분하거나 그룹핑을 하는 컨테이너 요소

```
<p class="">...</p>
<p id="">...</p>
<p>...</p>
```

- naming 표기법
- 네이밍할 때 영어 한개 단어로만 네이밍을 하기 힘들기 때문에 여러 단어를 연결해서 네이밍
- 연결되는 단어를 구분할 수 있도록 표기

```
hello world : 일반 표기

네이밍
hello_world : snake (파일명)
hello-html-world : kebab case (URL-폴더, class/id 이름)
helloHtmlWorld : camel case (js  - 변수 / 함수 이름)
HelloHtmlWorld : Pascal case (js - class 이름 )

```

#CSS

## CSS Introduction / Syntax

- cascading Style Sheet
- 여러개의 html 파일에 공통 적용

```
선택자 {

}

```
