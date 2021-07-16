# Git Bake up

> 원격 파일 저장 서비스 (.git(버전 정보를 포함)을 포함하여 모든 프로젝트 파일을 올림)
>
> - 파일 안전하게 사용/보관 가능
> - 자유롭게 어디서든 이용가능



## 1. 수업의 목표와 용어정리

- `Local Repository` : 지역 저장소 

- `Remote Repository` : 원격저장소

- `push` : 백업 (Local Repository -> Remote Repository )
- `clone` : 복제 (Local Repository <- Remote Repository )
- `pull` : 다운로드의 의미 
  - cf ) `clone`과 `pull`의 차이 
    - pull : 이미 로컬 저장소가 존재하는 상태에서 원격 저장소의 업데이트된 것을 내려받는 것
    - clone : 새로운 로컬 저장소를 만들어서 원격 저장소에서 내려받는 것



## 2. Git hosting 

> 원격 저장소를 임대하는 것

- 저장소 생성 (Github 기준)
  1. 우측 상단 + > New Repository
  2. Repository name 설정
  3. Create Repository
  4. 저장소 생성됨



## 3. 공부의 방향

1. Local -> Remote (push)
2. Remotr -> Local (clone/pull)
3. 통신 방법

- HTTP : 사용 용이 / 불편, 보안 취약
- SSH : 사용 어려움 / 편리, 보안 굿



## 4. 원격 저장소와 연결

> HTTP 방식을 이용하여 원격 저장소와 연결하는 방법

1. 저장소 생성 후 하단 내용 확인

##### …or push an existing repository from the command line

```
git remote add origin https://github.com/phjoo/Git-baek-up.git
git branch -M main
git push -u origin main
```

2. 명령어
   1. Local -> Remote 연결

      - `git remote add[원격 저장소 별명][원격 저장소 주소(HTTP)]` : 원격 저장소 주소와 연결시키는 명령어 

        ``` 
        git remote add origin https://github.com/phjoo/Git-baek-up.git
        ```

      - `git remot` : 원격 저장소 연결 확인

      - `git remot -v` : 원격 저장소 주소 확인 

   2. push

      - `git push` : 원격 저장소로 연결
      - `git push --set-upstream origin master` : 어떤 원격 저장소와 연결할지 정함
        - Username/Password : 인증을 위해 github 사용자의 아이디/비밀번호 입력

      

   

