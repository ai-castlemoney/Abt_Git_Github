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

7. git push origin master : github에 push
```
git push
```