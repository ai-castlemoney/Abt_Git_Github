## Github에 새로운 Repository 생성 후 로컬과 연결하는 방법

1. Github에서 new repository 생성
![new repository create](https://github.com/ai-castlemoney/github_test/blob/master/images/clone_github_test.png)
![new repository create1]()
![new repository create1]()
![new repository create1]()

2. local command line에서 위에서 생성한 repository와 같은 디렉토리(폴더) 생성
```
mac, linux : mkdir team_project
windows    : md team_project
```

3. 생성한 디렉토리(폴더)로 이동
```
mac, linux : cd team_project
windows    : cd team_project
```

4. 현재 디렉토리(폴더) 확인
```
mac, linux : pwd
windows    : cd
```

5. 아래와 순서와 같이 실행
```
echo "# team_project" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ai-castlemoney2/team_project.git
git push -u origin main
```