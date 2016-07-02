<!-- [웹표준 준수] HMTL 문법은 유효한가? -->

<!-- [접근성 고려] 사용자 입장에서 접근하는데 문제가 없는가? (음성 출력/키보드 접근 등) 
* 로고 이미지를 a태그로 감싸지 않아서 클릭이나 탭으로 접근이 불가능했다. validation 검사 후 내가 짠 html문서를 키보드로 탐색해보자!-->

<!-- [의미 구조화] HTML 구조는 올바른 의미를 가지는가? * sectioning요소가 아닌 header가 sectioning 요소인 nav를 포함하는 것이 올바른가? 하는 논의가 있었음
* html5에서 header는 하나의 sectioning 요소 안에서 배너나 로고 포함하는 역할을 함. 굳이 nav가 header안에 있을 필요는 없다.
* 어디까지를 nav로 보아야 할 것인가, nav와 main 경계 논의.
* nav는 사이트를 탐색하는 데 필요한 요소 = 동일 사이트 내 다른 페이지로 이동해도 같은 위치에 같은 모양으로 존재하는 부분을 nav로 두면 되겠다.
* main은 페이지에서 이용자들에게 보여주고자 하는 주요 컨텐츠. 문서 내에서 main요소는 한번만 사용된다.
* custom form요소 - 웹브라우저에서 기본적으로 제공되지 않는 (+), (-)버튼 등을 어떤 요소로 구현할 것인가? 에 대한 논의도 필요함. 사이트 살펴보면서 생각지도 않았던 부분이다. 앞으로 이런 요소들을 잘 살펴보자.
*예약창 부분의 여러 폼 요소들은 목록으로 묶어야 할까?
*폼 요소 내에서도 구획 나누어야 할 필요성 있겠다. 마일리지 사용/ 편도, 다구간 선택부분은 다른 내용인데 한꺼번에 폼 요소 안에 있으니 구분하기 어렵다. -> 동일 내용에 대한 부분을 목록으로 묶었다
-->

<!-- [코드 최적화] 불 필요한 <div> 또는 <span> 요소의 남용은 없었는가? 
*최대한 의미 있는 sectioning 요소들로 구조화하려고 하였으나 아직 최상단 네비게이션 부분(?) 언어 선택, 로그인 부분을 어떤 요소로 마크업 해야 할지 몰라서 div로 묶었다. utility nav라고 본다면 nav로 마크업 해도 괜찮을 듯 하다.
*급하게 하느라 이벤트 목록 부분의 각 li마다 ul부모를 하나씩 지정했다. 이벤트 목록이 하나의 ul부모에 포함되도록 수정하였다-->

<!-- [팀원간 소통] 코드는 읽기 쉽고, 간결한가? 
*sectioning 요소에 해당 내용과 관련된 클래스 이름을 줘서 파악하기 쉬웠다.
* 짧은 시간 내에 하려다보니 보이는대로 막 쓰게 된다. 컨텐츠는 옮기는 데 시간 쓰지 말고 더미텍스트 이용하자.
* 큰 구조를 파악하고 보기 쉽게 코드를 짜려고 노력하기! 
*들여쓰기는 잘 하고 있다고 생각했지만, 내가 내 코드 설명하는데도 한참 들여다봐야 했다. 
*큰 섹션마다 주석을 달고, 코드 짜다가 의문나는 점은 옆에 주석으로 메모해두자!
-->