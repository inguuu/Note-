# Note 

 #### 📝👦💡 기본적인 상식부터 최신 기술까지 메모!

---------------------------


## 📖  Microservice Architecture

- 시스템을 여러개의 독립된 서비스로 나눠서, 이 서비스를 조합함으로서 기능을 제공하는 아키텍쳐
- SOA의 경량화 버전(실패한다면 실패하는 이유도 같음)

#### 📌 여기서 서비스란

1) 단일화된 기능의 묶음 
2) Rest API 등을 통하여 기능 제공
3) 데이터를 공유하지 않고 독립적으로 가공 저장
4) 쿠버네티스의 서비스 개념과 매핑 가능


## 📖  What is Container?

- VM보다 가벼운 형식으로 어플리케이션을 pack, ship, run
- 컨테이너는 프로세스 격리를 기반으로 하는 애플리케이션 전달 메커니즘
- 리눅스 커널 기술 사용: cgroups, namspace + overlay fs + tooling
- 컨테이너 이미지를 사용하면 응용 프로그램 코드, 런타임 및 모든 Dependency들을 Pre-Defined Format으로 제한 가능
- 컨테이너는 새로운게 아니다. 기존 리눅스 LXC, Solaris Zones, BSD Jails 처럼 있던 개념

#### 📌 Docker
- Dokcer는 기존의 있는 것을 사용하여 빌드하고 관리할 오프소스 소프트웨어 


## 📖  What are Containers?

![그1](https://user-images.githubusercontent.com/49789734/77514183-b1d8c500-6eb9-11ea-8652-4f7e2712f8d6.png)

#### 📌 컨테이너에 의한 서버 환경 - 개발자들에게 인기 있는 이유 

##### 1. 어플리케이션은 어디에서든, 동일하게 동작함 
- 개발, 테스트, 프로덕션 어떤 환경에서든
- 베어메탈, 가상머신, 클라우드 어떤 환경에서든
- 랩탑에서도, 클라우드에서도 동일하게 구동

##### 2. 패키지화된 어플리케이션은 개발 싸이클의 속도를 빠르게 회전시킴
- 애자일한 생성과 배포가 가능
- 지속적인 통합/배포가 가능
- 단일 파일의 복사만으로 이를 가능하게 해줌 

##### 3. 마이크로서비스를 가능하게 해주기 위한 방법을 제공
- incrospectable(분석가능성) 
- isolated(격리성), elastic(탄력성) 


## 📖  Layers within a Docker Image?

- 도커파일은 텍스트 기반 문서로, 도커 이미지를 자동으로 빌드하기 위한 명령들을 기술 
- 컨테이너는 Multiple Layer로 구성되어 있음 - Top layer는 read/write, 나머지는 read-only
- 실제 사용자에게 보여지는 곳은 read/write layer 



## 📖  The benefits of using containers 

#### 4 Any
- Any Os (Linux, Windows)
- Anywhere (On-premises, Cloud)
- Any app(Monolith, Microservice)
- Any langauage(Java,.Net, Python, Node)



## 📖 Date Reference 

#### 자주 헷갈리는 부분 
- month의 범위는 0 ~ 11 중요
- get, set month를 주입하는게 다르다.
- get은 정상적으로 오지만 11월을 set하고 싶다면 10을 넣으면 된다. 

#### 📌 Example

```````
var weekday = new Array(7);

weekday[0] = "Sun";
weekday[1] = "Mon";
weekday[2] = "Tue";
weekday[3] = "Wed";
weekday[4] = "Thu";
weekday[5] = "Fri";
weekday[6] = "Sat";
 
var setDate = new Date();
setDate.setFullYear(closey,closem-1,i)
var PubDt="";
 		
var day;
day = setDate.getDay();
 			
if(i<10){
 	 	 PubDt= closey+closem+"0"+i;
else{
 				PubDt= closey+closem+i;
}
if(weekday[day]=="Sun"||weekday[day]=="Sat"){
 			    continue;
}
```````

## 📖 Grid Reference

- 이벤트, 메소드 중심 
https://eblo.tistory.com/32

- CSS 구조 중심 
https://heropy.blog/2019/08/17/css-grid/

