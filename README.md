# html_css_js
html css javascript를 공부하는 곳

객체_1121

객체-함수 : Date().toLocaleString(); ----Date()는 객체이자 함수
객체-변수 : now.toLocaleString();   ----now는 객체이자 변수
----------------------------------------------------------------------괄호 유무

프로토타입 : 틀	----속성,특징들을 이미 갖고있고 정해져있음.
인스턴스 : 붕어빵	----복사품, 복제품
------------------------------------------------------------------------

인스턴스(now) 생성 ---------->함수에서 인스턴스를 생성할 수 있음.(now객체)
var now = new Date();


객체.함수
->객체에게 함수를 실행해라 (함수에는 "()")

random()은 0~1까지/floor는 인수보다 작거나 같은 수 중에서 가장 큰 정수를 반환
ex)1~50무작위 숫자 => Math.floor(Math.random( )*50+1)==0;

------------------------------------------------------------------------
메서드 : 객체가 어떻게 동작할지 선언해 놓은 함수
ex)Window객체에 들어있는 alert()함수 =메서드
	window.alert("안녕하세요?")->작동

-------------------------------------------------------------------------
객체 종류(3) : 내장객체, 문서객체모델(DOM), 브라우저 객체모델, 사용자 정의 객체
-------------------------------------------------------------------------
객체 만드는 법(2) : 객체 리터럴 표기법, 생성자 함수 이용

객체리터럴 표기법 = 객체선언 + 값 지정	
(객체 틀을 만들지 않고 개별적으로 객체를 선언하고 사용하는 방법)
ex)var book={
	title: 책먹는하마
	author: 나
	info: function( ) {
			alert(this.title +"는" + this.author + "가 저자입니다"); 
		        }
	};

(객체선언+값지정 -> var a = 10;)
		(속성이름 : 값)

=>book.title    입력하면 -> 실행
=>book.info( ) 입력하면 -> 실행
---------------------------------------------------------------------------
=>book.date = "2021" 입력하면 -> date속성과 값 추가


----------------------------------------------------------------------------

생성자 함수 이용

function ABC(A,B,C){
this.A = B;
this.B = A;
this.C = C;
}
->undefined
---------------
var e = new ABC('2','22','222');
->undefined
---------------
e
->ABC {A: '22', B: '2', C: '222'}
-------------------------------------------------------------------------------








X연습

for(var i=0; i<bookList.length; i++){
	document.write("<p>"+bookList[i].title+"<p>");
	}














------------------------------------------------------------------------------


*Date 객체

new Date( )			->현재 날짜

new Date("2021-02-19T16:00") 	->시간까지 설정
-> Fri Feb 19 2021 16:00:00 GMT+0900 (한국 표준시)
