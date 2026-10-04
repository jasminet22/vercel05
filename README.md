# Deployment

- Vercel 배포 URL: https://vercel05-self.vercel.app/

# Key Learning

## 이번 주 핵심 내용 3가지

1. JavaScript를 사용한 DOM 활용법
2. 동적 요소 생성과 삭제
3. javascript를 사용한 crud 페이지 구현

## CRUD Service

- 구현한 서비스 주제: 도서 관리
- 사용하는 데이터 Field: id, title, author, category, price, year
- Create 구현 방법: 도서 데이터를 입력받아 `push()`로 배열에 추가하여 구현 
- Read 구현 방법: `render()`을 사용해서 구현
- Update 구현 방법: 수정 버튼을 누르면 기존 데이터를 입력칸에 넣고, 저장할 때 수정된 데이터를 저장하여 배열의 해당 도서를 변경
- Delete 구현 방법: `splice()`로 배열에서 도서를 삭제하고 목록을 다시 표시

## JavaScript

### 주요 기능

- `querySelector()`: `id`를 이용해 입력칸, 버튼, 목록 등의 HTML 요소를 선택
- `addEventListener()`: 선택된 요소가 동작을 실행하도록 연결
- `createElement()`: 목록에 표시할 `div`와 수정·삭제 버튼 생성
- `appendChild()`: 만든 도서 항목을 목록에 추가
- Array: 도서 객체를 저장하고 `push()`, `find()`, `indexOf()`, `splice()`로 데이터를 관리
- `render()`: 기존 목록을 비우고 배열의 도서 데이터를 다시 화면에 표시

## AI / Search Usage

- chatgpt를 사용
- 항목의 추가와 삭제, 수정 구현 방법을 질문하고 코드에 적용
- 처음에는 remove만 사용하려고 했지만 splice가 필요하다는 이유가 궁금해서 찾는 용도로 사용

## Problem & Solution

### 문제
이번 과제에서 발생한 문제는 crud 프로그램을 구현하면서 javascript을 활용해서 수정하는 기능을 구현하는 방법을 알지 못했던 것이 문제였다.

### 해결 방법
AI에게 수정 기능을 구현하는 방법을 질문하고 설명을 들었다. 수정 버튼을 누르면 선택한 도서의 데이터를 입력칸에 표시하고, 수정할 도서의 ID를 `editingId`에 저장한다. 저장 버튼을 누르면 `find()`로 ID가 같은 도서를 배열에서 찾고, 입력한 값으로 해당 도서의 제목, 저자, 카테고리, 가격, 출판 연도를 바꾼다. 마지막으로 입력칸을 비우고 `render()`를 다시 실행해 수정된 내용이 목록에 표시되도록 구현했다.

## Reflection
이번주 과제를 통해서 javascript와 dom, array에 대해서 잘 알게 된 것 같다. 