# Electron Vue3 Hello World

Electron과 Vue3를 사용하여 만든 간단한 데스크탑 애플리케이션입니다. "Hello World"를 화면에 표시합니다.

## 기능

- Vue3 기반의 사용자 인터페이스
- Electron을 통한 크로스 플랫폼 데스크탑 앱
- Vite를 사용한 빠른 개발 환경

## 요구사항

- Node.js (v16 이상 권장)
- npm 또는 yarn

## 설치

1. 저장소를 클론합니다:
   ```bash
   git clone <repository-url>
   cd electron-test
   ```

2. 의존성을 설치합니다:
   ```bash
   npm install
   ```

## 실행 방법

### 개발 모드

개발 중에 실시간으로 변경사항을 확인하려면 다음 명령을 사용하세요:

```bash
npm run electron-dev
```

이 명령은 Vite 개발 서버와 Electron 앱을 동시에 실행합니다. 코드 변경 시 자동으로 리로드됩니다.

### 프로덕션 빌드 및 실행

1. Vue 앱을 빌드합니다:
   ```bash
   npm run build
   ```

2. Electron 앱을 실행합니다:
   ```bash
   npm run electron
   ```

### 배포용 실행 파일 생성

프로젝트를 실행 파일로 패키징하려면:

```bash
npm run dist
```

이 명령은 플랫폼별 설치 파일을 `dist-electron` 폴더에 생성합니다.

## 프로젝트 구조

```
electron-test/
├── src/                    # Vue 앱 소스 코드
│   ├── App.vue            # 메인 Vue 컴포넌트
│   └── main.js            # Vue 앱 진입점
├── main.js                # Electron 메인 프로세스
├── index.html             # 메인 HTML 파일
├── package.json           # 프로젝트 설정 및 의존성
├── vite.config.js         # Vite 설정
└── dist-electron/         # 빌드된 실행 파일들
```

## 개발자 노트

- Vue3 Composition API를 사용합니다
- Electron의 메인 프로세스와 렌더러 프로세스가 분리되어 있습니다
- Vite를 통해 빠른 HMR(Hot Module Replacement)을 지원합니다

## 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다.