# learning-git-submodule
## 다른 디렉토리 이름으로 submodule 추가하기


```bash
git submodule add git@github.com:creaticoding/repo.git my-repo
```


- submodule없이 프로젝트가 push 되면 안된다. (submodule에 대한 내용은 가져오지도 쓰지도 못함)
  - 그래서 `--recurse-submodules` 옵션을 사용하면 `git push` 할 때 submodule 을 반영했는지 검사한다.



## 서브모듈 프로젝트를 Fetch & Update

```
git submodule update --remote
```

  - 서브모듈 디렉토리에서 Fetch 명령과 Merge 명령을 실행하지 않아도 git submodule update --remote 명령을 실행하면 Git이 알아서 서브모듈 프로젝트를 Fetch 하고 업데이트한다.
