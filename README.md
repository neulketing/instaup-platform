# 🚀 INSTAUP - SNS 마케팅 플랫폼
> 실제 한국인 SNS 마케팅 서비스를 제공하는 현대적인 웹 플랫폼

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue)](https://github.com/neulketing/instaup-platform)
[![Railway](https://img.shields.io/badge/Railway-Backend-success)](https://railway.app)
[![Netlify](https://img.shields.io/badge/Netlify-Frontend-brightgreen)](https://netlify.app)

## 📁 프로젝트 구조

```
📦 INSTAUP-PLATFORM
├── 🖥️ instaup-backend/           # Node.js + Express + Prisma 백엔드
│   ├── src/                      # 소스 코드
│   ├── prisma/                   # 데이터베이스 스키마
│   ├── package.json             # 백엔드 의존성
│   ├── railway.json             # Railway 배포 설정
│   └── README.md                # 백엔드 문서
│
├── 🎨 instaup-clean/            # React + Vite 프론트엔드 (메인 서비스)
│   ├── src/                     # 소스 코드
│   ├── public/                  # 정적 파일
│   ├── package.json            # 프론트엔드 의존성
│   ├── netlify.toml            # Netlify 배포 설정
│   └── README.md               # 프론트엔드 문서
│
├── 🎨 instaup-modern/          # React + Vite 프론트엔드 (모던 버전)
│   ├── src/                    # 소스 코드
│   └── package.json           # 의존성
│
├── 📁 archive/                 # 레거시 & 참고용 코드
│   ├── snsshop-clone/         # 참조용 SNS샵 클론
│   ├── phases/                # 단계별 개발 계획
│   └── TODO.md               # 과거 할일 목록
│
├── 📁 docs/                   # 프로젝트 문서
├── 🎯 uploads/                # 업로드된 이미지 파일들
├── .github/                   # GitHub Actions & 워크플로우
└── README.md                  # 메인 프로젝트 문서
```

## 🚀 빠른 시작

### 백엔드 실행
```bash
cd instaup-backend
bun install
bun run dev
```

### 프론트엔드 실행 (메인)
```bash
cd instaup-clean
bun install
bun run dev
```

### 프론트엔드 실행 (모던)
```bash
cd instaup-modern
bun install
bun run dev
```

## 🛠️ 기술 스택

### 백엔드
- **Node.js** + **Express.js** - 서버 프레임워크
- **Prisma** - ORM 및 데이터베이스 관리
- **TypeScript** - 타입 안전성
- **Railway** - 배포 플랫폼

### 프론트엔드
- **React** + **Vite** - UI 프레임워크
- **TypeScript** - 타입 안전성
- **Tailwind CSS** - 스타일링
- **shadcn/ui** - UI 컴포넌트
- **Netlify** - 배포 플랫폼

## 📈 주요 기능

- ✅ **인스타그램 팔로워 관리**
- ✅ **실시간 통계 대시보드**
- ✅ **사용자 인증 시스템**
- ✅ **결제 시스템 통합**
- ✅ **반응형 웹 디자인**
- ✅ **관리자 패널**

## 🌐 배포

### 프로덕션 환경
- **백엔드**: Railway ([배포 가이드](./instaup-backend/RAILWAY_DEPLOY_GUIDE.md))
- **프론트엔드**: Netlify ([배포 가이드](./instaup-clean/DEPLOYMENT_GUIDE.md))

### 개발 환경
- **백엔드**: `localhost:3000`
- **프론트엔드**: `localhost:5173`

## 📝 프로젝트 진행 상황

### ✅ 완료된 작업
- [x] 백엔드 API 서버 구축 (Express + Prisma)
- [x] 프론트엔드 UI 완성 (React + Tailwind)
- [x] 사용자 인증 시스템
- [x] 데이터베이스 스키마 설계
- [x] 배포 환경 구성
- [x] CI/CD 파이프라인

### 🔄 진행 중
- [ ] 고급 기능 추가
- [ ] 성능 최적화
- [ ] 테스트 커버리지 향상

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 `LICENSE` 파일을 참조하세요.

## 👥 팀

- **개발자**: [@neulketing](https://github.com/neulketing)
- **AI 어시스턴트**: Same AI

---

**🚀 Same AI로 개발된 프로젝트**
