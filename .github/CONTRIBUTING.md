# 🤝 Contributing to INSTAUP

INSTAUP 프로젝트에 기여해주셔서 감사합니다! 이 가이드는 프로젝트에 효과적으로 기여하는 방법을 설명합니다.

## 📋 목차
- [시작하기](#시작하기)
- [개발 환경 설정](#개발-환경-설정)
- [기여 방법](#기여-방법)
- [코드 스타일](#코드-스타일)
- [커밋 메시지](#커밋-메시지)
- [Pull Request](#pull-request)

## 🚀 시작하기

### 1. Repository Fork
```bash
# 1. GitHub에서 repository fork
# 2. 로컬에 clone
git clone https://github.com/your-username/instaup-platform.git
cd instaup-platform

# 3. upstream remote 추가
git remote add upstream https://github.com/neulketing/instaup-platform.git
```

### 2. 개발 환경 설정

**Backend 설정:**
```bash
cd instaup-backend
npm install
cp .env.example .env
# .env 파일 설정
npm run dev
```

**Frontend 설정:**
```bash
cd instaup-clean
bun install
bun run dev
```

## 🔧 기여 방법

### 🐛 Bug Reports
1. [Bug Report 템플릿](.github/ISSUE_TEMPLATE/bug_report.md) 사용
2. 재현 가능한 단계 제공
3. 환경 정보 포함
4. 스크린샷 첨부 (가능시)

### ✨ Feature Requests
1. [Feature Request 템플릿](.github/ISSUE_TEMPLATE/feature_request.md) 사용
2. 사용 사례 명확하게 설명
3. 기대되는 동작 설명

### 💻 Code Contributions

#### 브랜치 명명 규칙
```
feature/기능명     # 새로운 기능
bugfix/이슈명     # 버그 수정
hotfix/긴급수정   # 핫픽스
docs/문서업데이트  # 문서 변경
refactor/리팩토링 # 코드 리팩토링
```

#### 개발 워크플로우
```bash
# 1. 최신 코드 동기화
git checkout main
git pull upstream main

# 2. 새 브랜치 생성
git checkout -b feature/your-feature-name

# 3. 개발 진행
# ... 코드 작성 ...

# 4. 테스트
npm run test        # Backend
bun run test       # Frontend

# 5. 커밋
git add .
git commit -m "feat: add new feature"

# 6. 푸시 및 PR
git push origin feature/your-feature-name
```

## 🎨 코드 스타일

### TypeScript/JavaScript
- **Linting**: ESLint + Prettier 사용
- **Naming**: camelCase (변수, 함수), PascalCase (컴포넌트, 클래스)
- **Import 순서**: external → internal → relative

```typescript
// ✅ Good
import React from "react"
import { Button } from "@/components/ui/button"
import { getUserData } from "../utils/api"

// ❌ Bad
import { getUserData } from "../utils/api"
import React from "react"
import { Button } from "@/components/ui/button"
```

### React Components
```tsx
// ✅ Good
interface UserCardProps {
  user: User
  onEdit: (id: string) => void
}

export const UserCard: React.FC<UserCardProps> = ({ user, onEdit }) => {
  return (
    <div className="rounded-lg border p-4">
      <h3 className="text-lg font-semibold">{user.name}</h3>
      <Button onClick={() => onEdit(user.id)}>Edit</Button>
    </div>
  )
}
```

## 📝 커밋 메시지

**Conventional Commits** 규칙을 따릅니다:

```
type(scope): description

[optional body]

[optional footer]
```

### 타입
- `feat`: 새로운 기능
- `fix`: 버그 수정
- `docs`: 문서 변경
- `style`: 코드 스타일 변경
- `refactor`: 리팩토링
- `test`: 테스트 추가/수정
- `chore`: 기타 변경사항

### 예시
```
feat(auth): add social login functionality

- Add Google OAuth integration
- Add Facebook login button
- Update login page UI

Closes #123
```

## 🔍 Pull Request

### PR 체크리스트
- [ ] 이슈와 연결됨
- [ ] 테스트 추가/업데이트
- [ ] 문서 업데이트 (필요시)
- [ ] 코드 리뷰 요청
- [ ] CI/CD 통과

### PR 규칙
1. **작은 단위로 분할**: 하나의 PR은 하나의 목적
2. **명확한 제목**: 변경사항을 한 줄로 요약
3. **상세한 설명**: 왜, 무엇을, 어떻게 변경했는지
4. **테스트 포함**: 새로운 기능에는 테스트 필수

## 🧪 테스트

### Backend Tests
```bash
cd instaup-backend
npm run test          # 단위 테스트
npm run test:e2e      # E2E 테스트
npm run test:coverage # 커버리지
```

### Frontend Tests
```bash
cd instaup-clean
bun run test          # 단위 테스트
bun run test:coverage # 커버리지
```

## 📚 추가 리소스

- [프로젝트 README](./README.md)
- [API 문서](./instaup-backend/README.md)
- [Frontend 가이드](./instaup-clean/README.md)
- [배포 가이드](./instaup-clean/DEPLOYMENT_GUIDE.md)

## 🙋‍♂️ 도움이 필요하신가요?

- 🐛 **버그**: [Bug Report](https://github.com/neulketing/instaup-platform/issues/new?template=bug_report.md)
- ✨ **기능 요청**: [Feature Request](https://github.com/neulketing/instaup-platform/issues/new?template=feature_request.md)
- 💬 **질문**: [Discussions](https://github.com/neulketing/instaup-platform/discussions)
- 📧 **연락**: [@neulketing](https://github.com/neulketing)

---

**🚀 함께 만들어가는 INSTAUP!**  
**Made with ❤️ by the community**
