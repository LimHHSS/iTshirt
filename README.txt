Commit - '커밋'은 생성된 각 버전을 의미한다. 변경사항 별 버전

※ 파일 변경한 거 커밋하는법

 1. 스테이징 (버전으로 만들 파일을 선택하는 것)
-> 파일을 커밋하려면 먼저 git add <파일명> 명령어로 변경된 파일을 스테이징해야 함.
ex) git add README.txt

2. 커밋 메시지 만들기
-> git commit -m "메시지 입력"
-> -m은 message의 약자이다. 메시지는 큰 따옴표 " " 로 묶어서 입력해야 한다.

# git log 를 통해 지금까지 만든 커밋을 확인할 수 있다. 최신 커밋부터 보여준다.

3. 원격 저장소에 커밋 올리기
-> git remote add origin <Github 레포지토리 주소 입력>
-> github에서 새 레포지토리 만들고 그 주소를 입력하는 것이다. origin은 원격 저장소(깃허브 레포지토리)를 의미한다.

# git 터미널에서 레포지토리 주소가 ctrl+v로 붙여넣기 안되므로 우클릭 paste로 붙여넣기!

4. 커밋을 둘 장소의 이름을 짓는다. (branch)
-> 원격 저장소(origin) 안에 main 이라는 이름의 방을 만들것이다. 이 방은 branch라고 한다. (엄밀히 방은 아님)
-> git branch -M main

# -M은 branch의 이름을 master에서 main으로 바꾸겠다는 의미이다.

5. 로컬 저장소에 있는 커밋들을 원격 저장소 github에 push
-> git push origin main 

# origin(원격저장소)의 main이라는 방에 내 커밋들을 올려라(push)