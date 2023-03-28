## 섹션2. Git 중급  

<br>

### git reset 

___

|옵션|용도?|
|:--:|--|
|soft|커밋 로그를 제거하고 변경된 파일을 staged 상태로 변경|
|mixed|커밋 로그를 제거하고 변경된 파일을 unstaged 상태로 변경|
|hard|커밋 로그를 제거하고 변경된 파일을 삭제|

> git reset --hard [커밋 hash값]

<br><br>

### git reflog  

___

> git log history 전체 출력. reset --hard한 내용도 출력이 되기 때문에 reset --hard를 사용하면 reset --hard 이전으로 돌아갈 수 있다.  

<br><br>

### amend  

___

> git commit --amend -m "~~~~~"

<br><br>

## 섹션3. Git 고급  

<br>  

### branch  

> git branch  
> git branch topic  
> git checkout master  
> git merge topic
