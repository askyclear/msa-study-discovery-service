# msa-study-discovery-service

### Service Discovery 
MSA로 구성되어있는 서비스 인스턴스 각각의 ip와 포트 정보들을 등록하고 관리하는 역할을 하는 것.

### YML 설정 정보
eureka.server.enableSelfPreservation : 일시적인 네트워크 장애로 인한서비스 해제 막기위한 자기 보호 모드(default : true)
eureka.client.registerWithEureka :  유레카 서비스에 등록할지여부(default : true)

eureka.client.fetchRegistry : 유레카 서비스가 시작할때 레지스트리정보를 가져올지에대한 여부(default : true) 
true인 경우 검색시 Eureka Server를 호출하는 대신 레지스트리가 로컬로 캐싱되어 확인

eureka.server.responseCacheUpdateIntervalMs : 유레카 서버의 캐싱 업데이트 주기
eureka.client.registryFetchIntervalSeconds : 서비스 목록을 캐싱할 주기
