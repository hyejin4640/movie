#react movie 프로젝트

## Styling the Component
컴퍼넌트의 스타일을 변경하는 방법은 기존의 css를 적용하는 방법 또는 style={{}}을 사용하여 자바스크립트 형식으로도 적용이 가능하다. eg. style={{ backgroundColor: "red" }}로 표현
컴퍼넌트에선 기존의 class 대신 className을 사용하여 css클래스를 적용한다.

## Github page에 배포하기
Github pages 패키지 설치 npm i gh-pages
package.json파일에 homepage 및 배포할 Github 페이지 주소 추가
package.json파일 -> scripts 하위에 deploy항목 추가 gh-pages -d {$directory-name}
package.json파일 -> scripts 하위에 predeploy항목 추가 npm run build
terminal에서 npm run deploy 명령

##라우터
ReactJS의 url 라우팅 기능
*Router와 Route 컴퍼넌트 사용
같은 url상 그룹의 주소일 경우 모든 컴퍼넌트를 렌더링한다.
exact={true}로 정확하게 같은 해당 주소일 경우 컴퍼넌트를 렌더링 할 수 있게 한다.
Router에는 종류가 다양하며 (HashRouter, BrowserRouter 등) 각각 라우팅되는 방식이 다르다
라우팅 시에는 <a>태그 대신 react-router-dom의 Link 컴퍼넌트를 사용하여 라우팅 하라 -- <a>태그는 페이지 전체를 refresh 해버리기 때문에 제대로 동작하지 않았다.
Link 컴퍼넌트는 *Router 컴퍼넌트 내에 위치해야한다.
