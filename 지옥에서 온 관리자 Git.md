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

___

> git branch  
> git branch topic  
> git checkout master  
> git merge topic


<br>  


### rebase  

___  

> git rebase -i HEAD~3  

- vi editor로 commit log를 어떻게 수정할지를 결정한다.  
- 제일 과거의 commit log를 pick하고 그 이후의 log들은 squash한다.  
- pick한 commit log를 알맞게 수정해준다.  

<br>

## 섹션4. Github 사용법  

<br>

___

### Github push  

```bash
# 원격 저장소와 연결 : git remote add origin [git 주소]
$ git add remote origin https://github.com/wonsakku/git-study.git  

# remote 확인  
$ git remote -v
origin  https://github.com/wonsakku/git-study.git (fetch)
origin  https://github.com/wonsakku/git-study.git (push)

# remote 확인  
$ git ls-remote
From https://github.com/wonsakku/git-study.git

# push  
$ git push origin master
Enumerating objects: 48, done.
Counting objects: 100% (48/48), done.
Delta compression using up to 8 threads
Compressing objects: 100% (43/43), done.
Writing objects: 100% (48/48), 4.68 KiB | 799.00 KiB/s, done.
Total 48 (delta 22), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (22/22), done.
To https://github.com/wonsakku/git-study.git
 * [new branch]      master -> master

```