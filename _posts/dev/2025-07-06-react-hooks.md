---
title: "React Hooks 완벽 가이드"
date: 2025-07-06
categories: [개발]
tags: [react, hooks, javascript, frontend]
---

## React Hooks란?

React Hooks는 함수형 컴포넌트에서 상태와 생명주기를 사용할 수 있게 해주는 기능입니다.

### 주요 Hooks

#### 1. useState
```javascript
const [count, setCount] = useState(0);
```

#### 2. useEffect
```javascript
useEffect(() => {
  console.log('컴포넌트가 마운트되었습니다');
  return () => {
    console.log('컴포넌트가 언마운트됩니다');
  };
}, []);
```

#### 3. useContext
```javascript
const theme = useContext(ThemeContext);
```

### 커스텀 Hooks 만들기
```javascript
function useCounter(initialValue = 0) {
  const [count, setCount] = useState(initialValue);
  
  const increment = () => setCount(count + 1);
  const decrement = () => setCount(count - 1);
  
  return { count, increment, decrement };
}
```

### 장점
- 코드 재사용성 향상
- 로직 분리 용이
- 테스트하기 쉬움
- 더 간결한 코드

Hooks를 잘 활용하면 더 깔끔하고 유지보수하기 쉬운 React 애플리케이션을 만들 수 있습니다! 