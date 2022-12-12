
# HTML+CSS

헤더 바디가 없으면 그냥 바디로 인식
html 없는 태그면 없는거랑 같다
엔테티 코드 특수문자
여러개 연속적인 화이티 캐릭터는 한칸으로 취급
pre는 그대로 출력   

># CSS 3가지 박스 유형 비교
|인라인 박스(display:block)|인라인 박스(display:inline)|인라인 블록 박스(display:inline-block)|
|---|---|---|
|항상 새라인에서 시작|새라인에서 시작 못함 라인안(inline)에 있음|새라인에서 시작 못함 라인안(inline)에 있음|
|블록박스 내에만 배치|모든 박스 내 배치|모든 박스 내 배치|
|옆에 다른 요소 배치 불가능|옆에 다른 요소 배치 가능|옆에 다른 요소 배치 가능|
|width와 geight으로 크기 조절|width와 height으로 크기 조절 불가능|width와 geight으로 크기 조절|
|padding, border, margin조절 기능|margin-top, margin-bottom조절 불가능|padding, border, margin조절 불가능|

># POSITION
|속성|속성값|설명|
|---|---|---|
|정적배치|static|요소를 문서의 흐름에 맞추어 배치. 위치지정이 필요없음|
|상대배치|relative|이전요소에 저연스럽게 연결해 배치하되 위치를 지정할 수 있음|
|절대배치|absolute|원하는 위치를 지정해 배치|
|고정배치|fixed|지정한 위치에 고정해 배치. 화면에서 요소가 잘릴 수도 있다|

인라인태그  
+ 내용과 앞뒤 태그의 내용을 같은 라인에 출력
+ 내용물의 크기가 태그의 영역이 된다.
+ 정해진 역할 X
+ 인라인태그는 자식으로 또다른 인라인태그만 올 수 있다

블럭 태그 
* 다른 라인에 출력
* 내용물의 크기와 상관없이 너비는100%고정 높이는 내용의 크기에 맞춤
* 자신의 내용만으로 한 라인을 독점해서 출력
* 영역(구조)을 만들때 사용 > 컨테이너 역할 > 레이아웃 구성(틀 만들기)
* 블럭 태그는 자식으로 또다른 블럭 태그 or 인라인 태그를 가질 수 있다.

blank
* 새 윈도우 창을 열어서, 웹페이지를 연다	. 
* 기존의 창은 그대로 남겨져 있다.

self 
* 현재 윈도우창에 그대로, 링크된 웹페이지를 연다. ( 현재의 프레임 )

parent 
* 현재 프레임의 부모 프레임에서 새웹페이지가 열린다 .만약 어떤 창 A에서 창 B를 새로 열었습니다. 그런데 창 B에서 _parent로 창을 열면 창 A에서 열리게 된다.

top 
* 최상위 프레임에서 열립니다. _parent와 비슷하다.  _parent는 바로 이전창(부모창)에서 열리는 반면_top은 최상위( 가장 최고 부모)창에서 열린다.

form
* 사용자로부터 데이터를 입력 받기 위한 페이지
```
<form>
.
form elements
.
</form>
```   
required 
* 속성 뿐이지만 브라우져는 필수 입력으로 알고 값을 검증한다. 사용자가 올바로 입력하고 제출하기 버튼을 클릭한다면 기대한 것처럼 서버로 폼을 전송한다.

```
.<input type email>
.<form>
  .<!-- required 속성을 추가했다 -->
  .<input name="email" required />
  .<button type="submit">제출</button>
.</form>
```   

셀럭터 css 스타일 시트를 html 페이지에 적용하도록 만든 이름
html 태그의 모양을 꾸밀 스타일 시트를 선택하는 기능

한개 이상을 지정할때 class
한개만 지정할때 id

margin 바깥
padding 안쪽 여백   
  
z-index 속성은 위치 지정 요소와, 그 자손 또는 하위 플렉스 아이템의 Z축 순서를 지정합니다. 더 큰 z-index 값을 가진 요소가 작은 값의 요소 위를 덮습니다.  
```
/* 키워드 값 */
z-index: auto;

/* <integer> 값 */
z-index: 0;
z-index: 3;
z-index: 289;
z-index: -1; /* 음수 값으로 우선순위를 낮출 수 있음 */

/* 전역 값 */
z-index: inherit;
z-index: initial;
z-index: unset;
```   
visibility
overflow   

부드러운 스크롤 효과 추가   
```
html {
  scroll-behavior: smooth;
}
```   
order속성은 동일한 컨테이너 내의 나머지 유연한 항목에 상대적인 유연한 항목의 순서를 지정합니다
```order: number|initial|inherit;```   
align-self속성은 유연한 컨테이너 내에서 선택한 항목의 정렬을 지정합니다. align-self속성은 유연한 컨테이너의 align-items 속성을 재정의합니다.   
```align-self: auto|stretch|center|flex-start|flex-end|baseline|initial|inherit```

----------------------------------------------------

# Javascript

스크립트는 바디 제일 아래쪽에 있는편이 좋습니다.

변수 선언에는 기본적으로 const를 사용하고, 재할당이 필요한 경우에 한정해 let 을 사용하는 것이 좋다.
Var : 중복 선언 가능   
-------------------------------------------------------
객체
Class -> Object
명사, 동사
명사property, member variable, field
동사function, methon

Class
   변수 3개, 함수 2개
Object1, Object2,  Object3
OOP Object Oriented Programming 

코어 객체
자바스크립트 언어가 실행되는 어디서나 사용 가능 기본 객체
Array, date, string, math
객체와 멤버 사이에 점(.)연산자 이용
  
----------------------------------------------------------------

이벤트   
* 마우스 클릭, 키보드 입력, 이미지나 HTML 문서의 로딩, 타이머의 타임아웃 등 사용자의 입력 행위나 문서나 브라우저의 상태 변화를 자바스크립트 코드에게 알리는 통지   

이벤트 리스너   
* 발생한 이벤트에 대처하기위해 작성된 자바스크립트 코드   

이벤트 객체 event object   
* 발생한 이벤트에 관련된 다양한 정보를 담은 객체   
* 이벤트가 처리되고 나면 이벤트 객체 소멸      

버튼 누르면 파일 다운로드 가능한 명령어   
``` <a href="#" download="#"><button>↓ Free Download</button> ``` 

----------------------------------------------------------------

# Bootstrap core JS   
https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js



# 나의 포트폴리오

|Feature|Description|
|:--:|:--:|
|ABOUT|![캡처](https://user-images.githubusercontent.com/80075223/206958864-cb8488ae-286c-43e3-b5ce-cc43649012a3.PNG)|
|Page1|![캡처2](https://user-images.githubusercontent.com/80075223/206959001-d47ffe7a-74ff-4234-9cf2-15027055d051.PNG)|
|Page2|![캡처3](https://user-images.githubusercontent.com/80075223/206959041-b3877840-ff64-4fc5-abe0-a9b35072e19e.PNG)|
|Page3|![캡처4](https://user-images.githubusercontent.com/80075223/206959081-74502b1f-6b17-41eb-80ce-fdfb2b9c7ec5.PNG)|
|PORTFOLIO|![캡처5](https://user-images.githubusercontent.com/80075223/206960005-6037d620-7acc-46df-95ba-5f43735d5667.PNG)
|LINK|[![다운로드 123](https://user-images.githubusercontent.com/80075223/206889633-c0a4e415-0e07-4f6b-bf1e-c0c505e3c617.png)](https://rhkdtjq0915.github.io/bootstrapbluma/)[![다운로드 (1)123](https://user-images.githubusercontent.com/80075223/206889648-cd6dbc5a-1a10-42ad-9c9a-bf439b033d51.png)](https://splendid-marzipan-2d709e.netlify.app/)|
