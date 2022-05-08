# LifeCycle

- React에서의 각 컴포넌트는 3가지의 주요한 단계를 통해서 주기를 관리하고 있습니다
  <br>3가지 단계에는 1. Mount 단계, 2. Updating 단계, 3. Unmounting 단계를 의미 합니다.
  <br>

## Mounting

- Mounting 이란 DOM에 요소를 붙이는 것을 말합니다.
  Mounting을 할때에는 아래의 4단계를 거쳐 Mounting을 하게 됩니다.<br>

1. constructor()<br>
2. getDerivedStateFromProps()<br>
3. render()<br>
4. componentDidMount()<br>

### 이 4가지 단계중 render() 메소드 같은 경우는 DOM에 HTML를 표현 해주는 역활로 항상 호출이 되어야 합니다 <br><br>

## Updating

- Updating이란 단어 뜻 그대로 컴포넌트가 업데이트 할 때를 의미합니다.<br>
  업데이트에 기준은 새로운 Props가 생기거나 state값이 변경 될때를 기준으로 두고 있습니다. <br>
  컴포넌트가 업데이트가 되면 아래와 같은 순서로 실행이 됩니다.<br>

1. getDerivedStateFromProps()
2. shouldComponentUpdate()
3. render()
4. getSnapshotBeforeUpdate()
5. componentDidUpdate()
   <br><br>

## Unmounting

-컴포넌트가 DOM을 제거하거나 Unmounting을 할 때를 의미합니다.<br>
Unmounting 같은 경우는 한나의 순서로 진행이 됩니다.

1. componentWillmount()
