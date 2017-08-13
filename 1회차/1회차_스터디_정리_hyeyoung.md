1회차 스터디 정리
--------------

1. 대상 오픈소스 선정
> elasticsearch : https://github.com/elastic/elasticsearch


2. 선정 이유

> 로그 검색 엔진으로 elk stack 을 회사에서 사용하고 있으며,<br/>
elastic search의 java api와 lucene 라이브러리를 사용하여 코드를 짜본 경험이 있음.

3. Elastic Search 개요
> elastic search는 shay banon이 개발한 lucene 라이브러리를 기반으로 하는 고성능 분산 검색 엔진이다.<br />
(lucene은 독립 시스템이 아닌 색인과 검색을 가능하게 하는 라이브러리이다.) <br />
elasticsearhc는 자바로 개발된 오픈소스로 RestFull API 를 통해 검색 및 색인 관리 등 여러 기능을 사용할 수 있다. <br /> <br />
대게 elastic search + log stash + kibana (ELK stack) 를 묶어서 대용량 로그 검색 시스템으로 사용한다. <br />
> * elastic search : 데이터를 여러 노드에 분산하여 저장하는 시계열 데이터 저장소로, lucene의 기능을 대부분 지원해 분산 검색 엔진으로 사용됨 <br />
> * log stash : 수집할 로그를 선택하여, elastic search 에 인덱싱해 로그를 전송하는 역할 <br />
> * kibana : visualization을 담당, 수집된 로그를 시각화함.<br />

4. 오픈소스 프로젝트 가져오기 및 메인 저장소와 동기화

<pre>
1) https://github.com/elastic/elasticsearch 내 레파지토리로 fork 함
2) git clone https://github.com/pk8498/elasticsearch.git
3) git remote add upstream https://github.com/elastic/elasticsearch
4) git pull upstream master
</pre>
