# Sass Guide

- Sass 설치<br>
  http://wit.nts-corp.com/2015/01/09/2936

- 이클립스 syntax color 셋팅 <br>
  http://stackoverflow.com/questions/7614612/is-there-an-eclipse-editor-for-sasss-scss-files-or-syntax-coloring-plugin

- Sass 출력 스타일 <br>
  압축 (compressed) 스타일 사용 <br>
  명령어
  ```bash
  sass --watch --style compressed a.scss:a.css
  ```
  - normal(기본) - 25,047 bytes <br>
  - compact(축약) - 28,030 bytes <br>
  - `compressed (압축)` - 23,986 bytes

- sass 문법 설명 <br>
  들여쓰기, 주석, 기호(&, >) 등

- 크롬 연동 <br>
  http://blog.remotty.com/blog/2015/07/27/sass-debug-with-chrome/

- 변환 사이트 <br>
  http://csstoss.com/

## Sass Convention
##### 경로 및 파일명
/resources/scss/scss_a.scss (파일찾기 쉽게하기 위해 scss_ 접두사 사용)
```bash
  sass --watch --style compressed scss_a.scss:../css/a.css
  ```
##### 들여쓰기는 2칸
```sass
// X
.box{
    ... 
}
  
// O
.box{
  ... 
}
```
-
##### 주석
```sass
// X
// 주석입니다. (문법은 가능하나 이클립스 syntax color가 불안정함)
  
// O
/* 주석입니다. */
```
