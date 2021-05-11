# git 개인

## git init(저장소 설정)
1. git init
  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"
2. git remote add origin 레파지토리 주소(예-https://github.com/poscoun/Goott_JAVA.git)
3. git remote -v 

## git 업로드
1. git status
2. git add . ( . : all )
3. git commit -m "memo"
4. git push origin master

## git clone(저장소 불러오기)
1. git clone 레파지토리 주소

## git pull(최신화)
1. git pull origin master  안될 시 git pull 만 입력

## git 삭제
1. git rm -rf {파일명 및 폴더명}  // 원격 스토리지 및 로컬 스토리지에 있는 파일을 삭제한다.
   git rm -r - cached {파일명 및 폴더명}  // 원격 스토리지만 삭제한다.
 
2. git commit -m "remove webstom {파일명 및 폴더명} directory"
 
3. git push origin master    안될시 git push 만 입력

## 강제 업로드(안하는게 좋음)
$ git push origin +master

====================================================================================
# git 협업
1. Fork 가져가기 
2. origin(fork된 나의 레파지토리) clone 내려받기 [중요]
3. origin(팀원), upstream(팀장) 주소 저장(remote add upstream 업스트림주소) 절대 upstream 건들지 않기
4. pull request(PR) - 팀장한테 요청, 팀장은 모두 수락 후
5. branch 생성
- 브랜치 목록 보기 : git branch --list
- 브랜치 생성만 : git branch <브랜치명>
- 브랜치 이동 : git switch <브랜치명>
- 브랜치 생성 동시에 이동 : git checkout -b <브랜치명>
- 브랜치 삭제 : git branch -D <브랜치명>
6. 팀원들은 fetch(git fetch upstream) 받고, rebase(git rebase upstream/master) 한다.
7. git push origin <브랜치명>
8. 모든 팀원들의 PR이 완료되면, 각 팀원들의 브랜치를 삭제하고 패치(main) 후 다시 브랜치 생성 후 반복 [권장]

## 주의사항 
- 같은 파일 다른인원이 동시 작업하면 안됨
