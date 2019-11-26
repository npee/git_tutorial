# Git 연습

## 저장소 생성

    -git init
        -git config
        user.name 이름
        user.email 이메일

## 변경사항 Staging

- git add 파일명
- git add \* : 변경사항 전체
- git add . : 현재 디렉토리 아래 모든 변경 사항

## 변경사항을 저장소로

- git commit -m "현재 변경사항의 설명"

## 변경 로그의 확인

- git log

## Staging 추적 제외를 위한 설정 파일

- .gitignore에 제외할 파일명의 패턴을 명시

## 원격 저장소의 추가

- git remote add origin https://github.com/npee/git_tutorial.git

## 원격 저장소에 변경 이력 반영

- git push origin 로컬브랜치이름
- git push origin master # 원격 저장소(origin)에 로컬 브랜치 master를 업로드
