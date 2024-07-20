
<!--
# Hello World 



-->
# Hello World 

## ⚙️ 시스템 아키텍처
![image](https://github.com/user-attachments/assets/fb9b22ba-7dbc-4762-aa8d-0a374f5b7ac2)
* 다수의 리소스를 관리하기 위해 docker-compose를 사용합니다. 
* 모델 호출을 위해 FastAPI 프레임워크를 사용하고, 이를 SpringbBoot에 연동합니다. 
* FinGPT의 요청과 응답, 채팅 로그의 저장 등의 이벤트 기반 데이터 처리를 위해 Apache Kafka를 사용하는데, AWS에 맞춰서 배포부터 운영을 담당하는 Amazon MSK를 사용합니다. 
* 로그데이터를 저장할 mongoDB와 대용량의 텍스트 데이터를 빠르게 색인하고 검색할 수 있게 elastic search로 mongoDB의 로그를 조회, 저장합니다. 이 로그 데이터들을 Input으로 Flan-t5모델에 넣습니다. Output인 요약문은 MYSQL에 고객정보와함께 저장됩니다.
