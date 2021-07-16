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

- 저장소 생성
  1. 우측 상단 + > New Repository
  2. Repository name
  3. 