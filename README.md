# 강진선

# 13주차 (2023.12.07)

### SASS

> Next에서 기본적으로 지원하는 전 처리기 이다.
> 단 패키지 설치가 필요하다 $ npm install sass
> SASS 및 SCSS(Sassy CSS)문법으로 CSS Module을 만들고 사용할 수 있다.

### UI 라이브러리

> 라이브러리, 프레임워크, 유틸리티 기능이 필수는 아니다.
> 다만 생산성 향상 및 UI의 일괄성을 유지하는데 많은 도움을 받을 수 있다.

### Chakara UI

> 오픈소스 컴포넌트 라이브러리로, 모듈화 되어 있고 접근성이 뛰어나며 보기 좋은 UI를 만들 수 있다.
> 버튼, 모달, 입력 등 다양한 내장 컴포넌트를 제공한다.
> dark mode 및 light mode를 모두 지원한다.
> 기본 컴포넌트를 조합하여 새로운 컴포넌트를 쉽게 만들 수 있다.
> 타입스크립트로 작성되었으며 개발자에게 최고의 개발 경험을 제공한다.

### TailwindCSS

> 다른 프레임워크와는 다르게 css 규칙만을 제공한다
> 자바스크립트 모듈이나 리액트 컴포넌트를 제공하지 않기 때문에 필요한 경우 직접 만들어서 사용해야 한다.
> 변수값을 조정하여 개성있는 디자인을 만들 수 있다.
> dark mode 및 light mode를 쉽게 적용할 수 있다.
> 빌드 시점에 사용하지 않는 클래스는 제거 되기 때문에 높은 수준의 최적화를 지원한다.

### Headless UI

> tailwindCSS를 만든 팀의 무료 오픈소스 프로젝트이다.
> TailwindCSS는 웹 컴포넌트 안에서 사용할 수 있는 CSS클래스만 제공한다.
> 이런 단점을 보완하기 위해서 Headless UI가 탄생했다.
> Headless CSS

### 커스텀 서버가 필요한 경우

> 실제 웹 앱을 만들고 서비스를 제공할 때 Express.js나 Fastify서버에서 앱을 실행하는 경우는 드물다.
> 웹 앱을 기존의 서버에서 실행하는 경우, 멀티테넌지 지원이 필요한 경우, 더 세밀한 제어가 필요한 경우 커스텀 서버가 필요하다.

### 테스트

> 테스트는 개발에서 필수 과정이며, 세가지 단계로 나눌 수 있다.

> 1. 단위 테스트
>
> - 코드의 각 함수가 제대로 작동하는지 확인하는 테스트이다.

> 2. 엔드 투 엔드 테스트
>
> - 앱에 대한 사용자 상호 작용을 흉내내서 특정 작동이 발행했을 때 적절한 응답을 하는지 확인하는 테스트이다.
> - 폼 입력이나 CSS가 적절히 적용되는지 등을 테스트한다.

> 3. 통합 테스트
>
> - 함수나 모듈과 같이 서로 구분되는 영역이 함께 잘 작동하는지 확인하는 테스트이다. 서로 연관된 함수와 모듈을 한데 묶어서 주어진 입력에 맞는 적절한 출력을 만들어 내는지 확인한다.

### 테스트 러너

> 코드에서 모든 테스트를 찾고 테스트 결과를 수집하여 콘솔에 표시할 수 있는 것을 총칭하는 말이다.
> 테스트 러너 프로세스가 실패하거나 종료 시 반환값이 0이 아닌 경우 해당 테스트는 실패한 것으로 간주된다.
> Node.js와 자바스크립트 생태계에서는 다양한 테스트 러너를 제공한다.

# 12주차 (2023.11.30)

### Redux 추가하기

> <img width="1440" alt="스크린샷 2023-11-30 오후 3 15 30" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/d0d52f5f-f518-43a7-a073-2b6b12036dca">
> <img width="1440" alt="스크린샷 2023-11-30 오후 3 18 27" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/7aba2c89-b4f2-49e2-9bca-70344470e18a">

> 애플리케이션에서 데이터를 아무리 잘 구도화하고, 관리하고, 사용하고, 제공하더라도 애플리케이션 UI에 따라 화면에 제대로 보여주지 않는다면 아무 소용이 없다.

### CSS와 내장 스타일링 메서드

> 6장에서는 모듈화되고 유지 보수가 쉬우며 성능이 뛰어난 CSS스타일을 Next.js에 바로 적용할 수 있는 기법을 다룬다.

### Styled JSX

> SASS나 LESS 같은 새로운 스타일링 언어를 배우지 않고 자바스크립트와 CSS규칙을 함께 사용하고 싶다면 Style JSX가 좋은 선택이다.

> Styled JSX는 CSS-in-JS 라이브러리, 즉 CSS 속성 지정을 위해 자바스크립트를 사용할 수 있는 라이브러리이다.

> Next.js를 만든 Vercel에서 제공하며 특정 컴포넌트 스코프를 가지는 CSS 규칙이나 클래스를 만들 수 있다.

# 11주차 (2023.11.23)

### 지역 및 전역 상태 관리

> 상태는 동적 정보의 일종이다. 높은 수준의 상호 작용이 가능한 UI를 구현하거나, 더 뛰어난 UX 개발을 위한 필수 요소이다.

> 최신 웹앱에서는 UI가 state를 사용하고, 관리하는 경우가 많이 있다.
>
> - 밝은 테마에서 어두운 테마로 변경하거나, 배송 주소를 바꿈으로써 폼의 상태를 변경한다. 또한 버튼 클릭 만으로 앱의 상태를 변하게 할 수도 있다.

> 상태 관리 때문에 앱에 더 뛰어난 상호 작용 등의 기능을 구현할 수 있지만, 앱의 복잡도는 증가한다.

> 리액트 애플리케이션의 상태 관리에 있어 특히 어려운 점은 데이터의 흐름이 단방향이라는 것이다.
>
> - 부모 컴포넌트는 자식 컴포넌트에게 속성의 형태로 상태를 전달할 수 있지만 반대로 자식이 부모에게 상태를 전달할 수는 없다.
> - 지역 상태는 클래스 컴포넌트나 훅을 사용해서 별다른 어려움 없이 관리할 수 있지만 전역 상태는 단방향 데이터 흐름 때문에 정말 관리하기 힘들다.

### 지역 상태 관리

> 1. 아톰 컴포넌트
>
> - 아톰은 가장 흔히 접하는 리액트 컴포넌트이다. 이런 컴포넌트는 비교적 작은 크기의 지역 상태를 사용할 때가 많다. 더 큰 상태의 경우 molecules나 organisms와 같은 다른 단위로 옮긴다.

> 2. 로딩상태
>
> - 클라이언트 측에서 외부 데이터를 읽어올 때, 아직 데이터를 다 가져오지도 못했고 에러도 발생하지 않은 시점이 있다. 즉, 전송한 HTTP 요청이 아직 끝나지 않은 상태이다.
>   이런 경우 대개 loading 상태값을 true로 지정해서 데이터 전송 요청이 다 끝날 때까지 UI에 스피너 아이콘 등을 표시할 수 있다.

### 전역 상태 관리

> 애플리케이션의 전역 상태는 여러 컴포넌트들이 공유하는 상태를 의미한다.
> 뷰나 앵글러와는 다르게 리액트에서의 데이터 흐름은 단방향이다. 컴포넌트는 자식 컴포넌트에 데이터를 넘겨줄 수 있지만 반대로는 안된다.

### 콘텍스트 API

> 콘텍스트 API는 특정 콘텍스트 내의 모든 컴포넌트 간에 데이터를 공유할 수 있는 매우 직관적인 방법을 제공한다.
> 명시적으로 다른 컴포넌트에 속성값 형태로 데이터를 전달할 필요도 없고 심지어 자식 컴포넌트가 부모 컴포넌트에게 데이터를 공유할 수도 있다.

> <img width="1440" alt="스크린샷 2023-11-23 오후 4 37 56" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/9dd81e27-c838-4798-9946-cb878ad8a299">

# 10주차 (2023.11.16)

### GraphQL API

> 2012년에 메타에서 개발했다. API에서 사용할 수 있는 질의어로 REST나 SOAP 같은 방식과는 다른 새로운 관점으로 API 데이터를 다룬다.
> 꼭 필요한 데이터만 불러오도록 지정할 수 있다.
> 한 번의 요청으로 여러 곳의 데이터를 불러올 수 있다.
> 사용할 데이터에 대해 정적이면서도 강력한 타입 시스템을 제공한다.

> <img width="1440" alt="스크린샷 2023-11-18 오전 12 27 07" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/7fd20457-bfa9-46a5-ab05-2d88e2df42ca">

# 9주차 (2023.11.09)

### 스타일 파일 구성

> 스타일 파일은 Next.js 애플리케이션에서 어떤 스타일 관련 기술을 사용하는가에 따라 그 구성이 달라진다. Emotion, styled-components, JSS와 같은 CSS-in-JS 프레임워크 경우 컴포넌트별로 스타일 파일을 만든다. 그래서 스타일은 변경하기도 쉽다.

### lib 파일 구성

> lib 파일은 서드파티 라이브러리를 감싸는 스크립트를 지칭하는 말이다.

### 서버에서 REST API 사용하기

> <img width="1440" alt="스크린샷 2023-11-09 오후 2 42 32" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/a9317e34-e3e6-4ac8-8d7a-d6df570a49a4">

### 클라이언트에서 REST API 사용하기

> Next.js에서는 내장 getServerSideProps나 getStaticProps 함수 내에서 REST API를 호출하면 서버가 데이터를 가져오지만 그 외의 컴포넌트 내에서 데이터를 불러오는 작업은 클라이언트가 실행한다.

# 8주차 (2023.11.02)

### 코드 구성과 데이터 불러오기

> 4장 (86p)에서 알아볼 내용은 아토믹 디자인 원칙에 따른 컴포넌트 구성, 유틸리티 구성, 정적 자원 구성, 스타일 파일 구성, lib 파일 구성, 서버에서 REST API를 사용하는 방법, 클라이언트에서 REST API를 사용하는 방법, 클라이언트 및 서버에서 Apollo를 이용하여 GraphQL API를 사용하는 방법을 배울 것이다.

### 디렉터리 구조 구성

> 애플리케이션의 코드를 쉽게 유지 보수하고 확장하려면 프로젝트의 디렉터리 구조를 간결하고 분명하게 구성하고 유지하는 것이 무엇보다 중요하다.
> Next.js에서는 특정 파일과 디렉터리가 지정된 위치에 있어야 한다.
> \_app,js, \_document.js, pages/와 public/ 디렉터리 등이 그렇다.

> 1. node_modules/ : Next.js 프로젝트의 의존성 패키지를 설치하는 디렉터리
> 2. pages/ : 웹 애플리케이션의 페이지 파일을 저장하고 라우팅 시스템을 만드는 디렉터리
> 3. public/ : 컴파일된 CSS 및 자바스크립트 파일, 이미지, 아이콘 등의 정적 자원을 저장하고 제공하는 디렉터리
> 4. styles/ : 스타일링 포맷(CSS, SASS, LESS 등)과 관계없이 스타일링 모듈을 저장하는 디렉터리

### 컴포넌트 구성

> 1. atoms
>
> - 코드에서 사용되는 가장 기본적인 컴포넌트들이다.
> - button, input, p와 같은 표준 HTML 요소를 감싸는 용도로 사용되거나, 애니메이션 또는 컬러 팔레트 등과 같은 용도로 사용되는 컴포넌트를 이곳에 옮겨서 저장한다.
>
> 2. molecules
>
> - atoms에 속한 컴포넌트 여러 개를 조합하여 좀 더 복잡한 구조를 만드는 컴포넌트이다.
> - 유틸리티 기능들은 많이 사용되지 않는다.
>
> 3. organisms
>
> - molecules와 atoms를 섞어서 더 복잡한 구조의 컴포넌트를 만든다.
> - 회원 가입 양식이나 푸터, 캐러셀 등이 이에 속한다.
>
> 4. templates
>
> - 일종의 페이지 스켈레톤으로, 어디에 organisms, atoms, molecules를 배치할지 결정해서 사용자가 접근할 수 있는 페이지를 만든다.

### 유틸리티 구성

> 컴포넌트를 만들지 않는 코드 파일이 있다. 이런 파일을 흔히 유틸리티 스크립트라고 한다.

### 정적 자원 구성

> 정적 자원을 구성하기 전에 Next.js 애플리케이션에서 어떤 정적 파일을 제공해야 할지 파악할 필요가 있다. 일반적인 웹 사이트에서는 다음과 같은 정적 자원을 사용한다.
>
> 1. 이미지
> 2. 컴파일한 CSS파일
> 3. 아이콘(facivon 및 웹 앱 아이콘)
> 4. manifest.json,robot.txt 등의 정적 파일

# 7주차 (2023.10.26)

### 메타 데이터

> 페이스북의 오픈 그래프처럼 공유 자료를 카드 형태로 보내려면 메타 데이터를 추가해야 한다
> Next.js에서는 내장 Head 컴포넌트를 제공하여 이런 메타 데이터를 쉽게 다룰 수 있다.
> 어떤 컴포넌트에서든 HTML 페이지의 <Head> 내부 데이터를 변경, 추가, 삭제할 수 있다.

> <img width="1440" alt="스크린샷 2023-10-26 오후 3 11 32" src="https://github.com/jinseonKang/React2-3-1/assets/126742685/89bbd9cd-c411-4e19-b1a0-7e037e155859">

### \_app.js와 \_document.js 페이지 커스터마이징

> 웹 애플리케이션에 따라 페이지 초기화 과정을 조절해야 하는 경우가 있다.
> 이 경우 페이지를 렌더링할 때마다 렌더링한 HTML을 클라이언트로 보내기 전에 특정 작업을 처리해야 한다.

### document.js 페이지

> Next.js 페이지 컴포넌트에서는 <head>, <html>, <body> 와 같은 기본적인 HTML 태그를 정의할 필요가 없다.

> 1. Html
>
> - Next.js 애플리케이션의 <html> 태그에 해당한다. 여기에 lang과 같은 표준 HTML 속성들을 전달할 수 있다.

> 2. Head
>
> - 애플리케이션의 모든 페이지에 대한 공통 태그를 정의할 때 이 컴포넌트를 사용할 수 있다. 이 Head 컴포넌트는 이전에 살펴본 Head 컴포넌트와 다르다. 개념은 비슷하지만 여기서의 Head는 반드시 웹 사이트의 모든 페이지에서 공통으로 사용되는 코드가 있을 때만 사용할 수 있다.

> 3. Main
>
> - Next.js가 페이지 컴포넌트를 렌더링하는 곳이다. <Main> 외부의 컴포넌트는 브라우저에서 초기화되지 않기 때문에 페이지 간에 공통으로 사용되는 컴포넌트가 있다면 반드시 \_app.js 파일에서 해당 컴포넌트를 사용해야 한다.

> 4. NextScript
>
> - Next.js는 클라이언트에 전송할 페이지를 렌더링하고, 클라이언트에서 실행할 코드나 리액트 하이드레이션과 같은 작업을 처리할 수 있는 커스텀 스크립트를 끼워넣는다. NextScript는 이런 커스텀 자바스크립트가 위치하는 곳이다.

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
