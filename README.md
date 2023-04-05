# WEB_JavaScript

### 2023.04.05 ~ 2023.04.06
***
* 사용자와 동적으로 상호작용하는 웹페이지
* 기본적으로 JavaScript는 HTML 위에서 동작하는 언어
* 웹은 HTML을 이용해서 웹페이지를 우선 만든 후에, 그 웹페이지를 JavaScript를 이용해 사용자와 상호작용할 수 있도록 기능을 추가함으로써 HTML의 정보와 JavaScript의 기능을 모두 갖추게 됨
* 프로그램처럼 사용자와 상호작용하면서도 검색엔진을 통해서 검색된다는 것은 웹만의 독창적인 특성
***
첫번째 실습
1. <태그명:script>JavaScript를 넣는 방법, 웹브라우저한테 HTML의 코드로 지금부터 JavaScript가 시작됨을 알려주는 태그<태그명:/script>

* HTML 문법과 JavaScript 문법의 차이점: JavaScript는 동적 -> ex) HTML로 1+1이라고 작성하면 그대로 보여주는 반면, JavaScript로 작성 시 계산한 결과(사칙연산 가능)를 알려줌
***
두번째 실습
1. <태그명:input type="button" value="hi" onclick="alert('hi')">: hi라는 버튼을 만들고 버튼을 누르면 hi라는 경고창을 띄어주는 태그
=> 즉, hi라는 버튼을 누르면 onclick에 저장된(JavaScript 문법으로 작성된) 속성값을 실행함
2. <태그명:input type="text" onchang="alert('changed')">: 네모 안에 text 입력 가능하고 text 내용이 변하면 changed라는 경고창을 띄어주는 태그
3. <태그명:input type="text" onkeydown="alert('key down!')">: 네모 안에 text 입력 가능하고 아무 key나 누르면 key down!이라는 경고창을 띄어주는 태그
***
* 웹브라우저에서 일어나는 일을 '이벤트'라고 함 -> '어떤 이벤트가 일어났을 때 어떠한 JS가 실행되도록 하는 것' 중 onclick, onchange, onkeydown 등이 있음
* 웹브라우저는 웹브라우저 위에서 일어나는 여러 사건 중에 기념할만한 약 10~20개 정도의 이벤트를 정의해놓고 있음
* 그런 이벤트를 이용해 사용자와 상호작용하는 코드를 만들 수 있음
***
세번째 실습
1. 콘솔(Console): JavaScript를 실행하기 위해 파일을 만들지 않고 즉석으로 실행시키는 방법 -> 웹페이지-오른쪽 마우스-검사-콘솔
2. 콘솔에 '문자열'.length 입력 시 바로 결과값 확인 가능 or alert('문자열'.length) 사용하면 웹페이지에 경고창으로 결과값 띄우기 가능
3. 콘솔에서 실행시키는 JS는 해당 웹페이지 안에 삽입된 JS인 것처럼 동작
***
네번째 실습
1. Number(숫자)라고 하는 데이터 타입이 있고, 산술 연산자에 +, -, *, / 등이 존재
2. String(문자열)이라고 하는 데이터 타입이 있고, 적을 때 따옴표(" ", ' ')로 묶어줘야 함
3. String에 많은 기능이 있음 -> ex) length, toUpperCase(), IndexOf('찾길 원하는 문자열'), trim 등... 
***
다섯번째 실습
1. 변수는 값이 바뀔 수 있음, '='은 대입 연산자
2. 1, 2, 3, ... 등은 바뀌지 않는 상수
3. 변수를 선언할 때 var 같이 써주기 -> ex) var name = 'soobin';
***
* 콘솔에서 실행을 유보하고 싶을 때는 shift+enter
***
여섯번째 실습
1. style 속성의 속성값으로는 CSS라는 컴퓨터 언어가 와야 함 -> 디자인 역할
2. <태그명:body style="background-color:black; color:pink;">: body 부분의 배경은 black, 글씨는 pink로 디자인
***
일곱번째 실습
1. <태그명:태그 style="속성:속성값;">: CSS 기본 문법
2. <태그명:div>CSS or JS를 통해서 어떤 정보를 제어하고 싶을 때 해당 정보들을 감싸주는 역할의 무색무취 태그, 전체사용(줄바꿈O)<태그명:/div>
3. <태그명:span>CSS or JS를 통해서 어떤 정보를 제어하고 싶을 때 해당 정보들을 감싸주는 역할의 무색무취 태그, 해당부분사용(줄바꿈X)<태그명:/span>
4. head 태그 안에 <태그명:style>태그명 {속성: 속성값;}<태그명:/style> 라고 작성하면 body 태그 안에 있는 해당 부분의 CSS 문법을 한번에 제어 가능
5. elements는 태그명 바로 쓰면 되고, class는 이름 앞에 '.'을 붙이고, id는 '#'을 붙임
6. 우선순위: id > class > element -> 즉, id는 예외적인 처리를 주고싶을 때 사용!
***
여덟번째 실습
1. JS 문법에 따라서 동적으로 웹브라우저가 body 태그를 선택하게 하려 함
=> ex: 다크모드 버튼, *주의할점: CSS와 속성 이름 다를 수 있으므로 JS 문법에 맞게 작성!
<태그명:input type="button" value="night" onlick="
document.querySelector('body').style.backgroundColor = 'black';
">
***
* JavaScript는 컴퓨터 프로그래밍 언어, HTML은 아님
***
아홉번째 실습
1. JS에서 Boolean을 만들어내려면 ===, <, > 사용
2. HTML에선 '<' 대신 &lt; 사용
3. if 문의 괄호 안에는 boolean이 옴
***
열번째 실습
1. if문에 조건을 설정함으로써 하나의 버튼으로 다크모드 생성 가능
=> <태그명:input id="night_day" type="button" value="night" onclick="
    if(document.querySelector('#night_day').value === 'night') {
        document.querySelector('#night_day').value = 'day';
        document.querySelector('body').style.backgroundColor = 'black';
        document.querySelector('body').style.color = 'white';
    } else {
        document.querySelector('#night_day').value = 'night';
        document.querySelector('body').style.backgroundColor = 'white';
        document.querySelector('body').style.color = 'black';
    }
    ">
***
열한번째 실습
1. 리팩토링: 불필요한 중복 등을 제거하여 효율성 있는 코드로 다시 만드는 것
2. 어떤 Event가 속해 있는 태그 자신을 가리키는 것 = this
3. 변수로 지정할 수 있다면 해주기
=> 코딩 잘하는 팁: 중복을 끝까지 쫓아가서 제거
***
열두번째 실습
1. 배열 선언: var arr = ["a", "b", "c"];
2. 배열 멤버 얻을 때는 arr[0]으로 지정
3. push, pop 등으로 배열에 멤버 넣거나 뺄 수 있음
4. 길이 알고 싶다면, .length 사용하면 됨
***
열세번째 실습
1. 반복문의 기본 문법: while(true){ 코드; }
* 반복문은 순서대로 실행되는 프로그램의 실행 순서의 흐름을 제어하는 제어문이라고 할 수 있음 (조건문도 마찬가지)
***
* 문자열, 태그, 속성값 등등 문법에 잘 맞춰 쓰기!
***
열네번째 실습
1. querySelector 메소드는 해당하는 선택자 하나만 가져옴
2. querySelectorAll 메소드는 해당하는 선택자 모두를 배열로 가져옴
3. 선택자.style.color = '색깔이름"으로 하면 해당 코드가 실행되면 text 색이 바뀜
***
열다섯번째 실습
1. 함수 선언법: function 함수명() { 코드; }
***
열여섯번째 실습
1. 중복이 여러번 발생하지만 반복문으로 처리할 수 없는 경우 -> 함수 필요
2. argument: 함수로 전달하는 인자
3. parameter: argument를 받아서 함수 안으로 매개해주는 변수
4. 함수 선언 시 parameter 쓸 때는 'var' 붙일 필요 없음 -> ex: function sum(a, b)
5. 함수에서 return을 활용하면 원자화된 기능을 다양한 맥락에서 사용할 수 있도록 자유도가 생기게 됨
***
* 리팩토링 수단 중의 하나가 "함수"
* 함수의 매개변수로 "self"를, 인자로 "this" 사용해야 하는 경우 있음
***
* 의미가 불명확하거나 시간이 지나 어떤 의미인지 파악하기 어려운 코드라면 한줄이라도 함수를 통해 그 로직에 이름을 부여하는 것도 좋은 전략
* 객체를 폴더라는 관점으로 봐도 괜찮음
* 객체의 예로는 document 등이 있고, 객체가 사용하는 함수를 method라고 함
* 순서 없이 정보를 저장할 수 있는 것이 "객체" -> 즉, 객체는 이름이 있는 정리정돈 상자!
(* 순서 있게 정보를 저장하는 것은 "배열")
***
열일곱번째 실습
1. 객체를 만들 때 사용하는 기호를 object literal이라고 함
2. 객체 선언법: var 객체명 = { "key":"value", "key":"data", ... };
ex) var coworkers = {
	"programmer":"egoing",
	"designer":"leezche"
     };
3. 만들어져있는 객체에서 데이터를 가져오려면 => coworkers.programmer로 사용하면 됨
3. 객체 추가 예시: coworkers.bookkeeper = "duru";
4. 객체의 이름에는 공백을 넣을 수 없음 => 넣고 싶다면 coworkers.data scientist 대신 coworkers["data scientist"] 사용!
5. 객체에서 반복문 사용법: for(var key in coworkers) { 
			 document.write(key+'<br>');
  			 document.write(coworkers[key]+'<br>');
		          }
6. 객체에 함수(method)를 담는법: coworkers.showAll = function() { 코드; }
또는 객체 선언 시에, showAll:function(){ 코드; }; 으로 포함할 수도 있음
(* 함수를 var showAll = function() { 코드; } 라고 정의할 수도 있음)
7. 객체에 method를 담을 때 그 method가 속한 객체를 가리키는 기호 = "this"
8. 객체에 소속된 변수(ex: programmer, designer)는 "property", 함수(ex: showAll)는 "method"라고 함
***
열여덟번째 실습
1. 서로 연관된 코드들은 파일로 묶어 그룹핑 -> 가장 큰 정리정돈 도구라고 생각할 수 있음
2. script 태그 안의 코드를 js 파일로 따로 만든 후, 다른 파일에서 이것을 <태그명:script src="파일명.js"><태그명:/script>로 쓰면 같은 효과
=> ex) color.js 파일 생성, main.html 파일에서 <태그명:script src="color.js"><태그명:/script>로 사용
***
* 라이브러리: 재사용하기 쉽도록 되어 있는 소프트웨어
* 프레임워크: 만들고자 하는 것이 무엇이냐에 따라 공통적인 부분은 프레임워크가 만들어놓고, 다른 부분은 수정을 통해 만듦 즉, 거의 반제품과 같은 것
=> 둘 다 다른 사람과 협력하는 모델!
***
열아홉번째 실습
1. jQuery 라이브러리 사용법: jQuery CDN->코드 복사(script src 형식)->프로젝트의 원하는 파일에 붙여넣기 or jQuery 파일 다운로드->프로젝트 폴더 디렉토리로 이동시킴
=> ex: $('태그명').css('color', color)
=> jQuery는 새로운 언어가 아니라 사용자 대신 css라는 함수를 만들어 둔 것!
***
* 주석 처리: ctrl + /
***
* UI: User Interface, 사용자가 시스템을 제어하기 위해서 사용하는 조작 장치
* API: Application Programming Interface, 애플리케이션을 만들기 위해서 프로그래밍을 할 때 사용하는 조작 장치 -> ex: alert(경고창)
(* API와 순서는 서로 떼려야 뗄 수 없는 관계)
***
* 웹페이지에 있는 어떤 태그를 삭제하거나 자식 태그를 추가하고 싶다면 -> document(DOM) 객체를 자세히 살펴보기
* 웹페이지가 아닌 웹브라우저 자체를 제어해야 한다면 -> window 객체를 살펴보기
* 웹페이지를 reload하지 않고 정보를 변경하고 싶다면 -> ajax, 현대적인 웹앱을 만드는 데 필수적인 테크닉
* 웹페이지가 reload되어도 현재 상태를 유지하고 싶다면 -> cookie, 사용자를 위한 개인화된 서비스
* 인터넷이 끊겨도 동작하는 웹페이지를 만들고 싶다면 -> offline web application
* 화상통신 -> webRTC
* 음성 인식 -> speech
* 3차원 그래픽, 게임 -> webGL
* 가상현실 -> webVR
