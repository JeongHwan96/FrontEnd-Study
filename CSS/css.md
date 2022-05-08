# FrontEnd CSS 공부 하기(계속 추가중)

## 프론트 엔드 공부를 하면서 CSS 관련하여 정리하고 기억 하기 위해 작성중입니다😊

<br>

# Position

position 속성은 HTML 문서 상에서 요소가 배치되는 방식을방법을 지정합니다.

- static: Position 값을 지정 하지 않았을때 기본값으로 지정 되는 값이며 HTML에 요소들이 작성된 순서대로 브라우저 화면에 보여지게 됩니다.

- relative: 자기 자신을 기준으로 top, rigth, bottom, left의 값에 따라 배치를 합니다.

- absolute: 부모 요소를 기준으로 배치합니다

- fixed: 뷰포트 기준으로 배치를 합니다

- sticky: 스크롤 영역을 기준으로 배치가 됩니다.

## 🌻 뷰포트

- 뷰포트(viewport)는 화면에서 실제 내용이 표시되는 영역으로, 데스크톱은 사용자가 설정한 해상도가 뷰포트 영역이 되고, 스마트 기기는 기본으로 설정되어 있는 값이 뷰포트 영역이 됩니다.
  <br><br><br><br>

# Display

display 속성은 요소들을 어떤식으로 보여줄지를 결정을 합니다

- none : 요소들이 화면에 사라지게 됩니다

## 🌻 visibility : hidden 과의 차이점은 ?

visibility 를 hidden으로 처리 하게 되면 영역은 지정이 되지만 화면상에는 보이지 않게 됩니다
반면에 display를 none으로 처리 하게 되면 영역자체가 지정이 되질 않습니다.
<br><br><br><br>

- block : div, p, h1 등의 태그의 기본 값이며 block을 하게 되면 여러개의 엘리먼트들을 밀어내고 혼자 공간을 차지하게 됩니다

## 🌻 block 속성의 특징

1.  값과 height 값을 지정 해줄 수 있습니다.
2.  가로로 공간을 차지하게 됩니다
    <br><br><br><br>

- inline : block 속성과 다르게 엘리먼트의 전후 줄바꿈이 없습니다 즉 엘리먼트들이 나란히 배치가 됩니다 대표적인 inline 엘리먼트들은 span, a, em 태그 등이 있습니다.

## 🌻 inline 속성의 특징

block 속성과 다르게 width와 height값을 지정을 하여도 무시된다는 점

## 🌻그러면 padding이나 margin으로 지정 해되 되는거 아닌가요?

padding이나 margin을 사용하게 되더라도 좌우 간격만 반영이 됩니다 즉 상하 간격은 반영이 되지 않습니다!
<br><br><br><br>

-inline-block : inline 속성과 block 속성의 특징을 합쳐 놓은 속성입니다

## 🌻 inline-block 속성의 특징

1. 배치 부분에서는 inline 속성과 마찬가지로 전후 줄바꿈이 없이 나란히 배치가 됩니다
2. width,height,margin,padding 값이 block 속성과 똑같이 모두 지정이 가능합니다
   <br><br><br><br>

### margin과 padding의 설명과 차이점

- margin: 요소의 주변 여백을 의미 하며 쉽게 말해 바깥쪽 여백을 의미합니다.

- padding: 컨텐츠 영역의 테두리 사이 여백을 의미하며 쉽게 말하여 안쪽 여백을 의미합니다.

## 🌻 margin과 padding 사용법

- margin : margin-top,margin-right,margin-bottom,margin-left를 사용하여 각자 조정 하는 방법과 <br>
  margin: 10px 20px 30px 40px 과 같이 한번에 사용할 수가 있습니다 순서는 첫번째 나오는 값(10px)은 top 두번째 나오는 값(20px)은 right 세번째 나오는 값은(30px)은 bottom, 네번째 나오는 값(40px)은 left 입니다.

- padding : padding도 margin과 마찬가지로 margin 대신 padding을 넣어서 사용하면 됩니다

<br>
