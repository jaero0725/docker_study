# docker_study


## 도커란?(Docker)

어플리케이션을 패키징 할수 있는 툴

Container라는  application, system tools, dependencies 을 하나로 묶어서 서버, pc 에 배포해서 안정적으로 구동할 수 있도록 해줌

버전이 맞지 않는 경우에 에러가 나옴 
-> 이런 번거러움을 해결해주기 위함.

모든 것을 도커 컨테이너에 담아놨다.

런타임 환경에 필요한 모든 것을 담아놈. 

## Container VS VM 의 차이 

VM 에서 경량화된 컨셉이 Container 
개별적인 Container Engine을 사용 = 가장 많이 사용되는 것이 docker enginer 


## 도커의 3대 구성요소 

docker 101 동작 순서
컨테이너 만들고 -> 배포 -> 구동

3가지 building containers

dockerfile , image, container 
1) dockerfile : 설명서, copy files , install dependencies , set enviroment variables, run setup scipts
2) Image : application (스냅샷 
3) Container : 고립된 파일 시스템 에서 실행될 수 있는 것을 말함 이미지를 이용하여 어플리케이션을 동작

Image 불변의 상태 - 컨테이너에서 동작하는 상태는 개별적으로 수정가능한 상태, 
이미지는 클래스, 컨테이너는 인스턴스라고 보면 된다. 

## 도커이미지를 배포하는 과정(Shipping Containers)

Local Machine 
image         -> push  -> Container Registry                  
                          image             -> pull   ->   Server       <= Docker 

public          private
dockerhub       AWS
RED HAT         Google Cloud
Github Package  Azure
                       
