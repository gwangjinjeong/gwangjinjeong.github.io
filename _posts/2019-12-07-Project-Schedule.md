---
title:  "MD-CW-with-Deep-learning Project Schedule"
excerpt: "Multi-Distance Continuous Wave를 이용하여 10mm 20mm 30mm로 들어오는 Reflectance 값을 통해서 mua, mus를 구하자."
header:
  teaser: /assets/images/bio-photo-keyboard.jpg
categories:
  - MD-CW
tags:
  - MD-CW
  - DNN
  - Project Schedule
last_modified_at: 2019-12-07T22:00:00+09:00
---
# Abstract
[Google](http://file.mk.co.kr/imss/write/20181226140403__00.pdf), [Apple](https://support.apple.com/en-us/HT204666), Amazon 등 공룡기업들의 웨어러블기기에 대한 관심은 지속적으로 있어왔다.  
대부분의 웨어러블 디바이스는 주로 초당 green LED 수백번 쏘아 PPG data를 통해 심박수를 측정한다. 
하지만 우리 연구에서는 인간의 심박수 뿐만아니라, Hb,HHb, lipido, water까지 인체 조직의 특성을 알고자한다. 그래서 CW를 기술을 이용하기로 하였는데 이것의 특징은 ~하다.
이러한 특징이 잇음에도 불구하고  단순히 Reflectance를 통해서만 optical properties를 얻기에는 상대적인 값만 얻을 수 있기 때문에 한계가 있었다. 하지만 SSFDPM기법을 이용한 DOSI 장비의 경우 optical properties를 구하는데 SS와 6개 파장을 통해서 650nm부터 1000nm까지의 모든 주파수대역의 mua, mus를 구할 수 있었다. 하지만, 장비의 크기가 매우 크기 때문에,  웨어러블 장비를 사용하기에는 어려움이 있었다.
이번 연구에서는 CW를 통해서 DOSI와 같은 성능을 내기 위하여 Deep learning을 이용하도록 할것이다.

# Introduction
1. What is the SSFDPM
2. What is the MD-CW
3. How to combine SSFDPM and MD-CW 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk3NDEzNzYzMl19
-->