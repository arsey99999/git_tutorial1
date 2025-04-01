# git_tutorial1

# Git & GitHub 튜토리얼 (한글)

> 이 문서는 Git과 GitHub의 기초부터 실전까지 따라 하며 익힐 수 있는 완전 입문용 가이드입니다.
> 저도 헷갈릴때 참고 할 수 있고 예시 코드를 통해 누구나 쉽게 실습할 수 있도록 작성했습니다.
---

## 목차

1. Git & GitHub란?
2. Git 설치 및 사용자 정보 설정
3. Git 기본 명령어 실습 (add, commit, push 등)
4. GitHub 저장소 생성 및 연결
5. 예제 프로젝트 실습 (clone부터 push까지)
6. 협업 기능 - Fork, Pull Request
7. GitHub Pages 배포

---

## 1. Git & GitHub란?

- **Git**: 소스코드 변경 이력을 관리할 수 있는 분산 버전 관리 시스템입니다.
- **GitHub**: Git 저장소를 클라우드에서 관리하고 협업할 수 있는 플랫폼입니다.

---

## 2. Git 설치 및 사용자 정보 설정

### Git 설치
- [Git 다운로드](https://git-scm.com/)에서 운영체제에 맞게 설치

### 사용자 정보 입력 (Windows CMD 기준)
```
git config --global user.name "홍길동"
git config --global user.email "hong@example.com"
```

---

## 3. Git 기본 명령어 실습

### 새 프로젝트 생성 (Windows CMD 기준)
```
mkdir my-first-project
cd my-first-project
echo "# My First Project" > README.md
```

### Git 초기화
```
git init  // 로컬 저장소 초기화
```

### 변경 파일 추적 및 커밋
```
git status                // 현재 상태 확인
git add .                 // 모든 변경 파일 스테이징
git commit -m "첫 커밋"  // 커밋 메시지 작성
```

---

## 4. GitHub 저장소 생성 및 연결

1. [https://github.com](https://github.com) 접속
2. 우측 상단 ➕ 클릭 → "New repository"
3. 저장소 이름 입력 (예: `my-first-project`)
4. `README.md` 초기화는 **체크하지 않음**

### 원격 저장소 연결 (Windows CMD 기준)
```
git remote add origin https://github.com/사용자명/my-first-project.git
git branch -M main
git push -u origin main
```

---

## 5. 예제 프로젝트 실습

### 저장소 클론 (Windows CMD 기준)
```
git clone https://github.com/사용자명/my-first-project.git
cd my-first-project
```

### 파일 수정 및 커밋
```
echo "## 프로젝트 소개" >> README.md
git add README.md
git commit -m "README에 프로젝트 소개 추가"
git push origin main
```

### 예제 코드 추가
```
echo "print('Hello GitHub!')" > hello.py
git add hello.py
git commit -m "hello.py 파일 추가"
git push origin main
```

---

## 6. 협업 기능 - Fork & Pull Request

### Fork
- 다른 사람의 저장소를 내 계정으로 복사
- GitHub에서 "Fork" 버튼 클릭

### Pull Request
- 변경 내용을 원본 저장소에 반영 요청
1. 내 저장소에서 변경 후 push
2. "Pull Request" 버튼 클릭 후 설명 작성

---

## 7. GitHub Pages 배포

1. 저장소 이름을 `사용자명.github.io`로 생성
2. HTML 파일 업로드
3. `Settings` → `Pages` → `Deploy from branch`
4. 브랜치 선택 후 저장
5. 주소: `https://사용자명.github.io`

---

## 마무리

이제 Git과 GitHub 사용법을 직접 실습하며 익힐 수 있습니다. 
궁금한 점은 댓글이나 이슈를 통해 남겨주세요.

👉 더 많은 튜토리얼과 AI 활용법은 [gptonline.ai/ko](https://gptonline.ai/ko/)에서 확인하세요!
