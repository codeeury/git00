# HTML

## HTML Introduction

- HTML : Hyper Text Markup Language

  - Hyper Text : 하이퍼링크로 연결된 웹 문서 => 웹 문서(페이지)
  - Markup Language : 표시 언어

- HTML 표시 내용

  - Web Page의 Contents
    - Text Contents
    - multimedia Contents : image, video, audio (media contents)
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
(※) 강제 공백 ; $nbsp; - Non breaking space)
  - HTML Text : 줄바굼, 공백 인식
    - 공백 1칸으로 인식

### HTML List

- 순서없는 목록 : ul, li
- 순서있는 목록 : ol, li
- 설명 목록 : dl, dt, dd

※ 포함관계 / 중첩관계 (Nested Element)