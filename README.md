# 2018 Winter Co-operative Education Program

## Project Synopsis
- 행사명 : 2018년도 동계 현장실습프로그램(Co-operative Education Program, Co-op)
- 주최 : <a href=https://linc.skku.edu/>성균관대학교 LINC+사업단</a>, <a href=http://www.cyberwin.co.kr/>CyberTechFriend</a>
- 진행 기간 : '19.1.2 ~ '19.2.28
- 내용
  - 현장실습프로그램(Co-operative Education Program)은 학교와 기업이 공동으로 산업체 현장에서 필요한 실무교육 및 실습을 실시하는 산학협력 교육과정입니다. 상장기업, 공공기관, 연구기관 등 다양한 기업에서 현업 역량 잠재력이 뛰어난 본교 학생들을 직접 선발하여 지도교수와 함께 기업에서 제시한 다양한 프로젝트를 수행했습니다.
  - 이 프로젝트에서 저는 EdgeX라는 open source IoT 플랫폼을 스마트팩토리 솔루션 기업인 CyberTechFriend에서 활용할 수 있는지 연구하는 과제를 수행했습니다. Linux 기반의 운영체제의 노트북에 서버를 설치하고, 라즈베리파이 edge 디바이스에 endpoint SDK 배포를 통해 데이터를 수집 후 DB에 저장하였고, 궁극적으로는 Foolproof 기계를 연결하여 IoT service를 구현해냈습니다.
### Purpose
스마트팩토리의 구축에 필수적인 IoT 플랫폼을 연구하여 기업과 기업을 이어주는 서비스의 필요성이 증가하고 있습니다. 산업현장에는 다양한 디바이스가 사용되고 있고 이 디바이스들을 연결하는 IoT 플랫폼을 통해 그들의 효율적인 관리를 가능하게 합니다. 이를 위해 다양한 Open source IoT 플랫폼을 사용하고 이에 대한 각각의 기술적 차이 이해 및 이를 이용한 플랫폼 구현이 목표입니다.
### Necessity
일반적인 중소 기업에서 IoT 플랫폼을 도입하는 비용과 그에 대한 제반 시설을 도입하는 과정에서의 인력 수급등에 있어 어려움이 많습니다. 따라서 proprietary IoT 플랫폼이 아닌 open source 기반의 IoT 플랫폼을 활용하고 이를 활요하기 위한 지식이 필요합니다. 또한, 이러한 open source 플랫폼은 기존의 수요만을 대상으로 하는 플랫폼이 아니라 공급자를 연계할 수 있는 기술 과정이 필요합니다. 따라서 밴더, 모델에 해당하는 스키마를 연구하고 이를 IoT 플랫폼에 누적 시키는 등의 과정을 통해 도입할 필요가 존재합니다. 이러한 과정은 Edge IoT 플랫폼과 Cloud 분석 과정을 도입하여야 가능하고 현 연구의 목표는 Edge 에서의 IoT 플랫폼 연구에 국한하되 Web 표현이 가능하게 하는 것을 목표로 합니다.
### Background Knowledge
- IoT : 사물인터넷 기술은 현재 지속적 성장과 함께 보급, 확산되는 추세입니다. Cisco는 세계사물인터넷 시장이 2022년까지 14조4000억 달러 규모로 성장할 것이라고 예측하였으며 특히 제조업 시장과 관련된 사물인터넷 시장의 규모는 2015년 42억 달러에서 2020년까지 140억 달러 규모로 성장할 것으로 예측되며, 매년 평균 약 27%의 성장률을 보여줄 것으로 전망하였습니다. 현재 제공되고 있는 대다수의 IoT 서비스는 사물이 인터넷에 연결되어 수집된 데이터를 전달해주거나 데이터를 기반으로 사전 설정된 조건에 따라 사용자가 사물을 제어하는 형태입니다. 이러한 IoT 서비스에 적용 가능한 가전, 로봇, 웨어러블 기기 등 다양한 사물이 보급되고 있습니다. 산업 측면의 IoT 인 Industrial IoT의 경우 일반적으로 다양한 기기에서 제공하는 RS485, 232, Modbus 등의 통신 규약에 따른 기존의 데이터를 사물 인터넷 컨버팅 디바이스에 네트워크를 사용하여 Database로 전달하는 것이 일반적인 상황입니다.
중소기업 IT 환경은 일반적으로 시간에 따라 조직 전반에 걸쳐 배치되고 점점 그 네트워크 망의 중요도는 증가되고 있지만 서로 연계되어 있지 않은 경우가 많습니다. 별도의 자동화 시스템으로 구성되어 있어 시설 도처에 고립된 형태로 데이터를 취급하는 형태가 빈번히 발생하게 되고 또 그 고립된 자동화 시스템은 일반적으로 전용 하드웨어에 상주하는 형태여서 개선이 필요한 상황입니다.
- 국내 IoT 기술 개발 현황
    - 국내 IoT 사업체는 1,991개(2016년 기준)이며, 종사자 수 50인 미만의 중·소형 사업체가 80% 이상을 차지하고 있으며 분야별 사업체 수는 서비스 분야가 1,089개 (전체 54.7%)로 가장 많고 그 다음으로 디바이스(24.7%), 네트워크(11.3%), 플랫폼(9.4%) 순서로 조사되고 있습니다.<br>
    - 종사자 규모별 사업체 수는 10 ~ 49인 규모의 사업체가 1,148개(전체 57.7%)로 가장 많고 그 다음으로 1 ~ 9인 규모의 사업체가 472개(전체 23.7%)인 상황이라 기술 개발에 있어서 선진국 대비 부족한 수준을 가지고 있다. 전체적인 기술은 미국 대비 82.9% 수준입니다.  
    <img src=https://i.imgur.com/rGhWcjI.png><img src=https://i.imgur.com/CdbcF9D.png><br>
- 국외 IoT 기술 개발 현황
  - 미국의 사물인터넷 기술 개발 및 투자 현황은 굉장히 활발한 것으로 나타나며, 인텔과 Qualcomm과 같은 대기업들이 가장 활발한 투자를 하고 있으며 많은 벤처 캐피털들의 투자활동도 활발하게 이루어지고 있습니다.<br>
  <img src=https://i.imgur.com/8wykhoJ.png><br>

### Tools
- Ubuntu Laptop
  - IoT platform의 server역할을 수행하기 위한 노트북입니다. Server에 main IoT platform을 설치 후, 이 server에서 수집할 데이터의 타입, 환경변수 등등을 설정한 후 endpoint로 배포할 SDK를 제작했습니다. SDK의 배포는 보통 http post를 활용하여 전달했습니다.
- Raspberry Pi
  - Xenon Foolproof Temperature Request Timer로부터 일정한 주기로 rs485통신을 통해 데이터를 요청하고, 반환받은 데이터를 SDK를 전달받아 설치한 endpoint release를 통해 서버 전달하는 역할을 합니다.
- <a href=http://e-taesung.com/27>SmartQ Foolproof</a>
  - 정해진 통신 프로토콜을 통해 데이터를 반환하는 디바이스입니다.
  - 이 기기에 관한 자세한 내용은 CyberTechFriend에서 진행했던 프리랜서 <a href=https://github.com/CyberTechFriend-Outsourcing-Freelancer/FoolProof>repository</a>에서 확인할 수 있습니다.
- Golang
  - Kaa Opensource IoT Platform에서 endpoint로의 SDK를 배포할 때 개발자가 원하는 로직을 수행하도록 하는 logic을 구현하는 파일인 device.go가 golang으로 프로그래밍되어 있었습니다. 이 파일을 분석하기 위해 개인적으로 golang의 기본적인 코딩 지식을 공부했습니다.
- Python
### IoT Platform
Open source IoT platform 으로 Kaa, Thingsboard, Edge X를 비교하였습니다.
- <a href=https://www.kaaproject.org/>Kaa</a><br>
<img src=https://i.imgur.com/iVJLGhB.png width=100><br>
분산 처리 기반 Open source platform으로 클러스터로 구성되어 있는 서비스를 기반으로 처리하며 각 End Point 에 대한 SDK를 제공하는 형태로 쉽게 디바이스를 붙일 수 있게 되어 있습니다.
- <a href=https://thingsboard.io/>Thingsboard</a><br>
<img src=https://thingsboard.io/images/thingsboard_logo.png width=150><br>
실시간 데이터에 대한 표현영역에서 강점을 가지는 Open source IoT platform 으로서 위젯 형태로 구성된 플랫폼입니다.
- <a href=https://www.edgexfoundry.org/>Edge X Foundry</a><br>
<img src=https://www.pngitem.com/pimgs/m/466-4665404_edgex-foundry-logo-hd-png-download.png width=200><br>
마이크로서비스 기반 분산 처리 되는 형태로 구성되어 있으며 Edge 영역에서의 API를 기반으로한 통신과 데이터 전송을 기반으로 구성되어 있습니다.
### Architecture
- Kaa<br>
<img src=https://i.imgur.com/FqPAAqF.png><br>
- Thingsboard<br>
<img src=https://i.imgur.com/ypql3zk.png width = 500><br>
- Edge X Foundry<br>
<img src=https://i.imgur.com/hqLyJrr.png width = 500><br>
## Project Details
Kaa, Thingsboard, EdgeX 세 개의 Opensource IoT 플랫폼 중 CyberTechFriend 기업에 가장 적합하다고 판단한 플랫폼은 EdgeX이었습니다.
### Edge X 서버 문서 작성
EdgeX설치 가이드 사이트

1. Docker 및 Docker compose설치

2. https://github.com/edgexfoundry/developer-scripts/raw/master/compose-files/docker-compose-delhi-0.7.1.yml 파일 생성, 이름은 docker-compose.yml 로 저장.

3. docker-compose pull
   docker-compose up -d
   docker-compose ps 차례로 실행하기.

4. docker-compose.yml 에서 device-random 주석 삭제

5. docker-compose up -d device-random실행 후

```curl http://localhost:48080/api/v1/event/device/Random-Integer-Generator01/10```

명령어 입력해서 데이터 값 뜨는지 확인.(처음에는 안떳는데 시간이 지나니 되는경우가 있었음)

## Review
S-hero 때 스마트팩토리를 주제로 불량품을 검출하는 시스템 구축을 해보았습니다. 라즈베리파이와 아두이노에 연결된 센서의 데이터를 서버로 보내고, 서버에서 다시 컨베이어벨트의 구동과 서보모터의 가동을 하게하는 시스템이 결국 IoT라는 것을 알게 되었고, 그것을 좀더 확장하여 IoT에 대해 배우고자 이렇게 연구를 하게 되었습니다. 하지만 생각과는 달리, IoT 시스템을 구축하는 것은 생각보다 복잡하였고 설명이 부족해서 사용하기에 쉽지 않았습니다. Kaa 플랫폼의 분석을 거의 완료한 시점에 기업의 입장에서 적합하지 않은 플랫폼임을 알게 되고 EdgeX 플랫폼으로 주제를 바꾸게 되면서 난관에 부딪히기도 했습니다.
결과적으로 이러한 어려움을 이겨내고 결국 IoT 플랫폼을 구축하는데 성공했습니다. 데이터의 실시간 전송과 확인, 여러 디바이스의 연결도 가능하게 되었습니다.
현재 4차 산업혁명과 관련하여 IoT 가 떠오르고 있는데 학부생 입장에서 이러한 연구주제를 가지고 직접 IoT를 경험해보았고, 분석&#183;적용해보았다는 점에서 뿌듯하고 이후로 저에게 많은 도움이 된 프로젝트였습니다.
