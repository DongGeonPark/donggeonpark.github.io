---
title: "Git 기초 명령어 정리"
date: 2025-07-06
categories: [개발]
tags: [git, version-control, 개발도구]
---

## Git 기초 명령어 정리 📝

Git은 버전 관리를 위한 필수 도구입니다. 자주 사용하는 명령어들을 정리해보겠습니다.

### 기본 설정
```bash
# 사용자 정보 설정
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# 기본 브랜치 설정
git config --global init.defaultBranch main
```

### 저장소 초기화 및 클론
```bash
# 새 저장소 초기화
git init

# 원격 저장소 클론
git clone <repository-url>
```

### 기본 작업 흐름
```bash
# 파일 상태 확인
git status

# 파일 추가
git add <filename>
git add .  # 모든 파일 추가

# 커밋
git commit -m "커밋 메시지"

# 원격 저장소에 푸시
git push origin main
```

### 브랜치 관리
```bash
# 브랜치 목록 확인
git branch

# 새 브랜치 생성
git branch <branch-name>

# 브랜치 전환
git checkout <branch-name>
git switch <branch-name>  # Git 2.23+

# 브랜치 생성 및 전환
git checkout -b <branch-name>
```

### 변경사항 확인
```bash
# 변경사항 확인
git diff

# 커밋 히스토리 확인
git log
git log --oneline  # 간단한 형태
```

### 되돌리기
```bash
# 마지막 커밋 수정
git commit --amend

# 파일 되돌리기
git checkout -- <filename>

# 브랜치 되돌리기
git reset --hard HEAD~1
```

### 원격 저장소
```bash
# 원격 저장소 추가
git remote add origin <repository-url>

# 원격 저장소에서 가져오기
git pull origin main

# 원격 저장소 정보 확인
git remote -v
```

### 유용한 팁
- 커밋 메시지는 명확하고 간결하게 작성
- 자주 커밋하기
- 브랜치를 활용한 기능 개발
- .gitignore 파일 활용

Git을 잘 활용하면 팀 프로젝트에서 효율적으로 협업할 수 있습니다! 