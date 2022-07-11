## Github에 새로운 Repository 생성 후 로컬과 연결하는 방법

1. Github에서 new repository 생성

![new repository create](https://github.com/ai-castlemoney/Abt_Git_Github/blob/master/2.local_remote_connection/images/new_repository.png)

- 새로운 repository 생성과 함께 아래 그림과 같이 quick setup 방법에 대해 알려준다. 여기서는 quick setup의 첫번째 방법으로 실습해 본다.

![new repository create1](https://github.com/ai-castlemoney/Abt_Git_Github/blob/master/2.local_remote_connection/images/new_repository_1.png)
![new repository create3](https://github.com/ai-castlemoney/Abt_Git_Github/blob/master/2.local_remote_connection/images/new_repository_3.png)

2. local command line에서 위에서 생성한 repository와 같은 디렉토리(폴더) 생성(디렉토리(폴더)가 remote repository 이름과 달라도 상관없다.)
- local repository로 만들고자 하는 폴더로 이동 후 아래와 같이 폴더 생성

```bash
mac, linux : mkdir Abt_Git_Github
windows    : md Abt_Git_Github
```

3. 생성한 디렉토리(폴더)로 이동
```bash
mac, linux : cd Abt_Git_Github
windows    : cd Abt_Git_Github
```

4. 현재 디렉토리(폴더) 확인
```bash
mac, linux : pwd
windows    : cd
```

5. 아래 순서와 같이 실행
```bash
echo "# Abt_Git_Github" > README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ai-castlemoney2/Abt_Git_Github.git
git push -u origin main
```

6. 사용자 이름과 이메일 설정하는 방법
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

7. git 상태 확인하기
```bash
git status
```
```bash
On branch master
No commits yet
nothing to commit(create/copy files and use "git add" to track)
```