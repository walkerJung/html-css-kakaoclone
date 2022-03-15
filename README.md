# html-css-kakaoclone

- CSS 관련 검색을할땐 MDN 을 붙이자!

# 3.4 Margin Part One

- block 속성만 width, height 값을 가질수있다.
- block 은 margin, border, padding 속성을 가지고있다.
- margin : border 로 부터 바깥 공간을 말한다.

# 3.5 Margin Part Two

- Collapsing margin : 두 요소의 border 의 경계가 같으면 margin 값을 공유한다.

# 3.6 Paddings and IDs

- padding : border 로 부터 안쪽 공간을 말한다.

# 3.7 Border

- border : 경계선을 의미한다.

# 3.8 Classes

- inline 속성은 widht, height 값을 가질수 없으므로, margin-top 과 margin-bottom 을 가질수없다.
- padding 은 사방에 가질수 있다.
- 위와 같은 상황에 margin-top 과 margin-bottom 을 주려면 display : inline-block 으로 변경한다.

# 3.10 Flexbox Part One

- 부모 엘리먼트에 display : flex 를 적어준다.
- justify-content 를 사용하면 수평 축을 기준으로 움직인다.
- align-itmes 를 사용하면 수직 축을 기준으로 움직인다.

# 3.11 Flexbox Part Tow

- flex-direction 은 default 가 row 다
- flex-direction 이 row 인 상태에선 justify-content 와 align-itmes 가 바뀐다
- https://flexboxfroggy.com/#ko

# 3.12 Fixed

- position fixed 는 엘리먼트가 처음 생성된 자리에 고정시켜준다.
- top, left, right, bottom 중 하나만 수정해도 서로 다른 레어이에 위치하게 된다. (맨 위로 올라오게된다.)

# 3.13 Relative Absolute

- position relative 는 엘리먼트가 처음 위치한 곳을 기준으로 top, left, right, bottom 으로 위치를 수정할수 있다.
- position absolute 는 엘리먼트의 부모가 relative 인지 먼저 확인하고, relative 한 부모를 기준으로 top, left, right, bottom 위치를 수정할수있다. 단 relative 한 부모 엘리먼트가 없을경우 body 를 기준으로 이동한다.

# 3.14 Pseudo Selectors Part One

- pseudo selector : 세부적으로 엘리먼트를 선택할수 있게 해주는 문법이다.
- :first-child, :last-child, :nth-child() 상황에 맞게 사용하면 된다.

# 3.15 Combinators

- div span : div 아래 모든 span 을 의미한다.
- div > span : div 의 바로 밑 자식 span 을 의미한다.
- div > span + p : div 의 바로 밑 자식 span 의 바로 뒤에있는 형제 p 를 의미한다.
- div > span ~ p : div 의 바로 밑 자식 span 의 형제 p 를 의미한다. (바로 뒤에 나올 필요가 없다.)

# 3.16 Pseudo Selectors Part Two

- https://developer.mozilla.org/ko/docs/Web/CSS/Attribute_selectors
- http://flukeout.github.io/

# 3.17 States

- active : 해당 엘리먼트를 마우스로 클릭했을 때 효과가 적용된다.
- hover : 마우스를 해당 엘리먼트 위로 올렸을때 효과가 적용된다.
- focus : 선택되었을때 효과가 적용된다.
- focus-within : 부모 엘리먼트에 선언해서 사용한다, 즉 자신의 자식 엘리먼트 중 하나가 focus 되었을때 효과가 적용된다.
- 조건을 나열해서 여러 상황을 설정할수 있다. (나열한 조건 모두 만족할때 실행된다.)
  form:hover input:focus {
  background-color: teal;
  }

# 3.18 Recap

- ::placeholder : placeholder의 특성만 바꾸고 싶을때 사용한다.
- ::selection : drag 할때 특성을 바꾸고 싶을때 사용한다.

# 3.19 Colors and Variables

- :root 라는 엘리먼트에 변수를 추가해서 사용할수 있다. custom property 라고 부른다.
- 변수 이름 작성 양식은 --변수이름 이다. 띄어쓰기는-로 넣어준다. (ex > --main, --main-color)
- :root 에 선언한 변수를 사용할때는 var(변수이름) 으로 사용한다. (ex > var(--main), var(--main-color))

# 4.0 Transitions

- transition : 어떤 상태에서 다른 상태로 변화를 주는 애니메이션이다.
- transition 은 엘리먼트에 선언해야 한다. state (active, hover, focus ...) 에 선언하면 안된다.

# 4.1 Transitions Part Two

- ease-in function : 브라우저에게 변화하는 방법을 알려주는 역할이다.
- 보통 all 로 사용하고, 변화 요소를 각각 다르게 다루고 싶다면 각각 선언하여 사용한다.

# 4.2 Transformations

- transformation : 한 요소를 변형 시킬수 있다.
- 3d CSS 라고 생각하면 된다.

# 4.3 Animations Part One

- @keyframes 애니매이션이름{
  from{
  }
  to {
  }
  }

  img {
  animation : 애니메이션 이름 재생시간 옵션
  }

  infinite 를 붙이면 무한으로 반복된다.

# 4.4 Animations Part Two

- from to 대신에 0% 25% 50% 75% 100% 처럼 단계를 나눠서 animation 을 구현할수 있다.
- 꼭 transform 으로 만들 필요는없지만 웬만하면 transform 을 추천한다.
- https://animista.net/

# 4.5 Media Queries

- Media query : CSS 를 이용하여 스크린의 사이즈를 알수 있는 방법이다.
- @media screen and (max-width: px) {} 을 이용하여 원하는 픽셀부터 다르게 보이게 할수 있다. (min-width 도 사용해서 범위를 지정할수도있다.)
- orientation : portrait - 세로일 경우를 뜻한다.
- orientation : landscape - 가로일 경우를 뜻한다.
- ex > @media screen and (min-width: 600px) and (max-width: 1000px) {
  div {
  background-color: wheat;
  }
  }
- ex > @media screen and (orientation:landscape) {
  span {
  display: none;
  }
  }
