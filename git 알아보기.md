# git 용어 알기
## head 란?
- 현재 작업중인 브랜치의 가장 마지막 commit

참고: [git에서 head란](https://dkswnkk.tistory.com/576#:~:text=%EB%AA%A8%EB%93%A0%20%EB%B8%8C%EB%A0%8C%EC%B9%98%EC%97%90%EB%8A%94%20HEAD%EA%B0%92,%EC%B5%9C%EC%8B%A0%20%EC%BB%A4%EB%B0%8B%EC%9D%84%20%EC%9D%98%EB%AF%B8%ED%95%A9%EB%8B%88%EB%8B%A4)

## base란?
- a브랜치에서 b브랜치 생성 시 a브랜치의 최신 버전(=b브랜치가 생성된 곳)

참고: [git에서 base, rebase란](https://fgh0296.tistory.com/31#:~:text=base%EB%9E%80%20%EC%98%88%EB%A5%BC%20%EB%93%A4%EC%96%B4,base%EB%8A%94%20a3%EB%9D%BC%EB%8A%94%20%EA%B2%83%EC%9D%B4%EB%8B%A4.)

# git으로 이거저거 테스트 해보기
## 기본 상태
- MASTER에서 BCHDEV-001_WORK를 생성한 후 MASTER에 commit을 하고 BCHDEV-001_WORK에도 commit을 한 상태
![image](https://github.com/HappyRiverSea/gitPractice/assets/118653760/53b17b83-7493-4a11-ae91-7fb29a213fc3)

## MASTER에 BCHDEV-001_WORK를 Merge 하면?
![image](https://github.com/HappyRiverSea/gitPractice/assets/118653760/c288d444-d3d1-4af3-81ae-95118936930f)

## MASTER를 BCHDEV-001_WORK 기준으로 rebase
![image](https://github.com/HappyRiverSea/gitPractice/assets/118653760/ffd5f877-d66e-48a9-ada5-68f31f45196f)

## BCHDEV-001_WORK를 MASTER 기준으로 rebase
![image](https://github.com/HappyRiverSea/gitPractice/assets/118653760/10b06f0c-f8ca-4f3d-ad76-0167afece28d)

# 우리는 어떤 git branch 전략을 사용해야 할까?
## Merge를 한다면 알아보기 어려울까?
BCHDEV-001_WORK 브랜치 딴 후 -> MASTER에 새로운 커밋 -> BCHDEV-001_WORK를 MASTER에 머지 -> BCHDEV-002_WORK 브랜치 땀
![KakaoTalk_20230606_191315889](https://github.com/HappyRiverSea/gitPractice/assets/118653760/1d6c349e-a14b-49e4-8cdb-9b8c70a09173)



참고: [git의 다양한 머지 전략 비교](https://inmoonlight.github.io/2021/07/11/Git-merge-strategy/)

