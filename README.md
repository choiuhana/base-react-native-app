@choiuhana package 설치 방법

$ npm login --scope=@NAMESPACE --auth-type=legacy --registry=https://npm.pkg.github.com

> Username: USERNAME
> Password: TOKEN


build

developmentDebug
-> 개발 기본 단위, metro 프론트 서버 연결 및 Dev API 서버를 바라봄

developmentRelease
->  Dev API를 바라보는 release 빌드시 문제가 없는지 살피고 codePush 개발(development)버전을 테스트해볼 수 있음

productionDebug
-> metro 프론트 서버에 연결되어 Main API 서버를 바라봄, 실제 데이터를 통한 디버깅을 위함

productionRelease
-> Main API를 바라보는 최종 배포 버전의 Build, codePush 실사용(production)버전을 받아볼 수 있음


ios

//react-native run-ios --configuration {빌드 변형}

react-native run-ios --configuration developmentDebug


Android
//react-native run-android --variant {빌드 변형} --appIdSuffix {suffix}

react-native run-android --variant developmentDebug --appIdSuffix dev
