# Vuetilog (뷰티로그)
Vue와 Vuetify로 만든 블로거 테마

## 공지
0.0.8 버젼 이상을 사용해주세요. 테스팅 후에 적용된 SEO 관련 업데이트가 들어있습니다.

## 다른 언어:
[English](https://github.com/opdev1004/vuetilog)

## 예시
[https://vuetilog.blogspot.com/](https://vuetilog.blogspot.com/)

## 다운로드
[https://github.com/opdev1004/vuetilog/releases/](https://github.com/opdev1004/vuetilog/releases/)

## 기능:
1. Vue와 Vuetify로 개발 가능
2. 반응형 웹 디자인
3. SEO
4. 나은 라벨 컨트롤

## 설치:
1. Contempo 테마를 블로그에 적용
2. vuetilog.xml로 테마를 복구하거나 HTML 수정을 통해 테마를 붙여넣고 저장
3. 필요에 따라 설정 수정

### 포스트에서 코드 스타일 사용하는 방법
1. 에디터에서 마우스로 드래그하여 코드를 선택(Select)합니다
2. 선택된 코드들을 단락형식에서 보통으로 바꿉니다.
3. 에디터를 HTML 보기로 변경합니다
4. 코드 div 요소의 클래스를 "code"로 설정합니다. 예시.```class="code"``` 

### 레이아웃 시스템
| 섹션 | 설명 |
| - | - |
| Nav Top | 사이드바 전용 위젯을 추가할 수 있습니다. |
| Label Section | 라벨 위젯만 추가해주세요. |
| Nav Bottom | 사이드바 전용 위젯을 추가할 수 있습니다. |
| Main Content Top | 메인에 사용 될 수 있는 위젯을 추가 할 수 있습니다. 예시: 광고 위젯. |
| Main Content Bottom | 메인에 사용 될 수 있는 위젯을 추가 할 수 있습니다. 예시: 광고 위젯. |
| Components | 테마 개발자를 위한 섹션입니다. Vue 컴포넌트가 되기위해 많이 개조될 위젯들이 이곳에 놓여집니다. |
| Bottom Section | footer 전용 위젯을 추가할 수 있습니다. |

## 참여하기
Vuetilog를 발전시키는 것을 환영합니다.
이 깃헙 저장소에 Pull Request를 열어주세요.

## 라이센스:
MIT

## 테마 개발 디테일
### 테마 로드 순서
1. 블로거 시스템이 Vuetilog 테마로부터 HTML파일 생성
2. 웹브로우저가 블로그 페이지 로드
3. head 태그에서 Vue, Vuetify, CSS 등등을 로드
4. 컴포넌트화 될 요소들이 담긴 id='init-wrapper' div 태그를 훑고 지나감
5. Vue 앱 템플릿을 훑고 지나감
6. Vue로 로딩 오버레이 생성
7. id='init-wrapper' div 태그 안 요소들을 컴포넌트화
8. 컴포넌트들과 데이터와 함께 Vue 앱 생성
9. init-wrapper div 태그 제거
10. 로딩 오버레이 제거

### Vue와 Vuetify 사용방법
컴포넌트와 Vue 템플릿의 일부분이라면 정상적으로 로드됩니다.

### Vuetilog 컴포넌트
| 컴포넌트 | 위치 | 설명 |
| - | - | - |
| nav-top | Left Navigation Drawer | 사이드바 위젯들을 위한 컴포넌트 |
| label-section | Left Navigation Drawer | 라벨만을 보유하기 위한 컴포넌트 |
| nav-bottom | Left Navigation Drawer | 사이드바 위젯들을 위한 컴포넌트 |
| main-content-top | Main Page | 메인 위젯들을 위한 컴포넌트 |
| main-content-bottom | Main Page | 메인 위젯들을 위한 컴포넌트 |
| pagination | Main Page | 페이지 네비게이션 컴포넌트 |
| posts | Main Page | 포스트, 페이지 컴포넌트 |
| comments | Main Page | 댓글 컴포넌트 |
| post-feeds | Main Page | 피드 링크 컴포넌트 |
| popular-posts | Main Page | 포스트에 사용 되기위한 인기 포스트 컴포넌트 |
| featured-post | Main Page | 포스트에 사용 되기위한 추천 포스트 컴포넌트 |
| bottom-section | Main Page | Footer 위젯들을 위한 컴포넌트 |
