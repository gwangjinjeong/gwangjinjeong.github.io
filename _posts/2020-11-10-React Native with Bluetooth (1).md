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
eyJoaXN0b3J5IjpbLTQ1NTkyMTcxMiwxMjYyNDU4MTQ2LDQ5ND
cxMDAwOV19
-->