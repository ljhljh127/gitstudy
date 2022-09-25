# 깃 기본 스터디

## 1주차
Git이란?
분산형 버전관리 시스템

Git hub
깃 프로젝트를 호스팅 해주는 곳

Git commit 하는법
1.git init
깃 디렉토리를 만드는 명령어 숨겨진 폴더로 만들어짐

2.Github에 레포지토리 생성하기

3.생성된 주소 복사 후 다음과 같은 명령어 입력
git config user.name "(깃허브 name)"
git config user.email "(자신의 깃허브 가입 이메일)"
git remote add origin "(위에서 복사한 주소)"

4.git add 명령어로 추가
 여기서 .을 입력하면 모든 파일이라는 뜻임ex) git add .
Git status 로 변경내용 확인 가능
//추가내용 add명령어는 스테이징 영역에 추적하는 파일을 등록하는 의미임

5.git push 로 적용
Git push origin 브랜치명

6.Git commit 으로 커밋 생성 
Git commit -m 메시지
커밋은 작업 변경사항 일종의 주석의 느낌
//추가내용 스테이징 영역에서 식별한 파일들을 커밋 단위로 만든 후 등록



## 2주차

 
Git작업트리
프로젝트 내 작업을 처리하기 위하여 사용
깃이 추적,추적하지 않는 파일을 구분하고 추적하는 파일들의 상태를 구분 짓는 영역

1.작업디렉토리
실제로 작업중인 파일들이 존재하는 영역 파일을 생성하거나 기존 파일을 수정할 때 이곳

2.스테이징 영역
작업 디렉토리에서 작업중인 파일 중 깃이 추적하는 파일 식별하는 영역

3.지역 저장소
스테이징 영역에서 추적된 파일들이 커밋으로 등록되는 영역

Tracked와 Untracked
새로 생성된 파일은 기본적으로 Untracked 상태를 가짐
 
Add 하면
 
파일은 Tracked 상태로 들어가며 커밋 으로 기록될 준비가 되었다고 바뀜

만일 수정한다면
 

파일의 수정 여부에 따라 Modified와 Unmodified로 분류가 된다.

Modified와 Unmodified
Modified의 사전적 의미는 수정됨 이며 수정 여부에 따라 분류된다
 
위 그림과 같이 이루어지는데
일단 git add를 하는 순간 스테이징 영역으로 넘어가고 수정 여부에 따라 Modified
Unmodified로 나누어지며
Modified 영역에 있는 것은 Unstage 스테이지 상태가 아니다 즉 커밋 기록 불가이고
Unmodified 영역에 있다면 Stage 스테이지 위에 올라와 있다 즉 커밋 기록 할 준비가 됬다 라고 할 수 있다.

다른 사람 코드 가져오기
git clone 명령어
만약 변경사항을 로컬에 가져오려면 git pull origin 브랜치명으로 가져오면 됨


