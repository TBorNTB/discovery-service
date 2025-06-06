# discovery-service

서비스 디스커버리 (Service Discovery)를 위한 [Spring Cloud Eureka Server](https://cloud.spring.io/spring-cloud-netflix/multi/multi_spring-cloud-eureka-server.html) 레포지토리입니다.

##  개요

`discovery-service`는 마이크로서비스 아키텍처(MSA) 환경에서 개별 서비스들의 위치를 중앙에서 관리하고, 동적으로 서비스 인스턴스를 탐색할 수 있도록 도와주는 **Eureka 서버**입니다.

이 서버는 각 마이크로서비스(`user-service`, `order-service`, `catalog-service`, `api-gateway` 등)가 등록되어 서로의 위치(IP, 포트 등)를 자동으로 인식할 수 있도록 해줍니다.

---

## ⚙️ 기술 스택

- Java 17+
- Spring Boot
- Spring Cloud Netflix Eureka Server

---

##  실행 방법

1. 레포지토리 클론
    ```bash
    git clone https://github.com/your-org/discovery-service.git
    cd discovery-service
    ```

2. 실행
    ```bash
    추후 작성
    ```

3. Eureka 대시보드 접속  
    브라우저에서 [http://localhost:8761](http://localhost:8761) 접속

---

##  관련 서비스

추후 작성

---

##  참고

- 서비스에 등록하려면 클라이언트 서비스에서 다음 설정이 필요합니다:
    ```yaml
    eureka:
      client:
        register-with-eureka: true
        fetch-registry: true
        service-url:
          defaultZone: http://localhost:8761/eureka
    ```

---

##  작성자 / 관리

- Owner: [@PlusUltraCode](https://github.com/PlusUltraCode)
- Owner: [@sigmaith](https://github.com/sigmaith)
