# html-css-kakaoclone

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
