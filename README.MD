### Git, GitHub을 활용한 팀원간 협업방법
- 팀원 중 한명의 GitHub을 활용하는 것을 가정

1. git clone : github repository를 local로 download
```
git clone "clone 하고자 하는 github repository 주소"
```
- ex) 
    - git clone `https://github.com/ai-castlemoney/github_test.git`

![clone image](https://github.com/ai-castlemoney/github_test/blob/master/images/clone_github_test.png)

2. git remote -v : github과 연결상태 확인 
```
git remote -v
origin	https://github.com/ai-castlemoney/github_test.git (fetch)
origin	https://github.com/ai-castlemoney/github_test.git (push)
```

3. echo add test file > ex.txt : ex.txt file 생성
```
echo add test file > ex.txt
```

4. git add ex.txt : ex.txt staging
```
git add ex.txt
```

5. git commit -m "add ex.txt" : add commit message
```
git commit -m "add ex.txt"
```

6. git status : git 현 상태 확인
```
git status

현재 브랜치 master
브랜치가 'origin/master'에 맞게 업데이트된 상태입니다.

커밋할 변경 사항:
  (use "git restore --staged <file>..." to unstage)
	새 파일:       ex.txt
```

7. git push -u origin master : github에 push(첫 push에만 -u option 사용)
```
git push -u origin master

오브젝트 나열하는 중: 9, 완료.
오브젝트 개수 세는 중: 100% (9/9), 완료.
Delta compression using up to 10 threads
오브젝트 압축하는 중: 100% (4/4), 완료.
오브젝트 쓰는 중: 100% (5/5), 327.62 KiB | 29.78 MiB/s, 완료.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ai-castlemoney/github_test.git
   28b22c4..2d1c20c  master -> master
```
- 이후 push는 git push 만 하면 됨.

- 팀원 중 한명이 수정사항 push를 하면 팀원에게 pull 하고 push를 하도록 공지한다.
- 다른 팀원은 git pull 하여 github과 local repository를 동일한 상태로 만든 후
- 본인의 변경사항을 push한다.

