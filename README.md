# Git 연습

## 저장소 생성

    - git init
        - git config
            - user.name 이름
            - user.email 이메일

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

## 가지 치기

- git checkout 브랜치명 : 브랜치명 가지로 이동
- git checkout -b 브랜치명 : 브랜치명 가지를 만든 후 이동

- git checkout을 할 때 현재 가지에 변경 주인 파일이 남아 있으면 안된다

## 가지 병합

- 다른 가지의 변경 사항을 현재 가지로 반영할 경우
- git merge 브랜치명

## 태그 달기

- git log에서 commit의 ID를 확인
- git tag 태그명 commit ID

- 태그 업로드
- git push 원격저장소 로컬브랜치명 --tags
- 예) git push origin master --tags # 태그와 함께 브랜치를 push!

## 저장소 복제

- git clone 원저장소url
- git clone 원저장소path

<<<<<<< HEAD
## 클라이언트 변경 사항 발생
=======
## 서버 변경 사항 발생
>>>>>>> 18496c2195e931749510b083eebfa2e46afa1fe1
