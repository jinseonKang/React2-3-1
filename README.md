# 202130301 강진선

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
