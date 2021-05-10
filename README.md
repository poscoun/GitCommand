# git init(저장소 설정)
1. git init
  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"
2. git remote add origin 레파지토리 주소(예-https://github.com/poscoun/Goott_JAVA.git)
3. git remote -v 

# git 업로드
1. git status
2. git add . ( . : all )
3. git commit -m "memo"
4. git push origin master

# git clone(저장소 불러오기)
1. git clone 레파지토리 주소

# git pull(최신화)
1. git pull origin master  안될 시 git pull 만 입력

# git 삭제
1. git rm -rf {파일명 및 폴더명}  // 원격 스토리지 및 로컬 스토리지에 있는 파일을 삭제한다.
   git rm -r - cached {파일명 및 폴더명}  // 원격 스토리지만 삭제한다.
 
2. git commit -m "remove webstom {파일명 및 폴더명} directory"
 
3. git push origin master    안될시 git push 만 입력

# 강제 업로드
$ git push origin +master
