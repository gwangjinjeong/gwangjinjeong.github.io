---
title:  "React Native with Bluetooth (1) 환경설정"
excerpt: "Setup Development Environment "
header:
  teaser: /assets/images/bio-photo-keyboard.jpg
categories:
  - React_native
tags:
  - Bluetooth
  - React_native
last_modified_at: 2020-11-10T12:00:00-05:00
---
## 0. Preparation   
**App**
\- iPhone 8
\- Windows 10
\- Visual Code
**Bluetooth**
\- BLE Module: [nRF51822](https://www.nordicsemi.com/Products/Low-power-short-range-wireless/nRF51822)
\- MCU: [STM32F103](https://www.st.com/en/microcontrollers-microprocessors/stm32f103.html)
\- JTAG emulator: [miniJLINK V2.0](https://www.devicemart.co.kr/goods/view?no=33262)

<hr>

**ReactNative의 장점**

-   JavaScript와 React를 안다면 RN을 공부하지 않아도 개발할 수 있다.
-   NPM과 같은 거대한 라이브러리 저장소가 있다.
-   함수형 프로그래밍을 할 수 있다. (Case By Case)
-   Expo를 사용할 수 있다.

**ReactNative의 단점**

-   Facebook에서 ReactNative에 대한 지원을 점점 끊는다.
-   하드웨워 혹은 커스터마이징 혹은 카메라 등 하드한 작업을 하기에는 무리다.
-   네비게이션, 이미지 확대 등 간단한 기능도 지원을 하지 않는다 = 라이브러리를 사용해야한다.
-   오류가 난다면 고치기가 힘들다. 즉 오픈소스에 의지해야하니 오류 잡기가 힘들다.

----------

**Flutter의 장점**

-   Google의 지원이 엄청 빵빵하다.
-   객체지향 프로그래밍 스타일이다. (Case By Case)
-   네비게이션, 카메라 등 Flutter 안에서 모든걸 제공해준다.
-   문서가 매우 잘 정리되어있다. (강의 영상 제공 by Google)

**Flutter의 단점**

-   Google이 갑자기 Flutter를 언제 죽일지 걱정해야한다.
-   모든 Flutter 앱은 구글앱처럼 생겼다. 물론 아이폰도 마찬가지이다.
-   쉽게 구현할 수 있는건 어렵게 해놓고, 어렵게 구현할 수 있는것은 쉽게 해놓았다.(RN 개발자 시점)
-   Dart라는 언어를 처음부터 공부해야한다.
<hr>

위의 장단점이 존재한다. 

## 1. React
### 1. Visual code 설치
 Editor는 Visual code로 사용
### 2. 핸드폰에 Expo client 설치
핸드폰에 시뮬레이션을 돌리기 위한 예물레이터 
### 3. npm 설치
https://nodejs.org/en/
확인시,
```cmd
node -v 
npm -v
로 확인가능
```
### 4. expo 설치
```cmd
npm install --global expo-cli
expo init [AppName]
cd [AppName]
expo start
QR코드 인식후 실행
```


# Bluetooth


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwMjQ4NzAyMzIsLTIxMzQyNzk2MjgsLT
E5NjU1MTM0MTYsLTkxODI4NDM3MCwtNDU1OTIxNzEyLDEyNjI0
NTgxNDYsNDk0NzEwMDA5XX0=
-->