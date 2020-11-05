# block element

```
한 줄에 하나의 요소만 포함할 수 있는 html 요소
Ex) address, article, aside, audio, blockquote, canvas, dd, div, dl, fieldset, figcaption, figure, footer, form, h1-h6, header, hgroup, hr, noscript, ol, output, p, pre, section, table, ul, video

```

- 기본 너비값 : 100% (form element 제외), **width 옵션은 무시된다.**
- 너비값, 높이값 가질 수 있음
- 상하좌우 모든 마진 가질 수 있음

# Inline element

```
한 줄에 여러 요소를 포함할 수 있는 HTML 요소
ex) img, br, sub, span, input, label, a, button, b, l, s
a, abbr, acronym, b, bdo, big, br, button, cite, code, dfn, em, i, img, input, kbd, label, map, object, q, samp, small, script, select, span, strong, sub, sup, textarea, tt, var

```

- 기본 너비값 : 컨텐츠 너비값
- 너비값, 높이값 가질 수 없음(**폼 엘리먼트, 이미지 제외**)
- 상하 마진 가질 수 없음(**이미지 제외**)

# 속성 설정.

block과 inline의 속성을 변환시키려면 display 를 사용할 수 있다.

```css
div {
  display: inline;
}
```
