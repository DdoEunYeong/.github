# DdoEunYeong (또 오은영!)

🏆 **숭실대학교 2025 스파르탄 위닝 창업캠프 우수상 수상**

아이코지: 아동 상담 및 감정 분석을 위한 통합 플랫폼

<img width="638" height="878" alt="image" src="https://github.com/user-attachments/assets/d6cf9342-afc6-488e-9183-b5a9d5f7f5ad" />

## 📋 프로젝트 개요

DdoEunYeong은 AI 기반 감정 분석과 음성 인식을 활용하여 아동의 심리 상태를 분석하고 상담 서비스를 제공하는 웹 애플리케이션입니다.

## 🏗️ 프로젝트 구조

```
DdoEunYeong/
├── ai/                    # AI 서버 (FastAPI)
├── backend/              # 백엔드 서버 (Spring Boot)
└── frontend/             # 프론트엔드 (Next.js)
```

## 🛠️ 기술 스택

### Frontend
- **Framework**: Next.js 15.2.4
- **Language**: TypeScript 5
- **UI Library**: React 19
- **Styling**: Tailwind CSS 3.4.17
- **UI Components**: 
  - Radix UI (접근성 우선 컴포넌트)
  - shadcn/ui (컴포넌트 시스템)
- **Form Management**: React Hook Form 7.54.1
- **Validation**: Zod 3.24.1
- **Charts**: Recharts 2.15.0
- **PDF Generation**: jsPDF 3.0.1
- **Canvas**: html2canvas 1.4.1
- **Voice Activity Detection**: @ricky0123/vad-web 0.0.24
- **Text-to-Speech**: Web Speech API (speechSynthesis)
- **Icons**: Lucide React 0.454.0
- **Theme**: next-themes 0.4.4

### Backend
- **Framework**: Spring Boot 3.3.2
- **Language**: Java 17
- **Build Tool**: Gradle
- **Database**: 
  - MySQL (메인 데이터베이스)
  - Redis (세션 관리, 캐싱)
- **ORM**: Spring Data JPA
- **Query**: QueryDSL 5.0.0
- **Security**: 
  - Spring Security
  - JWT (JSON Web Token)
  - OAuth2 Client
- **WebSocket**: Spring WebSocket
- **HTTP Client**: WebClient, Apache HttpClient5
- **Cloud Storage**: AWS S3
- **Computer Vision**: JavaCV 1.5.10
- **API Documentation**: SpringDoc OpenAPI 2.5.0
- **Code Generation**: Lombok

### AI Server
- **Framework**: FastAPI 0.111.0
- **Language**: Python
- **ASGI Server**: Uvicorn 0.29.0
- **Emotion Analysis**: 
  - DeepFace 0.0.83
  - TensorFlow 2.11.0
  - OpenCV 4.10.0.82
- **Speech-to-Text**: ElevenLabs API
- **Image Processing**: NumPy, OpenCV
- **Environment**: python-dotenv 1.0.1

## 🚀 주요 기능

### 1. 사용자 관리
- 회원가입/로그인 (JWT 기반 인증)
- 사용자 프로필 관리

### 2. 아동 프로필 관리
- 아동 정보 등록 및 관리
- 성별, 나이 등 기본 정보 관리

### 3. AI 기반 감정 분석
- DeepFace 라이브러리를 활용한 실시간 얼굴 감정 분석
- 감정 점수 및 지배적 감정 제공

### 4. 음성 인식 및 분석
- ElevenLabs STT API를 활용한 음성-텍스트 실시간 변환
- 실시간 음성 활동 감지 (VAD)
- Web Speech API를 활용한 텍스트-음성 변환 (TTS)

### 5. 상담 서비스
- 웹소켓 및 AI 기반 상담 세션
- 상담 결과 리포트 자동 생성

### 6. 데이터 관리
- 사용자 상담 영상 데이터 저장
- 상담 기록 관리
- 감정 분석 결과 저장 및 추적

## 📁 주요 디렉토리 설명

### `/ai/`
- FastAPI 기반 AI 서버
- 감정 분석(Deepface) 및 STT(ElevenLabs) 기능 제공

### `/backend/`
- Spring Boot 기반 REST API 서버
- JPA를 활용한 데이터 관리
- WebSocket을 통한 실시간 영상/음성 통신
- AWS S3 연동
- GPT API를 활용해 상담 결과 분석
- Gemini API를 활용해 사진 누끼 처리

### `/frontend/`
- Next.js 기반 웹 애플리케이션
- 반응형 UI/UX
- 실시간 음성/영상 처리
