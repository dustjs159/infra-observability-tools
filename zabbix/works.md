Zabbix 동작 방식
======================
![how_to_zabbix](https://github.com/dustjs159/infra-observability-tools/assets/57285121/e2f34ff1-5cac-416b-a7a0-4bdb32ed3a9f)

Zabbix는 Zabbix Server <-> Zabbix Agent간 통신을 통해 모니터링 대상의 지표를 수집하게 된다.

* Zabbix Server : Zabbix 중앙 서버
* Zabbix Agent : 모니터링 대상 내에 설치되는 Zabbix Agent. (모니터링 대상이라고 보면 된다.)

이 때 수집할 지표들을 Zabbix Server가 Zabbix Agent로 부터 가져오느냐, 아니면 Zabbix Agent가 Zabbix Server 쪽으로 넘겨주느냐에 따라 Active / Passive 방식으로 구분한다.

![how_to_zabbix_2](https://github.com/dustjs159/infra-observability-tools/assets/57285121/3f93c0c3-b7de-4ff2-90ac-0a86ef1fea73)

* Passive 방식 : Zabbix Server가 Zabbix Agent로 부터 지표를 가져오는 방식
* Active 방식 : Zabbix Agent가 Zabbix Server쪽으로 지표를 넘겨주는 방식



