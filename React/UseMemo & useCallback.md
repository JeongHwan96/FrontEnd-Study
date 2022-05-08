# Memoization

먼저 UseMemo 함수를 알기전에 Memoization 의 개념을 알아보도록 하겠습니다
Memoization이란 간단하게 말하면 수행한 연산의 결과값을 어딘가에 저장을 하고 똑같은 입력이 들어오게 되면 저장을 했던 결과값을 다시 재활용 하는 기법을 말합니다. <br><br>

## Why do you use Memoization<br>

Memoization을 사용하게 되면 중복 연산을 피할 수 있습니다 그로 인해 서능을 최적화 시킬 수 있게 됩니다. <br><br>

# UseMemo

- UseMemo 이란<br>
  Memoization된 "값"을 반환 하는 것을 말합니다.

  ## 🌻 how to use UseMemo() ?

UseMemo()를 사용 하기 위해서는 useMemo를 import 시켜야 합니다<br>

## import {useMemo} from 'react'; <br>

  <br>
 기본 형태: useMemo(() => {console.log("Hello")}, [example]);<br>
 example 값이 변할 때에만 console에 Hello를 출력하게 됩니다.
<br><br><br>

# UseCallback

- UseCallback 이란<br>
  Memoization된 "함수"을 반환 하는 것을 말합니다.

  ## 🌻 how to use UseCallback() ?

UseMemo()를 사용 하기 위해서는 useMemo를 import 시켜야 합니다<br>

## import {useCallback} from 'react'; <br>

  <br>
 기본 형태: useCallback(() => {console.log("Hello")}, [example]);<br>
 example 값이 변할 때에만 {console.log("Hello")} 함수를 반환 합니다.
