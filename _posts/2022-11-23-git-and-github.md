---
comments: true
layout: post
title:  "Git & Github"
date:   2022-11-23

---
## Git과 Github

Git은 오픈소스 분산 버전 관리 시스템입니다. 여러 개발자들이 하나의 프로젝트를 진행하기 위해서는 분산된 버전들이 생기게 되는데 이를 관리하기 위한 시스템입니다. 그렇다면 그 원격 저장소가 필요하게 되는데 그것이 Github입니다. 로컬 저장소에서 작업한 파일과 코드들을 다른 개발자들과 협업을 하기 위해서는 하나의 공통의 원격 저장소가 필요합니다. Github은 바로 이를 가능하게 해줍니다. 여러명의 개발자가 하나의 파일을 작업해도 문제가 생기지 않게 도와주고 언제나 원격저장소에서 코드를 가져오고 버전을 관리할 수 있게 도와줍니다.

## Local과 Remote

로컬에서 작업한 파일들을 원격 저장소로 올리기 위해서는 몇 가지 단계들을 거칩니다.

<img src="/assets/img/githubstage.png" alt=""> 

사진을 보면 로컬에서 3단계의 stage를 거쳐 원격 저장소로 업로드되는데, 

1. git add를 이용해 staging area로 변경사항들을 옮긴다.
2. commit 메세지와 함께 staging area에 있는 파일들의 변경사항들을 레포지토리에 commit한다.
3. 커밋들이 모두 끝나면 그 사항들을 원격 저장소에 업로드하기 위해 git push를 한다.
4. conflic가 나면 merge를 통해 해결한다.
5. 원격저장소에 있는 변경사항들은 git pull을 이용해 가져올 수 있다.

## Branch

git을 사용할때 코드의 흐름을 만들 수 있다.

<img src="/assets/img/gitbranch.png" alt="">

하나의 버전에서 또 다른 버전으로 넘어갈 때 다양한 흐름의 버전들을 만들면서 개발을 진행 할 수 있다.

git branch <branch_name>으로 쉽게 브랜치를 만들 수 있고, git checkout <branch_name>으로 브랜치를 쉽게 전환할 수 있다.

다양한 흐름으로 만든 후 이제 작업한 브랜치들을 합쳐줘야한다. 이 때 git merge <branch_name>을 사용한다. 또한 만든 브랜치를 삭제도 가능한데, git branch -d <branch_name>를 사용한다.