# JSX

- JavaScript XML의 약어
- 브라우저에서 실행하기 전에 바벨을 사용하여 일반 자바스크립트 형태의 코드로 변환된다.
- JavaScript와 HTML을 동시에 작성 할 수 있어서 편리하다.
- HTML을 작성 하듯이 코드를 적기 때문에 가독성이 높다.
  <br>

## How To Use JSX <br>

1. 부모 요소가 반드시 하나가 감싸는 형태로 작성을 하여야 합니다. <br><br>
   예시 <br><br>
   function Example() { <br>
   &nbsp;return ( <br>
   &nbsp;&nbsp;`<div>` <br>
   &nbsp;&nbsp;&nbsp;&nbsp;`<div>Hello</div>` <br>
   &nbsp;&nbsp;&nbsp;&nbsp;`<div>Kim</div>`<br>
   &nbsp;&nbsp;`</div>` <br>
   );
   } <br><br>

return 다음에 있는 div 태그를 사용 하여 감싼 다음에 사용 합니다(<></> 태그와 `<Fragment><Fragment>`태그를 사용할 수 있습니다.) <br><br>

잘못된 예시 <br><br>
function Example() { <br>
&nbsp;return ( <br>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;`<div>Hello</div>` <br>
&nbsp;&nbsp;&nbsp;&nbsp;`<div>Kim</div>`<br>
);
} <br><br>

부모 태그를 사용하지 않고 Hello와 Kim을 div 태그를 사용했을때
