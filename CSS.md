# CSS

display

- none : 화면에서 제거
- block
- inline
- inline-block

visibility

- visible
- hidden : 화면에서 안보이게 함(공간은 유지)
- collapse : table 태그를 보이지 않게 만듭니다.

box-sizing

* content-box (기본값)
* border-box : width와 height로만 지정

background-size

- contain : 너비 100%
- cover : 높이 100%
- repeat : 반복 기본 옵션
- no-repeat
- repeat-x : x축 방향으로 반복
- repeat-y : y축 방향으로 반복



line-height : 높이와 똑같이 하여 글자를 수직 정렬



position

* static(기본값) : float를 제외한 속성 사용 불가능
* relative : static이었을 때 배치되는 위치를 기준으로 상대적 위치 지정

- absolute : 절대 위치 좌표 (가장 가까운 부모나 조상 요소중 relative속성을 가지고 있는 요소를 기준으로 한다.)
- fixed : 브라우저 창을 기준으로 좌표
- sticky : 기준점 넘기 전에는 relative기준점 넘으면 fixed처럼 동작

_자손의  position 속성에 absolute 키워드를 적용하면 부모는 height 속성을 사용합니다_

_자손의  position 속성에 absolute 키워드를 적용하면 부모의 position 속성에 relative 키워드를 적용합니다._



z-index : 태그의 z위치 조정



overflow : 자손이 부모의 범위를 벗어날 때 어떻게 처리할지를 결정



float

- left
- right

*자손에 float 속성을 적용하면 부모의 overflow 속성에 hidden 키워드를 적용합니다.*

*clear : both를 사용하여 레이아웃을 구성하는 방법도 있다.*



그레이디언트는 colorzilla.com을 이용한다.

모든 HTML 페이지의 첫 번째 스타일시트는 초기화 코드로 시작하며 리셋코드 홈페이지에서 복사해 온다.



width값을 지정하고 margin : 0 auto 로 작성하여 중앙 정렬

