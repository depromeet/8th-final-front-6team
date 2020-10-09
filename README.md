# 디프만 8기 파이널 프로젝트 6조 프론트엔드

## 룰

### 기술스택

- React

### PR

- `feature/이슈내용`, `fix/이슈내용` prefix를 붙일것

### 구조

- `페이지 컴포넌트`, `일반 리액트 컴포넌트`로 구분
- 페이지 컴포넌트에서 `라우팅`, `비즈니스 로직` 처리
- 상태관리는 `useReducer` 훅을 사용 (Mobx, Redux 사용X)
- 각 리듀서는 `src/reducers/*` 에 정리하고 로직을 깔끔하게 관리하기 위해 `immer` 사용

### 그 외 규칙들
- 컴포넌트 내부에서의 이벤트핸들러는 `handle` prefix, 외부에서 props로 주입받은 이벤트핸들러는 `on` prefix를 붙인다.ex) onClick(props로 받은 경우), handleClick(컴포넌트내부)
