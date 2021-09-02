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



float (float 속성을 이용해 block인 태그를 수평 정렬 가능.)

- left
- right

*자손에 float 속성을 적용하면 부모의 overflow 속성에 hidden 키워드를 적용합니다.*

*clear : both를 사용하여 레이아웃을 구성하는 방법도 있다.*



그레이디언트는 colorzilla.com을 이용한다.

모든 HTML 페이지의 첫 번째 스타일시트는 초기화 코드로 시작하며 리셋코드 홈페이지에서 복사해 온다.



width값을 지정하고 margin : 0 auto 로 작성하여 중앙 정렬

모바일 웹의 내비게이션 목록은 overflow와 float 속성을 사용하는 방법과 display 속성에 table 키워드를 적용하는 방법, table 태그를 사용하는 방법이 있다.

글자 생략

```html
{
	white-space:nowrap;
	overflow:hidden;
	text-overflow:ellipsis;
}
```

transition-delay : 이벤트 발생 후 몇 초 후에 재생할지 지정

transition-duration : 몇 초 동안 재생할지 지정

transition-property : 어떤 속성을 변형할지 지정

transition-timing-function : 수치 변형 함수를 지정

- cubic-bezier.com

backface-visivility: 3차원 공간에서 평면의 후면을 보이거나 보이지 않게 만드는 속성

perspective: 원근법 벤더 프리픽스 필요

```html
<link rel="styleseet" href="StyleSheet.css" media="screen"/>
위의 코드는 아래코드와 같다.
<style>
@import url(StyleSheet.css) screen;
</style>
```

~~~html
@font-face {
	font-family: 'font-name';
	src: url('/content/file.ttf'),
			 local(file2);
}
~~~

~~~html
<style>
  @media print and (min-width: 100px) {
    h1 {
      
    }
  }
</style>

width, height, device-width, device-height, orientation(장치의 방향), device-aspect-ratio, color(장치의 색상 비트), color-index(장치에서 표현 가능한 최대 색상 개수), monochrome(흑백 장치의 픽셀당 비트수), resolution(장치의 해상도) 속성을 사용가능, orientation을 제외하면 min-,max-접두사 사용가능.
~~~

