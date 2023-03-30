<h1 깃허브와 협업>

- Branch
> 분기들을 관리해준다. 
>> 실체는 포인터! 
>> Head : 내가 보고 있는 공간
>> testing : 가장 마지막 커밋을 가리키는 포인터
>> 확인할 때는 git checkout <새로운 브랜치> // 
git branch testing : testing이라ㅡㄴㄴ 이름의 브랜치를 만든다.
git checkout testing : testing이라는 브랜치로 head포인트 옮김
git branch : 현재 있는 브랜치드르을 전부 볼 수 있다. 


git은 공통조상을 기준으로 빠르게 합칠 수 있다. 
3 ways merge : 3개를 비교하는 상황 만약 충돌이 있다면, 이걸 conflict라 부르고, 
merge상황에서 conflict해결법 
두 브랜치를 merge할때 충돌이 발생한다면 개발자가 선택해주고 커밋해줘야한다
merge 는 add만 된다. 

git stash :: 지금까지 작업 못해둔거있으면 스택에 쌓아둠. 

깃플로우 : 브랜치를 관리하는 전략 / develop : 은 팀원들이 다 검사받은 코드만 합치는 것. // release branch : 버전 관리할 때 쓰는 것 
github commit meseage convention 
commit message와 branch 이름에는 규칙이 있다. 