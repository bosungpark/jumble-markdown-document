VPC 와 Subnet
=

https://youtu.be/WY2xoIClOFA?si=r0yhiZt8fQd-dOFq

VPC
-
Virtual Private Clould의 약자로 AWS 계정 전용 가상 네트워크이다.
VPC는 AWS 클라우드에서 다른 가상 네트워크와 논리적으로 분리되어 있으며 AWS 리소스를 VPC에서 실행 가능하다.
IP 주소 범위와 VPC 범위를 설정하고 서브넷을 추가하고 보안그룹을 연결한 후 라우팅 테이블을 구성한다.

즉, 가상으로 존재하는 데이터 센터(단위)
외부에 격리된 네트워크 컨테이너 구성 가능
원하는 대로 사설망 구축 가능
리전단위

서브넷
-
VPC의 하위 단위, VPC에 할당된 IP를 더 작은 단위로 분할한 개념
하나의 서브넷은 하나의 가용영역 안에 위치
CLDR block range로 IP주소 지정

1. 퍼블릭 서브넷: 외부에서 인터넷을 통해 접근 가능, 인터넷 게이트웨이 사용, 웹 서버 등 유저에게 노출되어야 하는 서비스
2. 프라이빗 서비스: 퍼블릭 IP 부여 불가능, 데이터베이스 등 외부에 노출될 필요가 없는 인프라 

라우트 테이블
-
트래픽이 어디로 가야 할지 알려주는 이정표
VPC 생성시 기본으로 하나 제공

인터넷 게이트웨이
-
VPC가 외부의 인터넷과 통신할 수 있도록 경로를 만들어 주는 리소스
고가용성 확장성이 기본적으로 확보되어 있음
라우트 테이블에서 경로 설정 후 접근 가능
무료
