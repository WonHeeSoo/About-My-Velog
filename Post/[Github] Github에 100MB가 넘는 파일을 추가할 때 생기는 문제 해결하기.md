[Github] Github에 100MB가 넘는 파일을 추가할 때 생기는 문제 해결하기

# 💣 문제

Github 프로젝트에 SDK를 적용하고 커밋을 하려는 과정에서 100MB가 넘는 파일이 존재해 오류가 났습니다.

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Git/Git100MB.PNG?raw=true)

# 💡 해결

위의 이미지에선 오류가 나면서 해결책을 알려줍니다.
그 해결책인 git-lfs를 사용합니다.

1. [git-lfs](https://github.com/git-lfs/git-lfs)를 설치합니다.

```bash
$ git lfs install
```

---

2. 100MB가 넘는 파일을 등록합니다.

```bash
$ git lfs track "*.so"
```

---


3. git lfs를 설치하면서 같이 생성된 `.gitattributes`도 등록합니다.

```bash
$ git add .gitattributes
```

---

4. 100MB가 넘는 파일도 `add`, `commit`하고 push합니다.
> 💡 `git lfs track "*.so"`은 LFS에 해당되는 파일이라는 것을 알리는 것이고 그 파일을 `add`해야 합니다. 

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Git/Git100MB.PNG?raw=true)

LFS에 등록하기 전에 이미 100MB가 넘는 파일을 `commit`을 했기 때문에 같은 오류가 나타납니다.

---

5. 100MB가 넘는 파일을 `commit` 한 것까지 취소하고 다시 `add`, `commit` 후에 `push`를 하니 정상적으로 github에 `push`된 것을 알 수 있습니다.

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Git/Git100MB-LFS.PNG?raw=true)

---

[Git Large File Storage](https://git-lfs.github.com/)
[Git-LFS Github](https://github.com/git-lfs/git-lfs)
