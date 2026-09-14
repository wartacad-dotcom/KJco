# 종민님 1회성 설정 체크리스트 (GitHub Pages SEO 블로그)

아래 항목은 계정/권한과 직결되어 기술팀장이 대신 수행하지 않습니다. 종민님이 직접 진행해 주세요.
완료 후 기술팀에 "완료" 알려주시면 이후 자동화 연결을 진행합니다.

## 1. GitHub 계정 확인/생성
- [ ] 기존 GitHub 계정이 있는지 확인. 없다면 https://github.com/signup 에서 무료 계정 생성.
- [ ] 계정 이메일은 회사 대표 이메일(wartacad@gmail.com) 또는 별도 지정 이메일 중 선택.

## 2. 새 저장소 생성
- [ ] GitHub에서 새 저장소 생성 (예: `idea-developer-blog`). **Public**으로 생성 (GitHub Pages 무료 사용 조건 — Private 저장소는 무료 요금제에서 Pages 미지원).
- [ ] 저장소 이름을 `기술팀/SEO블로그/_config.yml`의 `baseurl` 값과 동일하게 맞춰주세요. (현재 플레이스홀더: `idea-developer-blog`)

## 3. 로컬 파일 업로드 (최초 1회)
- [ ] `C:\Users\종민\Desktop\킹종컴퍼니\기술팀\SEO블로그\` 폴더 내용을 새 저장소에 push.
  - 이 환경에 git이 설치되어 있지 않다면 https://git-scm.com/download/win 에서 설치.
  - 예시 명령 (저장소 생성 후 GitHub이 안내하는 명령과 동일):
    ```
    cd "C:\Users\종민\Desktop\킹종컴퍼니\기술팀\SEO블로그"
    git init
    git add .
    git commit -m "chore: initial Jekyll scaffold"
    git branch -M main
    git remote add origin https://github.com/<계정명>/idea-developer-blog.git
    git push -u origin main
    ```

## 4. GitHub Pages 활성화
- [ ] 저장소 → Settings → Pages 이동.
- [ ] Source: "Deploy from a branch" 선택, Branch: `main` / `/(root)` 선택 후 Save.
- [ ] 몇 분 후 `https://<계정명>.github.io/idea-developer-blog/` 접속 확인.

## 5. 인증 수단 준비 (향후 자동 push용)
자동화가 파일 생성 후 git push까지 무인으로 하려면 인증 수단이 필요합니다. 아래 중 하나를 선택해 준비해 주세요.
- [ ] **옵션 A (권장): Personal Access Token(PAT) 발급**
  - GitHub 우측 상단 프로필 → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token.
  - Repository access: 해당 저장소만 선택 (최소 권한 원칙).
  - Permissions: `Contents: Read and write` 만 부여.
  - 만료 기한 설정 권장 (예: 90일, 만료 시 재발급).
  - 발급된 토큰은 안전한 곳(예: Windows 자격 증명 관리자, 1Password 등)에 보관하고 기술팀에는 토큰 "값"이 아니라 "등록 완료 여부"만 전달.
- [ ] **옵션 B: GitHub CLI(`gh`) 설치 후 `gh auth login`**
  - https://cli.github.com 에서 설치 (winget: `winget install --id GitHub.cli`).
  - 설치 후 `gh auth login` 실행, 브라우저 인증 방식 선택.
  - 이 방식은 대화형 로그인이 필요해 무인 스케줄 환경에서는 옵션 A(PAT)가 더 적합합니다.

## 6. 완료 후 통보
- [ ] 위 1~5 완료 후 기술팀장에게 "저장소 URL + Pages URL"만 공유 (토큰 값은 공유하지 않음).
- [ ] 기술팀장이 저장소 URL 기준으로 자동 push 파이프라인 연결을 진행하고, 스케줄 자동화 활성화는 별도로 마스터/종민님 승인을 받습니다.

## 참고: 왜 이 단계들은 기술팀장이 대신 못 하나
- GitHub 계정 생성, 저장소 생성, Pages 활성화, 토큰 발급은 모두 종민님 개인/회사 계정 권한 범위의 작업입니다.
- 회사 매뉴얼(업무 규칙 6) 상 "파괴적이거나 되돌리기 어려운 작업(계정/채널 생성 등)"은 임의로 대행하지 않습니다.
