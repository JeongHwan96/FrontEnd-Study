# FrontEnd React 공부 하기(계속 추가중)

## 프론트 엔드 공부를 하면서 React에 관련하여 기본 적인 부분과 알아둬야 하는 부분을 정리하고 기억 하기 위해 작성중입니다😊

<br>

# Virtual DOM

- Virtual DOM 이란<br>
  실제 DOM(Real DOM) 의 문제점을 해결 하기 위해 만들어진 DOM
  <br>

## 🌻 실제 DOM(Real DOM)의 문제점이 무엇일까?<br>

실제 DOM의 문제점은 페이지를 재 렌더링을 할때 느리다는 문제점을 가지고 있습니다
더 정확히 말하면 브라우저 단에서 DOM의 변화가 일어나면 CSS를 다시 연산하고 레이아웃을 구성하며 웹 페이지를 repaint 하는데서 시간이 걸리기 때문에 느려진다고 말합니다.
<br>

## 🌻 Virtual DOM의 특징<br>

1. 바뀐 부분만 실제 돔에 적용함으로 속도가 빠르다.
2. Real Dom 보다 가볍다
3. 성능 향상에 도움을 준다.
   <br>

## 🌻 Virtual DOM의 작동 원리<br>

1. 데이터를 업데이트를 하면 전체 UI를 가상 돔(Virtual DOM)에 리 렌더링 작업을 한다.
2. 업데이트 하기전 가상 돔에 있는 정보와 현재 가상 돔에 있는 정보를 비교한다.
3. 비교해서 변경 된 부분만 실제 DOM에 적용을 시킨다.
   <br><br><br><br>

# Props 와 State

Props 란 간단히 말해 부모 컴포넌트가 자식 컴포넌트에게 주는 값들을 말합니다.<br>
State 란 컴포넌트 내부에서 선언을 하며 내부에서 값을 변경 할 수가 있습니다. <br>
동적인 데이터를 다룰 때 주로 사용이 됩니다.
<br><br><br><br>

# Class Component 와 Function Conponent

## 🌻 What is Class Component?<br>

React에서는 컴포넌트를 선언 하는 두가지 방법 중 하나이며 현재는 많이 사용하지 않는다

## 🌻 Class Compoenet 특징<br>

1. state와 lifeCycle을 사용할 수 있다.
2. render() 메소드가 반드시 필요하다.
3. class 키워드가 필요하다
4. component를 상속 받아야한다.
   <br><br>

## 🌻 What is Function Component?<br>

함수를 기반으로 작성하는 컴포넌트

## 🌻 Function Compoenet 특징<br>

1. 클래스형 컴포넌트에 비해 훨씬 짧고 직관적인 코드를 짤 수 있다.
2. Hook을 사용하여 Function Component에서도 Class Component의 라이프 사이클 메서드와 같은 기능을 사용 할 수 있다.

## 🌻 Why use Function Component more?

1. State를 사용하지 않고 Props를 받아서 UI에 뿌려주기 때문에
2. Hook을 사용하여 로직의 재 사용이 가능 하기 때문에
   <br><br><br><br>

# Hook

React v16.8 에 추가된 기능으로 Function Component에서도 상태를 관리 할 수 있게 되었다.
<br>
대표 적으로 useState(), useEffect() 등이 있다.

## 🌻 What is useState?

컴포넌트에서 state값을 추가할때 사용된다<br>
Function Component는 Class Component 처럼 state를 사용 할 수 없어서 useState() 를 사용하여 class Component의 state 와 같은 기능을 할 수 있도록 해준다
<br>

## 🌻 how to use useState() ?

useState()를 사용하기 위해서는 useState를 import 시켜야 합니다<br>

## import {useState} from 'react'; <br>

다음으로 useState를 선언 해야합니다

## const [data, setData] = useState(초기값);<br>

배열 안에 있는(예시에는 data) 이름은 원하는 이름으로 작성 할 수 있습니다<br>
배열의 첫 번째 원소는 상태값을 의미 하고 두 번째 원소는 상태값을 업데이트 하는 함수 입니다.
<br><br><br>

## 🌻 What is useEffect

컴포넌트가 렌더링 될 때 특정 작업을 실행할 수 있도록 하는 Hook이다.
<br>
Function Component는 Class Component 처럼 state를 사용 할 수 없어서 useState() 를 사용하여 class Component의 state 와 같은 기능을 할 수 있도록 해준다
<br>

## 🌻 how to use useState() ?

useState()와 마찬가지로 사용하기 위해서는 useEffect를 import 시켜야 합니다<br>

## import {useEffect} from 'react'; <br>

다음으로 useState를 선언 해야합니다<br><br>
기본 형태 : useEffect(function, deps)<br>
예시 :
useEffect(() => { <br>
axios <br>
.get("https://f94836e9-9f51-4d28-82bd-9af8ad671717.mock.pstmn.io/example") <br>
.then((response) => {<br>
console.log(response);<br>
setDataName(response.data);<br>
});
}, []);<br><br>
예시에 있는 내용들은 꼭 axios가 아닌 다른 것을 적어도 무방합니다<br>
기본 형태에서 deps 부분은 function을 실행 시킬 조건을 적어줍니다 예시 와 같이 []만 적게 되면 무조건 한번만 실행 된다는 의미 입니다
