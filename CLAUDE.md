# CLAUDE.md - 프로젝트 가이드

이 파일은 Claude Code에 프로젝트 컨텍스트를 제공합니다.

## Project Context

### 프로젝트 개요
**개인 개발 블로그** - Notion을 CMS로 활용한 개인 기술 블로그

### 핵심 문서
- **PRD 문서**: @docs/PRD.md - 프로젝트 요구사항, 기능, 기술 스택, 데이터베이스 구조
- **개발 로드맵**: @docs/ROADMAP.md - 5단계 개발 계획, 각 Phase별 상세 일정 및 체크리스트

### 기술 스택
- **Frontend**: Next.js 15, TypeScript, React 19
- **Styling**: Tailwind CSS, shadcn/ui
- **CMS**: Notion API (@notionhq/client)
- **Icons**: Lucide React
- **Deployment**: Vercel

### 주요 기능
1. Notion 데이터베이스에서 블로그 글 목록 가져오기
2. 개별 글 상세 페이지 표시
3. 카테고리별 필터링
4. 검색 기능
5. 반응형 디자인

### 프로젝트 구조
```
notion-cms-project/
├── docs/
│   ├── PRD.md          # 프로젝트 요구사항 문서
│   └── ROADMAP.md      # 개발 로드맵
├── src/
│   ├── app/            # Next.js 앱 라우터
│   ├── components/     # React 컴포넌트
│   ├── lib/            # 유틸리티 및 타입
│   └── hooks/          # Custom hooks
├── public/             # 정적 파일
├── CLAUDE.md           # 이 파일
├── README.md           # 프로젝트 설명
├── .gitignore          # Git 설정
└── package.json        # 의존성 관리
```

### 개발 단계
현재 **Phase 1: 프로젝트 초기 설정** 준비 중

다음 단계별 개발 예정:
- Phase 1 (1-2일): 프로젝트 골격
- Phase 2 (2-3일): 공통 모듈
- Phase 3 (3-4일): 핵심 기능
- Phase 4 (2-3일): 추가 기능
- Phase 5 (1-2일): 최적화 및 배포

자세한 내용은 @docs/ROADMAP.md 참고

### 환경 설정
```
NOTION_API_KEY=your_notion_api_key
NOTION_DATABASE_ID=your_database_id
```

### 유용한 명령어
```bash
npm install          # 의존성 설치
npm run dev          # 개발 서버 실행
npm run build        # 프로덕션 빌드
npm start            # 프로덕션 서버 실행
npm run lint         # 코드 린팅
git push origin main # GitHub에 푸시
```

### GitHub 저장소
- **저장소**: https://github.com/figoo1984-spec/notion-cms-project
- **현재 상태**: 초기 설정 완료, Phase 1 준비 중

---

**마지막 업데이트**: 2026-10-29
