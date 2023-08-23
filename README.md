# 230823 HOMEWORK #

🤍[MDN Basic HTML](https://developer.mozilla.org/ko/docs/Learn/Getting_started_with_the_web/HTML_basics)<br>
<br>

## HTML 기본 ##


#### 1. HTML 이란? ####
* 콘텐츠의 구조를 정으하는 마크업 언어.
* 콘텐츠의 서로 다른 부분들을 씌우거나 감싸서 다른 형식으로 보이게 하거나 특정한 방식으로 동작하도록 하는 __일련의 요소__로 이루어져 있다.


#### 2. HTML 요소 분석 ####

* **여는 태그** : 요소의 이름으로 구성. 요소가 시작하거나 효과가 시작하는 곳을 나타낸다.
* **닫는 태그** : 여는 태그 이름 앞에 '/'를 붙여 사용하며 요소의 끝을 나타낸다. 초보자가 흔히 닫는 태그를 쓰지 않는 오류를 범할수 있어 주의해야 한다.
* **콘텐츠** : 요소의 내용
* **요소** : 요소는 이렇게 여는 태그, 닫는 태그, 콘텐츠로 이루어져 있다.
요소는 속성도 가질수 있다.
* **속성** : 실제 콘텐츠로 표시되지 않으며 추가적인 정보를 담고 있다.
	* 속성이 항상 가져야 하는 것
		* 요소 이름(또는 요소가 하나 이상 속성을 이미 가지고 있다면 이전 속성)과 속성 사이에 공백이 있어야 한다.
		* 속성 이름 뒤에는 등호(=)가 와야 한다
		* 속성 값의 앞 뒤에 열고 닫는 인용부호(" 또는 ')가 있어야 한다.

ex)<br>
`<p ~~class="editor-note"~~>My cat is very cute.</p>`

이 예제에서 클래스 속성을 이용해 나중에 해당 요소를 특정해 스타일이나 다른 정보를 설정할 때 사용할 수 있는 식별자를 지정할 수 있다.


#### 3. 요소 중첩 ####

* 요소를 다른 요소의 안에 놓을 수 있다. 이를 __요소 중첩__ 이라 부른다.
* 요소는 겹치지 않게 안쪽이나 바깥쪽으로 열고 닫혀야 한다.

ex)<br>
`<p>My cat is <strong>very</strong> cute.</p>` (O)<br>
`<p>My cat is <strong>very cute.</p></strong>` (X)<br>


#### 4. 빈 요소 ####

* 어떤 요소들은 내용을 갖지 않는다. 이를 __빈 요소__ 라고 한다.

ex)<br>
`<img src="images/firefox-icon.png" alt="My test image" />`

* 이 요소는 두 개의 속성을 포함하고 있으나 닫는 태그가 없다.
* 이 요소의 목적은 페이지에서 이미지가 나타날 위치에 이미지를 넣는 것이며, 이미지 요소는 효과를 주기 위해 콘텐츠를 감싸지 않는다.

* `src` (source) 속성을 통해 이미지 파일의 경로를 포함한다.
* `alt` (alternative) 이미지를 볼 수 없는 사용자들을 위해 설명 텍스트를 넣을 수 있다.


#### 5. 문서해부 ####

* 각 요소들이 어떻게 전체 HTML 페이지를 구성하는지 살펴보겠다.<br>
ex)<br>
`<!DOCTYPE html>`<br>
`<html lang="ko">`<br>
`	<head>`<br>
`		<meta charset="utf-8">`<br>
`		<title>웹 페이지의 탭 부분</title>`<br>
`	</head>`<br>
`	<body>`<br>
`	브라우저에서 보여지는 부분`<br>
`	</body>`<br>
`</html>`<br>

* `<!DOCTYPE html>` : 문서 타입 정의 선언문(DTD). HTML문서 최상단에 선언하며 반드시 넣어줘야 한다. 브라우저가 올바른 화면표시(Rendering)를 하기 위해 필요
* `<head></head>` : 문서의 제목. 메타정보, 라이브러리 등 포함
* `<meta charset="utf-8">` : 문서의 언어 설정. 어떤 언어든 깨지지 않고 번역해주는 설정으로 반드시 작성해야 한다.
* `<title></title>` : 페이지의 제목 설정. 웹페이지의 Tab 부분에 보여진다.
* `<body></body>` : 브라우저에 보여지는 부분으로 웹 사용자들에게 모든 컨텐츠를 보여줄 수 있다.


