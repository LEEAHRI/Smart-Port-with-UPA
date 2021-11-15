## 울산항만공사와 협업한 프로젝트 입니다.
(비용문제로 AWS 서버 2021-10-14일 이후로 비활성화 하였습니다.)

프로젝트 진행 기간 : 2021-08-02 ~ 2021-08-30

app.py : 웹을 실행시키는 파일로 flask 기반으로 작동됩니다. 현재 AWS EC2를 통해 배포 중입니다.
※ 고도화 작업으로 디버깅이 끝나지 않았습니다.

## Post-Factory
자동차 화물 수출 작업을 OCR기법을 통해 Data 적재까지 자동화 하는 서비스 입니다.

Tessaract API를 이용한 OCR을 사용해 차대번호를 인식, 분석합니다.
자동검수 프로세스를 통해 쌓이는 Data를 정보공유 플랫폼에서 한눈에 확인할 수 있습니다. 

## 프로젝트의 주요 기능 및 구조
<img src="https://user-images.githubusercontent.com/71698417/141727675-6e3d15e2-8d4f-4c8b-84a7-bd5248cc02f5.png">

- 1차,2차 검수원 하역사등록 및 로그인
- 선사 스케줄표 구현
- OCR 차대번호 분석 구현
- 정보공유 dashboard 

## ERD
<img src="https://user-images.githubusercontent.com/71698417/141714314-5a2729b2-c71d-4484-8b28-9e884f470915.JPG" width="500">




# 실행 방법
1) localCamera 폴더를 clone 받으시고 실행을 시킵니다. (저자는 pycharm 환경에서 실행을 시켰습니다.)
2) AWS의 주소(http://3.20.99.214:4997/)로 접속 후 사용이 가능합니다.

    ※ 웹은 이미 AWS로 배포 중임으로 AWS 주소로 접속이 가능하나 OCR 페이지로 이동이 불가능합니다.
    OCR은 로컬 카메라를 사용하기 위해 git의 localCamera 폴더를 받으시고 local에서 실행이 가능합니다.
    
    ※ localCamera를 실행을 시켜도 되지 않는 경우 line87 : cam = cv2.VideoCapture(1)의 숫자를 카메라가 연결되있는 index로 변경하면 가능합니다.
   
