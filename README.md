# 차량 간 정보 전달을 위한 Li-Fi 무선 통신

> `ICVLC`는 **Inter-Car Visible Light Communication**의 약자로, 차량 간 정보 전달을 위한 Li-Fi 무선 통신 프로젝트이다.

## Li-Fi란?

`Li-Fi`는 **Light Fidelity**의 줄임말로, 빛을 이용한 무선 통신을 가능하게 하는 기술이다. 이론적으로 가시광선, 자외선 및 적외선을 모두 사용할 수 있지만 현재는 **가시광선**을 이용하는 연구가 활발히 이루어지고 있다. `Li-Fi`는 기존의 무선 통신 주파수 대역과는 다른 대역을 사용하기 때문에 현재 포화 상태인 2.4GHz Wi-Fi 대역과 겹치지 않아 주파수 혼선을 감소시킬 수 있다. 또한 벽을 통과할 수 없는 빛의 특성으로 인해 외부로부터의 **감청 및 해킹에 상대적으로 안전**하므로 **병원, 군사 시설** 등에서 특수한 목적으로 사용할 수 있다. 통신에 사용되는 광원은 매우 빠른 속도로 켜졌다 꺼졌다를 반복하므로 사람의 눈으로 깜빡임을 감지하기 어렵다. 따라서 실내등 또는 가로등과 같은 곳에 `Li-Fi` 통신 장치를 설치하는 것이 가능하다는 장점이 있다.

## 프로젝트 소개

차들이 달리는 도로 위에서는 **차량 간의 소통이 제한적**이다. 응급 환자를 태운 구급차가 뒤에 있어도 길을 비켜주지 않거나, 경적이나 전조등을 이용한 간접적인 소통방식으로 오해를 불러일으키기 쉽다. 연쇄 추돌 사고와 같은 돌발적인 상황에서도 앞 차로부터 메시지를 받을 수 있다면 대형사고를 피할 수 있을 것이다. 이러한 문제점을 해결하기 위해 차량 간 정보 전달을 목표로 프로젝트를 구성하였다. `ICVLC`는 도로 위와 차량에 다양한 빛을 내는 광원이 있다는 것에 아이디어를 얻어 `Li-Fi` 무선 통신 기술을 활용하여 **차량 간 정보 전달을 구현한 프로젝트**다.

최근 자동차의 전조등은 (아우디의 Matrix LED, BMW의 Adapated LED 등) LED로 변경되고 있는 추세이다. 자동차의 전조등과 후미등에 `Li-Fi` 무선 통신 장치를 설치할 수 있다면 근거리 차량 간 정보 전달이 가능할 것이다.

## 구현 코드 저장소

- [Docs](https://github.com/icvlc/icvlc) - 프로젝트 문서 저장소
- [Sender](https://github.com/icvlc/sender) - STT(Speech to Text)를 이용하여 입력된 메시지를 블루투스로 전송하는 모바일 앱
- [Emitter](https://github.com/icvlc/emitter) - 블루투스로 입력받은 메시지를 맨체스터 부호화하여 LED를 깜빡이는 아두이노 프로그램
- [Receiver](https://github.com/icvlc/receiver) - 조도 센서를 이용하여 부호화된 메시지를 해석해 시리얼 포트로 출력하는 아두이노 프로그램
- [Player](https://github.com/icvlc/player) - 시리얼 포트로 읽은 메시지를 TTS(Text to Speech)를 이용하여 출력하는 프로그램


## 일정

- **2019/10/21 (월)** - 프로젝트 계획
- **2019/10/22 (화)** - 기본 아두이노 보드 제작, 통신 구현
- **2019/10/23 (수)** - 통신 코드 개선, 아두이노 블루투스 모듈 추가, 메시지 입력용 APP 구현, 문서화
- **2019/10/24 (목)** - 우드락 자동차 모형 제작, 테스트 및 데모 영상, 발표자료 준비
- **2019/10/25 (금)** - 프로젝트 발표

## Arduino Circuit Diagram

![ICVLC Circuit Diagram - circuito.io](https://user-images.githubusercontent.com/14247340/67408051-62812680-f5f3-11e9-906c-4dd95658a2a1.png)

> 블루투스 모듈을 추가한 최종 아두이노 회로도

## 발표 자료

[SLIDE.pdf](https://github.com/icvlc/icvlc/blob/master/SLIDE.pdf)

## 시연 영상

유튜브 영상 링크 (준비 중)

## 향후 발전 방향

- 차량 간 양방향 통신으로 확장
- 연쇄 추돌과 같은 돌발적인 요인으로 인한 위험(급제동)을 앞 차로부터 수신하여 2차 사고 예방
- 가로등으로부터 실시간 도로 데이터 수신
- GPS를 보조하여 터널 내 차량의 정확한 위치 파악

## Team

- [Hanjun Kim - hallazzang](https://github.com/hallazzang)
- [DONGGEON LIM - PW486](https://github.com/PW486)
- [JiwoonWon - JWWon](https://github.com/JWWon)

## License

[MIT](https://github.com/icvlc/icvlc/blob/master/LICENSE)