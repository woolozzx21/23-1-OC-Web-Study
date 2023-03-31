<h1 깃허브와 협업>

- Branch
 분기들을 관리해준다. 실체는 포인터! 
 Head : 내가 보고 있는 공간
testing : 가장 마지막 커밋을 가리키는 포인터
확인할 때는 git checkout <새로운 브랜치> // 
git branch testing : testing이라는 이름의 브랜치를 만든다.
git checkout testing : testing이라는 브랜치로 head포인트 옮김
git branch : 현재 있는 브랜치들을 전부 볼 수 있다. 
git brand -D [브랜치 이름] : 브랜치 삭제

>Merge
- 다른 브랜치로 합치는 것.
- 보통 main브랜치는 실 서비스에 배포된 서비스를 관리하고, 
    main브랜치가 아닌 브랜치에 새로운 기능을 개발하고, 완료되면 main브랜치에 merge 하는 식.
- 가장 기본적인 merge : Fast Forward Merge
    현재 브랜치의 HEAD가 대상 브랜치의 HEAD까지로 옮기는 merge
    git switch[현재 브랜치]
    git merge[대상 브랜치]

- git은 공통조상을 기준으로 빠르게 합칠 수 있다. 
3 ways merge : 3개를 비교하는 상황 만약 충돌이 있다면(동일 파일을 수정한 경우), 이걸 conflict라 부르고, 
>merge상황에서 conflict해결법 
-두 브랜치를 merge할때 충돌이 발생한다면 개발자가 선택해주고 커밋해줘야한다
- merge 는 add만 된다. 

git stash :: 지금까지 작업 못해둔거있으면 스택에 쌓아둠. 

깃플로우 : 브랜치를 관리하는 전략 / develop : 은 팀원들이 다 검사받은 코드만 합치는 것. // release branch : 버전 관리할 때 쓰는 것 
github commit meseage convention 
commit message와 branch 이름에는 규칙이 있다. 

fork : 원작자의 코드를 fork하면, 자신의 원격 저장소에서 코드를 마음대로 뜯어 고칠 수 있다. 
원작자에게 요청을 보내어 원작자가 수락하면, 원작코드가 뜯어 고친 코드로 바뀌고 나는 contributor가 된다.


- git clone [url] [dir] 
내 로컬 dir에 url의 리포지터리를 가져온다. 

> commit 메시지 컨벤션
commit 메시지는 제목/본문/꼬리말로 구성된다.

- type
Feat : 새로운 기능 추가
Fix : 버그 수정
Docs : 문서 수정
Style : 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우
Refactor : 코드 리팩토링
Test : 테스트 코드, 리팩토링 테스트 코드 추가
Chore : 잡무

- Subject 
제목은 50자 넘기지 않고, 대문자로 작성 마침표를 붙이지 않음
과거시제 사용하지 않고 명령어로 작성. 

- Body 
선택사항이기 때문에 모든 커밋에 작성할 필요 X
부연 설명.