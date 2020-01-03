---
title:  "주피터 노트북 원격으로 이용하기"
excerpt: "os library를 이용해서 폴더 내 파일 목록 가져오기"
header:
  teaser: /assets/images/bio-photo-keyboard.jpg
categories:
  - JupyterTip
tags:
  - passwd
  - remote
last_modified_at: 2020-01-03T12:00:00-05:00
---
1. anaconda 실행
2. 코드 입력
	``` cmd
	 jupyter notebook password
	 ```
3.  시작 위치 변경 for 보안
4. openssl for 보안
- git bash 열기
- ```pwd```로 현재 위치 확인
	``` git
	openssl req -x509 -nodes -days 1000 -newkey rsa:1024 -keyout mycert.pem -out mycert.pem
	```
-  확인한 위치에서 mycert.pem을 가지고 오기
- `jupyter_notebook_config.py`를 열어서 아래의 내용을 입력.
	``` python
	c.NotebookApp.certfile ='C:/mycert.pem가 있는 절대 경로'
	```
- 
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDc0NTQ1MzAsLTk0NzQwNTk3NSw3MzA5OT
gxMTZdfQ==
-->