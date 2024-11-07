# React 배우기 전에 쓰는 이유부터 알아야

## React 왜 씁니까

### Naver Vibe, Flipkart, Instagram 이런 사이트들을 Single Page Application 이라고 하는데

#### 장점
1. HTML 파일을 1개만 사용
2. 다른 페이지를 보여줄 때 HTML 부분만 샥 갈아치워서 보여줌
3. HTML 재사용이 편리함
4. 컴포넌트 단위로 개발하여 여러 개발자들이 분업하기 좋음
5. React Native를 사용하면 리액트와 비슷한 문법으로 모바일 앱 개발 가능
6. 프론트엔드와 백엔드 파트를 완전히 분리하여 각각 개발 가능

### 단점
1. 많은 자바스크립트로 인해 웹페이지 크기가 커짐
2. 웹페이지 로드시 HTML 내용물이 천천히 채워져서 SEO에 악영향이 있을 수 있음 (hydration 작업)
3. 간단한 사이트도 코드가 쓸데없이 복잡해짐

> 이러한 단점에도 불구하고 장점이 더 커서 React를 사용합니다.

## 필요한 사전지식

1. **HTML / CSS**: 기본적인 개념 이해
2. **JavaScript**: 변수, 함수, 조건문 (if), 반복문 (for), 배열과 객체 자료 다루기

# React 설치와 개발환경 셋팅

## 1. 개발환경 셋팅
1. **Node.js 설치**
   - Node.js를 다운로드 및 설치합니다. (검색창에 `nodejs`를 검색)
2. **VS Code 설치**
   - Visual Studio Code (VS Code) 에디터를 다운로드 및 설치합니다. (검색창에 `vscode`를 검색)

## 2. React 프로젝트 생성
1. **작업 폴더 생성 및 터미널 열기**
   - 프로젝트용 폴더를 만들고 `Shift + 우클릭`하여 PowerShell 또는 터미널을 엽니다.
   
2. **React 프로젝트 생성**
   - 터미널에 다음 명령어를 입력합니다:
     ```bash
     npx create-react-app 프로젝트명
     ```
     
3. **에러 해결**
   - **Windows**: "허가되지 않은 스크립트" 에러 발생 시
     1. Windows 검색에서 PowerShell을 검색하고 **관리자 권한으로 실행**
     2. 다음 명령어 입력 후 `Yes` 선택
        ```bash
        Set-ExecutionPolicy Unrestricted
        ```
   - **Mac**: "Permission" 관련 에러 발생 시
     1. 터미널에 다음 명령어 입력 후 비밀번호 입력 및 `Yes` 입력
        ```bash
        sudo npx create-react-app 프로젝트명
        ```

## 3. App.js 파일 열기
- 생성된 프로젝트 폴더에서 `src/App.js` 파일을 엽니다.

## 4. 개발 서버 실행 (미리보기)
- 터미널에서 다음 명령어로 미리보기 서버를 실행합니다:
  ```bash
  npm start
  
## 5. 셋팅 설명
- **create-react-app 라이브러리**: React 프로젝트를 쉽게 생성하기 위해 사용하는 라이브러리
  - React를 사용하려면 `create-react-app`이 필요한데, 이 라이브러리를 실행하려면 **npm**이 필요합니다. (npm은 Node.js를 설치하면 함께 설치됩니다)
- **프로젝트 생성 명령어**
  - `npx create-react-app my-app`: `my-app`이라는 이름의 새로운 React 프로젝트를 생성하는 명령어입니다.

## 6. 프로젝트 폴더 및 파일 설명
- **node_modules 폴더**: 프로젝트에서 사용하는 라이브러리 코드 보관함
- **public 폴더**: 정적(static) 파일을 모아놓는 곳 (이미지, 아이콘, HTML 등)
- **src 폴더**: 실제 코드를 작성하는 공간
- **App.js**: 메인 페이지 역할
  - `index.js`에서 `App.js`를 `index.html`로 렌더링하여 브라우저에 HTML로 보여줍니다.
- **package.json**: 프로젝트 정보 및 의존성 관리 파일
