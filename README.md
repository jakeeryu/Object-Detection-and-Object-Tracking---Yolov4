# Object Detection and Object Tracking - YOLOv4

![example_video](https://user-images.githubusercontent.com/106287761/223606020-64ca9609-fc7f-40f6-a0d1-0d19c13fb082.gif)

### 프로젝트 주제
* 고속도로의 고정 카메라 영상을 통한 차량 객체 탐지 및 추적 딥러닝 모델

### 프로젝트 목적
* 영상 데이터 처리 방법 학습
* Computer vision을 통한 객체 탐지 및 추적 방법 학습

### 데이터 소개
* Pixabay에서 저작권이 없는 총 4개 상황의(밤, 확대, 흐림, etc.) 교통 CCTV 영상을 사용
* 영상 크기는 6.2mb 에서 최대 25mb 크기의 mp4 영상 파일을 사용

### 프로젝트 결과
* 탐지된 차량에 bounding box와 center point를 부여
* 고유 id 번호가 부여되어 center point 기준 프레임 간의 빗변 거리를 측정하여 객체 추적

### 개선점
* id 번호가 같은 물체에게 새로 부여되는 경우가 있었음
    * 객체 추적 과정에서 새로운 객체로 인식되는 과정 관찰 필요
        * center point 빗변 거리 계산 과정 또는 물체 전처리 과정 예상

* 자동차가 아닌 운전자 얼굴 인식 및 추적 id 부여
    * 탐지 객체 면적을 지정하여 조정

* 다른 사전학습 모델을 사용하여 객체 인지 정확도 비교
