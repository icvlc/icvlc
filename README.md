# 💡 Li-Fi 무선 통신 기술을 이용한 차량 간 정보 송수신 장치 🚗🚗

## Li-Fi 란?

라이트 피텔리티(Light-Fidelity)'의 줄임말. 빛을 사용하여 장치간에 데이터를 전송하는 무선 통신 기술.
기술적으로는 가시광선, 자외선 및 적외선을 이용하여 고속으로 데이터를 전송할 수 있지만, 현재는 LED 램프를 이용한 가시 광선 통신(VLC) 만 가능하다. 현재의 무선통신은 (300MHz-30GHz) 주파수 사용, 그러나 Li-Fi는 80THz-750THz(1THz=1,000GHz)의 넓은 대역폭의 주파수를 사용하므로 주파수 혼선 없이 통신이 가능하다. 빛을 이용하기 때문에 전자기 간섭에 취약한 군대, 병원, 항공기 등에서 안전하게 사용할 수 있다.
가시광 통신 (VLC)은 매우 빠른 속도로 LED의 전류를 끄고 켜는 방식으로 작동한다. 사람 눈으로는 깜박임을 인지할 수 없다.
Wi-Fi 대비 10배 저결하고 훨씬 빠르며 짧은 범위로 통신하며 벽을 통과하지 못하기 때문에 외부의 해킹으로부터 안전하다.
항공, 병원, 차량, 광고, 교육 등 산업 전 분야에서 활용 가능하다.


## 프로젝트 소개
헤드라이트를 이용한 차량간 VLC(Visual Light Communication) 통신
- 아우디의 Matrix LED, BMW의 Adapted LED 등 자동차 헤드라이트에 LED가 점차 적용되는 추세
- 인간이 인지하지 못하는 속도로 헤드라이트를 깜빡거려 앞차에게 데이터를 전송해 행동을 유도
  - Ex. 엠뷸런스가 사이렌을 울리는 대신 앞차에게 비켜줄 것을 부탁하는 메세지 전송
  - Ex. 경찰이 추격중인 차량에게만 메세지를 전송해 멈출것을 명령

## 일정
- 화요일 - 통신 확인(맨체스터 코드), 속도 튜닝
- 수요일 - 개발 완료(LCD에 출력, STT로 텍스트 입력)
- 목요일 - 발표 준비(우드락, 발표자료), 테스트

## Arduino Circuit Diagram
![VLC Basic Diagram - circuito.io](https://user-images.githubusercontent.com/14247340/67360934-2c678680-f5a2-11e9-9c0d-18845fe25af1.png)

## 시연 영상
유튜브 업로드

## 향후 발전 방향
- 가로등으로부터 실시간 도로 데이터 수신 (Li-Fi)
- 터널내 차량의 정확한 위치 및 속도 측정 (GPS 보조)