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
0. 만약에 iptime과 같은 공유기에 연결되어 있는 경우.    
	- iptime 관리자 페이지 들어가서
	- 포드포워딩   
		- 서버로 사용할 컴퓨터 ip주소, 포트(8888이 기본)    
1. anaconda 실행   
2. 코드 입력   
	``` cmd
	$ jupyter notebook password
	Enter password:  ****
	Verify password: ****
	[NotebookPasswordApp] Wrote hashed password to /Users/you/.jupyter/jupyter_notebook_config.json
	```   

3.  시작 위치 변경 for 보안
	- [https://wonderbout.tistory.com/50](https://wonderbout.tistory.com/50)
4. openssl for 보안
	- git bash 열기
	- ```pwd```로 현재 위치 확인
		``` python
		openssl req -x509 -nodes -days 1000 -newkey rsa:1024 -keyout mycert.pem -out mycert.pem
		```
	-  확인한 위치에서 mycert.pem을 가지고 와서 적절한 폴더에 넣기
	- `jupyter_notebook_config.py`를 열어서 아래의 내용을 입력.   
		``` python
		c.NotebookApp.certfile ="C:/mycert.pem가 있는 절대 경로"
	```   
6. 


참조 페이지
- [주피터 노트북 공식 페이지](https://jupyter-notebook.readthedocs.io/en/stable/public_server.html)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk0NDE3MjA3Niw0NzQ1NDUzMCwtOTQ3ND
A1OTc1LDczMDk5ODExNl19
-->