# Note 

기본적인 상식부터 최신 기술까지 메모!

📝👦💡

### 📖  Microservice Architecture

- 시스템을 여러개의 독립된 서비스로 나눠서, 이 서비스를 조합함으로서 기능을 제공하는 아키텍쳐
- SOA의 경량화 버전(실패한다면 실패하는 이유도 같음)

##### 📌 여기서 서비스란

1) 단일화된 기능의 묶음 
2) Rest API 등을 통하여 기능 제공
3) 데이터를 공유하지 않고 독립적으로 가공 저장
4) 쿠버네티스의 서비스 개념과 매핑 가능


### 📖  What is Container?

- VM보다 가벼운 형식으로 어플리케이션을 pack, ship, run
- 컨테이너는 프로세스 격리를 기반으로 하는 애플리케이션 전달 메커니즘
- 리눅스 커널 기술 사용: cgroups, namspace + overlay fs + tooling
- 컨테이너 이미지를 사용하면 응용 프로그램 코드, 런타임 및 모든 Dependency들을 Pre-Defined Format으로 제한 가능
- 컨테이너는 새로운게 아니다. 기존 리눅스 LXC, Solaris Zones, BSD Jails 처럼 있던 개념

##### 📌 Docker
- Dokcer는 기존의 있는 것을 사용하여 빌드하고 관리할 오프소스 소프트웨어 
