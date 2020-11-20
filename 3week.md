## 제이쿼리 개요
- 자바스크립트 명세방법
    - 자바스크립트 코드는 <script> 태그안에
- 내용과 코드를 분리
- DOM(Document Object Model)
- 기본 기능
    - core
    - selector
    - css
    - traversing
    - manipulation
    - attributes
    - events
    - ajax
    - ui
---
## 제이쿼리 함수
- `jQuery()` 함수의 3가지 입력 인자 유형
    - 선택자 입력 인자
```js
jQuery('body p');
```
    - HTML 입력 인자
```js
jQuery('<h1> HTML 동적 추가 </h1>').appendTo('body');
```
    - 함수 입력 인자
```js
jQuery(function() { alert("DOM");});
```
---
## 제이쿼리 선택자
- 기본 선택자
    - * : $('*')
    - 태그명 : $('div'), $('h1, h3, p')
    - 아이디 : $('#id1'), $('div#id1')
    - 클래스 : $('.class1'), $('div.class1'), $('.class1.class2')
- 계층 선택자
    - 선택자 > 자식선택자 : 바로 밑에 위치한 하위 엘리먼트
    - 선택자 자손선택자 : 안에 포함된 모든 하위 엘리먼트
    - 선택자 + 형제선택자 : 특정 엘리먼트 바로 다음에 나오는 특정한 형제 엘리먼트
    - 선택자 ~ 형제선택자 : 특정 엘리먼트 다음에 나오는 모든 형제 엘리먼트
- 속성 선택자
    - 선택자[속성명] : 해당 속성을 포함하는 엘리먼트
    - 선택자[속성명="조건값"] : 일치하는 엘리먼트
    - 선택자[속성명*="조건값"] : 포함하는 엘리먼트
    - 선택자[속성명^="조건값"] : 조건값으로 시작하는 엘리먼트
    - 선택자[속성명$="조건값"] : 조건값으로 끝나는 엘리먼트
- 위치필터 기본 선택자 : 첨자가 0부터 시작
    - 선택자:first
    - 선택자:last
    - 선택자:odd
    - 선택자:even
    - 선택자:eq(n)
    - 선택자:lt(n)
    - 선택자:gt(n)
    - 선택자:not()
- 위치필터 계층 선택자 : 첨자가 1부터 시작
    - 선택자:first-child   -> 선택된 엘리먼트 중에서 부모의
    - 선택자:last-child
    - 선택자:nth-child(odd)
    - 선택자:nth-child(even)
    - 선택자:nth-child(n)
    - 선택자:nth-child(Xn+y)
    - 선택자:only-child
- 폼 필터 선택자
    - 선택자:input
    - 선택자:button
    - 선택자:text
    - 선택자:checkbox
    - 선택자:radio
    - 선택자:file
    - 선택자:image
    - 선택자:password
    - 선택자:submit
    - 선택자:reset
- 상태 필터 선택자
    - 선택자:selected
    - 선택자:checked
    - 선택자:enabled
    - 선택자:disabled
    - 선택자:visible
    - 선택자:hidden
    - 선택자:focus
    - 선택자:animated
- 내용 필터 선택자 : has(), contains(), empty, parent
- 