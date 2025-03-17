



### ECS


#### Service connect

https://docs.aws.amazon.com/ko_kr/AmazonECS/latest/developerguide/interconnecting-services.html


```
애플리케이션이 Amazon ECS 서비스에서 실행되는 다른 애플리케이션에 연결해야 하는 경우 Amazon ECS에서는 다음과 같은 방법으로 로드 밸런서 없이 할 수 있습니다.
```





### VPC

- 환경별 분리
- instance private subnet 사용
- public subnet 은 IGW, nat gateway, public load balancer 에만 사용


### 리서치 필요한 부분

#### ECS - 서비스간 통신
- Service connect 를 사용한 ECS 서비스간 private 통신
- Service connect 사용 시 데이터 전송 암호
- Service 간 통신에 TSL 적용 필요성, 비용
	- 단기 사설 인증서 발급 시 사설 CA 당 월 50 USD
	- 인증서 발급 개 당 0.75 USD. 5일 마다 자동 갱신 되므로 4.5 USD (0.75 x 6)
	- https://docs.aws.amazon.com/ko_kr/AmazonECS/latest/developerguide/service-connect-tls.html
- 다른 VPC ECS cluster 에서의 Service 간 통신
- 다른 VPC EC2 에서의 Service 간 통신


#### EC2 운영
- ASG 를 통한 무중단 배포 (rolling update)
- ASG 를 통한 이중화, 가용성 확보

#### IaC

- Cloudformation, terraform 등 적용 고려
	- 인프라 관리 용이성


#### EKS
