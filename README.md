
# GitHub 사용법 실습 정리 (올리기 / 내리기 / 연결)

## 목적
GitHub와 로컬 PC를 연결하고  
코드를 **올리고(push)**, **내리고(pull/clone)** 하는 기본 흐름을 익힌다.  
실습 중 겪은 문제들과 해결 방법을 함께 정리한다.

---

## 실습 환경
- Windows
- PowerShell / Git Bash
- GitHub 개인 계정

---

## GitHub ↔ 내 컴퓨터 연결 (최초 1회)

### 방법 1️⃣ 권장: GitHub에서 내려받으며 시작
```bash
git clone <GitHub_저장소_URL>
git clone https://github.com/hoorak17/vacation-practice.git
git init
git add .
git commit -m "init"
git remote add origin <GitHub_저장소_URL>
git push -u origin main
git add .
git commit -m "커밋 메시지"
git push
git pull
git clone <GitHub_저장소_URL>
git push origin master:main --force
git branch -M main
git push -u origin main
vacation-practice/
  README.md
  git-basic/
    test.cpp
처음: git clone
올리기: git add → git commit → git push
내리기: git pull

---

### 이제 실제로 할 일 (3줄)
```bash
README.md 열기
→ 위 내용 전체 붙여넣기
→ git add README.md && git commit -m "GitHub 기본 사용법 정리" && git push
