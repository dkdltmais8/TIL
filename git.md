#git init 대상이 되는 폴더를 git으로 관리하기 시작하겠다.
#git status 어떤 변경사항이 있는지 알아보기 위한 명령어
#Untracked files 아직 변경사항이 저장되지 않은 파일들
#stage 변경사항이 관리되기 시작하는 단계
#stage에 파일 올리기 => git add 파일명
#누가 기륵했는가 (git config --global user.namer ,user.email)
#commit 단계
# git commit -m '커밋 메세지'
#git log 기록확인

맨 처음 폴더 git 이 관리 할건지 안할건지
1.git init   저장소(repository)만드는 용도 .
 ( 폴더당 딱 한번) 끝에 master가 보인다면 init 할 필요없음
2.파일을 기록하고 싶다면 
git add 파일명
3. git commit -m '커밋 메세지 내용'(변경사항 요약해서 적음)
3.수정사항 발생 -> 다시 2번 반복
4. 상태 확인하기  git status
## --global은 모든 저장소에 똑같이 적용함을 의미 
5.내 정보 입력하기 git config --global user.name유저이름
                git config --global user.email 이메일
6.커밋 기록 확인하기
git log --oneline

##원격(remote) 저장소
-github  무료  개인 
-gitlab(SSAFY) 유료 회사 조직

폴더(repository)단위로 관리 됨
##내 컴퓨터의 저장소 -> github의 내가 만든 원격 저장소 등록
git remote add origin(=원격저장소이름) 주소url

#원격저장소에 파일보내기
git push origin master

