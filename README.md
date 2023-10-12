# 202130301 강진선

# 6주차 (2023.10.12)

### 페이지에서 경로 매개변수 사용하기

> <img width="1440" alt="스크린샷 2023-10-12 오후 2 41 19" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/c0fbf4df-73db-454e-b762-b796468960a4">

> Next.js에서는 리액트 훅 덕분에 쉽게 경로 매개변수 값을 가져올 수 있다.

### 컴포넌트에서 경로 매개변수 사용하기

> Next.js에서는 useRouter 훅 덕분에 별다른 어려움 없이 컴포넌트 안에서 경로 매개변수를 사용할 수 있다.
> 리액트 훅은 리액트 상태나 함수형 컴포넌트의 라이프 사이클을 다룰 수 있는 함수이며 useRouter 역시 다른 리액트 훅과 동일하게 작동한다.

### 클라이언트에서의 내비게이션

> <img width="1440" alt="스크린샷 2023-10-12 오후 2 41 19" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/183ca709-3e50-45de-a31c-9140c0d4ea2b">

> <img width="1440" alt="스크린샷 2023-10-12 오후 3 05 00" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/516616e3-83e2-423f-8547-196f99eae250">

### 정적 자원 제공

> 정적 자원은 이미지, 폰트, 아이콘, 컴파일한 CSS 또는 JS 파일과 같이 동적으로
> 변하지 않는 모든 종류의 파일을 의미한다.
> 이런 정적 자원은 /public 디렉터리 안에 저장하는 방식으로 클라이언트에 쉽게 제공한다.
> /public 디렉터리 안에 있는 모든 파일은 Next.js가 정적 자원으로 간주하고 제공된다.

### 누적 레이아웃 이동

> 일반적으로 최적화되지 않은 이미지를 제공하는 것은 사용자 경험에 나쁜 영향을 준다.
> 이미지를 불러오는 데 시간이 오래 걸리고, 이미지를 불러온 후에도 이미지 주변의 레이아웃이 변경되는 등 UX 관점에서도 좋지 않다.

### 자동 이미지 최적화

> <img width="1440" alt="스크린샷 2023-10-12 오후 4 15 27" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/6ee2c3ed-0d6c-40b5-a30a-52ec2b86a6f8">

> 이미지 최적화 기능을 사용하면 이미지를 WebP와 같은 최신 이미지 포맥으로 제공할 수 있다.
> 브라우저가 해당 이미지 포맷을 지원해야 한다.
> 최신 포맷을 지원하지 않는 브라우저의 경우에는 png나 jpeg와 같은 예전 이미지 포맷도 제공한다.
> 필요한 경우 이미지 크기를 조절해서 클라이언트가 아주 큰 이미지를 다운로드 하느라 속도가 느려지는 상황도 피할 수 있다.
> 브라우저가 이미지를 요청하면 이미지를 최적화하고, 크기를 조절하고, 렌더링한다.
> layout 속성값을 지정해서 이미지를 원하는 대로 자를 수 있다. layout 속성에는 fixed, responsive, intrinsic, fill 이렇게 네 개의 값을 지정할 수 있다.

### 외부 서비스를 통한 자동 이미지 최적화

> Next.config.js 파일 내에 loader 속성을 지정해서 외부 서비스를 통해 자동 이미지 최적화 작업을 처리한다.
> 웹앱을 Vercel 등 서비스 제공 업체로 배포하는 경우에는 이 속성을 지정할 필요가 없다.
> 그 밖의 경우라면 loader를 지정하고, 컴포넌트 내에서 loader 속성을 전달하면 된다.

# 5주차 (2023.10.05)

### 동적 컴포넌트 로딩

> <img width="1440" alt="스크린샷 2023-10-05 오후 2 15 01" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/c57a5b51-8b1c-4929-9723-e538d27e4bd8">
>
> 이 코드를 실행하면 Highlight 컴포넌트를 동적 임포트로 불러온다.
> 이렇게 동적 임포트를 사용하면 Next.js는 해당 컴포넌트를 서버에서 렌더링 하지 않는다.
> 따라서 사용자는 리액트 하이드레이션이 끝날 때까지 기다려야 해당 컴포넌트를 사용할 수 있게 된다.

### 정적 사이트 생성(SSR)

> SSG는 일부 또는 전체 페이지를 빌드 시점에 미리 렌더링 한다.
> Next.js는 페이지를 빌드 과정에서 정적 페이지로 미리 렌더링해서 HTML 마크업 형테로 제공한다.

### SSG의 장점

> 1. 쉬운 확장
>
> - 정적 페이지는 단순 HTML 파일이므로 CDN을 통해 파일을 제공하거나 캐시에 저장하기 쉽다.
>
> - 직접 웹 서버에서 웹 애플리케이션을 제공하는 경우에도 정적 페이지는 별도의 연산 없이 정적 자원 형태로 제공되기 때문에 서버에 부하를 거의 주지 않는다.
>
> 2. 뛰어난 성능
>
> - 빌드 시점에 HTML 페이지를 미리 렌더링하기 때문에 페이지를 요청해도 클라이언트나 서버가 무언가를 처리할 필요가 없다.
>
> 3. 더 안전한 API 요청
>
> - 페이지 렌더링을 위해 웹 서버가 민감하고 중요한 데이터를 클라이언트로 보낼 필요가 없다.
>
> - 필요한 모든 정보가 빌드 시점에 미리 렌더링되어 있다.

### Next.js 기초와 내장 컴포넌트

> Next는 서버 사이드 렌더링 외에도 많은 내장 컴포넌트와 함수를 제공한다.

### 라우팅 시스템

> <img width="1440" alt="스크린샷 2023-10-05 오후 3 52 23" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/123f5442-eb71-4fa0-9553-d9b6fd6dac05">

> React Router, Reach Router, Wouter와 같은 라이브러리를 사용하면 클라이언트에서의 라우팅만 구현할 수 있다.
> 모든 페이지가 클라이언트에서만 만들어지고 렌더링되는 것이다.

# 4주차 (2023.09.21)

### 클라이언트 사이드 렌더링(CSR)

> SSR은 이점이 많지만 주의해야 할 점도 있다. 브라우저 전용 API를 사용해야 하는 컴포넌트가 있다면 해당
> 컴포넌트를 반드시 브라우저에서 렌더링하도록 명시적으로 지정해야 한다.
> Next.js는 페에지를 기본적으로 서버에서 렌더링하기 때문에 window, document와 같은 객체나 API를
> 제공하지 않는다. 이런 부분에서는 CSR이 필요하다.
> 표준 리액트 앱은 서버에서 자바스크립트 번들을 클라이언트로 전송한 다음 렌더링을 시작한다.
> 실제 렌더링은 클라이언트로 전송한 웹 애플리케이션에서 이루어진다.

### CSR을 사용할 때 주요 이점

> 1. 네이티브 애플리케이션처럼 느껴지는 웹 애플리케이션
>
> - 콘텐츠를 바꾸기 위해 페이지를 새로 고칠 필요가 없다.
>
> 2. 쉬운 페이지 전환
>
> - 클라이언트에서의 네이게이션은 브라우저 화면을 새로 고칠 필요 없이 다른 페이지로의 이동을 가능하게 만든다.
>
> 3. 지연된 로딩과 성능
>
> - CSR을 사용하면 웹 앱에서는 최소로 필요한 HTML 마크업만 렌더링 한다.
>
> 4. 서버 부하 감소
>
> - AWS Lamda나 Firebase와 같은 서버리스 환경에서 웹 앱을 제공할 수 있다.

### CSR을 사용할 때 단점

> 1. 네트워크 속도가 느린 환경에서는 전체 자바스크립트 코드와 CSS 파일을 받는 것에만 수 초가 소요될 수 있다.
>
> 2. 웹 앱의 SEO에도 여향을 준다. 검색 엔진 봇들이 웹 앱의 페이지를 수집해도 그 내영은 빈 것으로 보인다.

### React.useEffect 훅

> 최근 리액트는 함수형 컴포넌트 사용을 강조하고 있다. next.js가 useEffect를 리액트 하이드레이션 이후
> 브라우저에서 실행하도록 만들어야 한다, 이렇게 하면 특정 작업을 반드시 클라이언트에서 실행하도록 강제할 수 있다.

# 3주차 (2023.09.14)

### 렌더링 전량

> 렌더링 전략이란 웹 페이지 또는 웹 애플리케이션을 웹 브라우저에 제공하는 방법을 의미한다.
>
> Next.js에서는 반드시 클라이언트에서 렌더링해야 할 컴포넌트도 지정할 수 있어서 개발이 훨씬 쉽다.

### 서버 사이드 렌더링(SSR)

> 1. 웹 페이지를 제공하는 가장 흔한 방법이다.
>
> 2. Next.js도 마찬가지로 각 요청에 따라 서버에서 HTML 페이지를 동적으로 렌더링하고 웹 브라우저로 전송할 수 있다.
>
> 3. 서버에서 렌더링한 페이지에 스크립트 코드를 집어넣어서 나중에 웹 페이지를 동적으로 처리할 수도 있는데 이를 하이드레이션이라고 한다.
>
> 4. 특정 렌더링 전략만 사용한다고 가정하면 SSR은 리액트의 CSR(클라이언트 사이즈 렌더링)에 비해 여러 가지 장점이 있다.

### SSR의 장점

> 1. 더 안전한 웹 애플리케이션
>
> - 중요한 데이터를 클라이언트에 노출할 필요가 없기 때문에 더 안전하다.
>
> 2. 더 뛰어난 웹 사이트 호환성
>
> - 클라이언트 환경이 자바스크립트를 사용하지 못하거나 오래된 브라우저를 사용하더라도 웹 페이지를 제공할 수 있다.
>
> 3. 더 뛰어난 SEO
>
> - 클라이언트에서 서버가 렌더링한 HTML 콘텐츠를 받기 때문에 봇이나 웹 크롤러 같은 검색 엔진 웹 문서 수집기가 페이지를 렌더링할 필요가 없다.

# 2주차 (2023.09.07)

### Next.js 시작하기

> 프로젝트 기본 구조
>
> - node.js와 npm만 설치하면 된다.
> - create-next-app이 기본적인 next.js 앱을 시작할 수 있는 코드를 생성해준다.
> - 터미널에서 npx create-next-app my-first-next-app --use-npm 명령을 실행해서 next.js 앱을 실행시킨다.
> - 만약 보일러플레이트 코드 생성 방식을 사용하지 않는다면, 모든 의존성 패키지를 따로 추가한 다음 기본적인 디렉터리 구조를 추가하는 것만으로도 새로운 Next.js 애플리케이션을 만들 수 있다.

### 타입스크립트 지원

> 1. next.js는 타입스크립트로 작성된 프레임워크라서 태생적으로 고품질의 타입 정의를 지원한다.
>
> 2. next.js 앱에서 기본 언어를 타입스크립트로 지정하는 방법
>
> - 프로젝트의 최상위 디렉터리 안에 tsconfig.json이라는 타입스크립트 설정 파일만 만들면 된다.
> - 그리고 npm run dev 명령을 실행하면 된다.
>
> 3. next.js가 바벨의 @babel/plugin-transform-typescript를 사용해서 설정파일을 관리하기 때문에 주의사항을 숙지해야 한다.

# 1주차 (2023.08.31)

> 오늘은 첫 번째 시간을 맞아서 오리엔테이션을 했다.
>
> 1학기에는 react를 배웠지만 2학기에는 next.js 를 배운다 하였다.
>
> 수행평가는 1학기와 마찬가지로 GitHub에 매주 학습한 내용을 업로드한 결과를 보고 평가하신다고 하였다.
>
> 1학기와 다른 점이 있었는데 저장소를 private로 생성하였다.

### Next.js란?

> Angular, React, Vue 와 같은 프레임워크가 등장하면서 웹 개발
> 분야는 급속도로 변하기 시작하였다.
>
> 1. 리액트는 페이스북(메타)의 조던 발케가 만들어, 2013년 오픈소스를 발표한다.
>
> 2. 리액트는 클라이언트 사이드에서만 작동한다는 문제점이 있다.
>
> 3. 이 문제를 해결하기 위해 서버에서 미리 렌더링해 두는 방법을 연구하기 시작한다.
>
> 4. 이러한 연구의 결과로 나온 것이 Next.js 이다.
>
> 5. 이로써 리액트가 제공하지 않는 여러가지 기능을 제공하게 된다.

### Next.js가 제공하는 새로운 기능들

> 1. 코드 분할(Splitting): 페이지를 로딩 할 때 번들을 여러 조각으로 나누어 필요한 부분만 전송하는 방식
>
> 2. 서버 사이트 렌더링
>
> 3. 파일 기반 라우팅
>
> 4. 경로 기반 프리페칭(prefetching): 사용자가 다음에 이동할 수 있는 페이지를 미리 가져오는 기술.
>
> 5. 정적 사이트 생성
>
> 6. 증분 정적 콘텐츠 생성
>
> 7. 타입스크립트에 대한 기본 지원
>
> 8. 자동 폴리필(Polyfill) 적용: 이전 브라우저에서 최신 기능을 제공하는 데 필요한 코드를 제공
>
> 9. 이미지 최적화: Nect/image 컴포넌트로 제공하는 이미지의 최적화 기술
>
> 10. 웹 애플리케이션의 국제화 지원: 다국어 지원
>
> 11. 성능 분석

### Next.js와 비슷한 프레임워크

> [Gatsby]
>
> - 정적 웹 사이트를 만들 수 있는 프레임워크
> - 정적 사이트 생성만 지원
> - 클라이언트 사이드 렌더링만 지원
> - 동적으로 변하는 복잡한 웹 사이트는 만들 수 없다.

> [Razzle]
>
> - 서버 사이드 랜더링이 가능한 자바스크립트 애플리케이션 개발이 가능
> - CRA와 유사하게 프로젝트를 구성할 수 있다는 장점
> - React, Preact, Reason-React, Angular 및 Vue와 함께 사용

### Next.js 시작하기

> 개발 환경에는 Node.js와 npm만 설치하면 된다.
> node.js만 설치하면 npm은 함께 설치 된다.
> 버전에는 크게 영향을 받지 않을 것이다.
> 사용 중 의존성에 문제가 있다고 판단될 때 변경하면 된다.
