# git-test
## git 명령어
**echo "# git-test"** **>> [README.md](http://readme.md/)** :  README.md생성

git설치 → https://git-scm.com/download/win

**git init** : 해당 폴더를 git 프로젝트로 지정(init을 취소하는 방법은 init으로 생성된 .git 폴더를 제거하면 된다.)

**git remote add <remote> <git address>** : 원격 저장소와 github저장소를 연결(init한 폴더에서 실행)

**git remote --verbose** : 연결된 원격 저장소 확인

**git remote rename <old-remote-name> <new-remote-name>** : 원격 저장소 이름 변경

**git remote remove <remote-name>** : 원격 연결 삭제

**git add <filename>** : starting area에 파일을 올린다.(한번에 파일을 올리기: **git add .** / **git add —all**)

**git add /new/*** / **git add *.py** :  특정 디렉토리에 있는 문서나 py파일만 올리고 싶을 때

**git add --patch <filename> :** 한 파일 내에서 수정 사항만 준비 영역에 넣고 싶을 때(경로 형식은 안되는 것 같다. )
**git status** : 현재 상태 확인

**git commit -m “메모”** : staging area에 올라간 파일을 commit(메모는 커밋을 하면서 메모할 메세지)

**git commit —amend** : 커밋 메세지 수정

(i를 눌러 수정한 후, ESC (에디터 모드에서 명령 모드로 변경)  -> :wq (저장 및 종료 모드 입력) -> Enter순으로 클릭 )

**git branch -M main** : 메인 브랜치 만들기

**git push <remote_name> <branch_name> :** 커밋한 파일을 push해서 원격 저장소(github)로 보내기

**git pull <remote_name> <branch_name>** : 원격 저장소에서 변경된 정보를 확인하고, 최신 데이터를 복사하여 로컬 Git에 가져옴

**git fetch** : 원격 저장소에 변경사항이 있는지 확인만 하고, 변경된 데이터를 로컬 Git에 실제로 가져오지는 않음

따라서 fetch 수행 후 Pull 실행 시 더욱 안전

**git branch** : 현재 생성되어있는 브랜치 확인

**git branch <new branch name>** :  새로운 브랜치 생성

**git branch -D <branch name>** :  브랜치 삭제

**git branch -m <old branch name> <new branch name>** :  브랜치 이름 변경

**git checkout <branch name>** :  작업중인 브랜치 변경

**git merge <branch name> :** 현재 브랜치에 branch name의 내용을 합친다.