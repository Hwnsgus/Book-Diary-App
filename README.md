📖 Book Diary App: 독서 기록 및 AI 기반 맞춤 도서 추천 iOS 앱

🌟 프로젝트 개요

Book Diary는 사용자가 매일 작성하는 **독서 감상문(일기)**을 기반으로 **AI(ChatGPT)**가 개인 맞춤형 도서를 추천해주는 혁신적인 iOS 애플리케이션입니다.

사용자의 감상문에서 핵심 감정, 주제, 키워드를 추출하여 ChatGPT API로 심층 분석하고, 그 결과에 기반한 관련 도서 정보와 함께 구매/참고 웹사이트 링크를 제공합니다. SwiftUI를 이용한 직관적이고 사용자 친화적인 UI와 Firebase를 활용한 안정적인 사용자 관리 및 데이터 동기화 기능을 제공합니다.

✨ 주요 기능 (Features)

기능

설명

독서 기록 관리

책 제목, 저자, 감상문, 별점(평점) 등 독서 기록의 생성, 수정 및 삭제 기능 제공

💡 AI 도서 추천

사용자의 감상문 분석을 통해 핵심 키워드를 도출하고, 이를 바탕으로 개인화된 도서 추천 문구 생성 (OpenAI ChatGPT API 활용)

🗓 커스텀 캘린더

날짜별 독서 기록 현황을 한눈에 확인하고, 사용자의 독서 패턴을 시각적으로 파악할 수 있는 캘린더 UI 제공

🧭 탭바 네비게이션

SwiftUI 기반의 MainTabBarView를 통해 주요 기능 간의 쉬운 이동 제공 (Home / Add / Recommend / MyPage)

🔐 회원가입 및 로그인

Firebase Authentication을 활용한 안전하고 간편한 계정 관리 시스템 구축

☁️ 데이터 동기화

Cloud Firestore를 사용하여 모든 독서 기록을 클라우드에 저장하고, 여러 디바이스 간의 데이터 동기화 지원

🛠 개발 환경 및 기술 스택 (Tech Stack)

구분

기술 / 도구

상세 설명

언어

Swift

iOS 애플리케이션 개발의 기본 언어

UI

SwiftUI

선언적 구문을 활용한 직관적이고 모던한 사용자 인터페이스 구축

아키텍처

MVVM, Combine

Model-View-ViewModel 패턴 적용으로 코드 분리 및 테스트 용이성 확보. 비동기 데이터 처리 및 상태 관리에 Combine 프레임워크 활용

AI

OpenAI ChatGPT (API)

사용자 감상문 분석 및 도서 추천 문구 생성을 위한 LLM (Large Language Model) API 연동

백엔드/DB

Firebase (Firestore, Auth)

실시간 데이터베이스(Firestore) 및 사용자 인증(Authentication) 솔루션 활용

IDE

Xcode 15

개발 환경 (iOS 16.0+ 권장)

패키지 관리

Swift Package Manager

종속성 관리 및 빌드 시스템 구축

버전 관리

Git / GitHub

형상 관리 및 협업 도구

🚀 설치 및 실행 (Installation & Run)

리포지토리 클론:

git clone [Your Repository URL]


Firebase 설정:

Firebase 프로젝트를 생성하고, GoogleService-Info.plist 파일을 프로젝트 루트 디렉토리에 추가합니다.

Firestore와 Authentication 서비스를 활성화합니다.

OpenAI API 키 설정:

프로젝트 내에 API 키를 관리할 수 있는 환경 변수 또는 Configuration 파일을 생성하고, 발급받은 ChatGPT API Key를 설정합니다.

패키지 종속성 설치:

# Xcode가 자동으로 Swift Package Manager 종속성을 resolve 합니다.


실행:

Xcode에서 프로젝트를 열고, 시뮬레이터 또는 실제 디바이스(iOS 16.0 이상)를 선택하여 빌드 및 실행합니다.