# High-Availability-Testing-Using-Docker

![image](https://github.com/Painterrr/High-Availability-Testing-Using-Docker/assets/98957340/7627dae4-bbe7-4b8c-804d-39b9169a0b1b)

도커 컴포즈로 wordpress, mysql-1, mysql-2 구성.
도커 스웜으로 wordpress를 매니저 노드로 지정.
mysql-1, mysql-2를 워커 노드로 구성.
wordpress와 mysql-1을 연결 후, 데이터 입력 하다가 mysql-1 다운.
<br>
1. mysql-2로 데이터가 저장될지
2. mysql-1이 새로 생성되어 데이터가 저장될지
<br>
테스트 결과
mysql-1이 다운된 후 곧바로 새로운 mysq1-1이 생성되어 매니저 노드와 연결.
데이터 저장 유지.
고가용성 확보.
