---
title:  "Bluetooth 내용정리"
excerpt: "Bluetooth연동을 위한 내용정리 "
header:
  teaser: /assets/images/bio-photo-keyboard.jpg
categories:
  - Bluetooth
tags:
  - Bluetooth
last_modified_at: 2020-11-13T12:00:00-05:00
---
센서의 데이터를 Bluetooth를 통해서 핸드폰으로 데이터를 받고 싶은데 이에 대한 지식이 부족한 상황이다 그래서 인터넷에서 찾은 정보들을 정리하고자 한다.
## 1. 가지고 있는것
* STM32F103
* nRF51822 BLE module
* iPhone 8
## 2. Bluetooth?
주로 블루투스기기 구현방법은 
(1) 'Bluetooth Basic Rate/Enhanced Data Rate (BR/EDR)'
(2) 'Bluetooth with low energy (LE)'
2가지로 나뉠수 있다.  

### 2-1 Bluetooth BR/EDR
스트리밍 오디오와 같은 유저케이스에 적합한 구현방법으로 상대적으로 짧은 커버리지와 연속적인 무선 연결을 지원합니다.
### 2-2 Bluetooth LE
보다 긴 커버리지를 지원하며, 연속적인 무선 연결을 필요치 않지만 짧은 시간동안의 디지털 데이타 전송을 하는 사물인터넷 (IoT : Internet of Things)에 적합합니다. 그리고 장시간 사용을 위해서는 긴 배터리 수명을 필요로 합니다.
### 2-3 Dual-Mode
듀얼모드 칩셋(Dual-mode chipset)도 가능한데, 오디오 헤드셋과 같은 BR/EDR 기기와 웨어러블(Wearable) 또는 비컨(Beacon)과 같은 LE 기기 모두와 연결이 필요한 스마트폰 또는 태블릿을 위해 필요하다.

Reference
[1] https://learn.adafruit.com/introduction-to-bluetooth-low-energy/introduction

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTU2MjI5OTEwXX0=
-->