# opencv_pose_detection
Study for OpenPose<br>
사람을 움직임 및 포즈를 탐지하는 OpenPose 모델 실습 코드입니다.

# Requirement

1. 가장 먼저 MPI 및 COCO 모델이 필요합니다. 본인이 해당 알고리즘을 통해<br> 
직접 학습시킨 모델이 있다면 그것을 사용해도 무방합니다.

MPII Model

http://posefs1.perception.cs.cmu.edu/OpenPose/models/pose/mpi/pose_iter_160000.caffemodel

COCO Model

http://posefs1.perception.cs.cmu.edu/OpenPose/models/pose/coco/pose_iter_440000.caffemodel

2. 해당 모델을 사용할 수 있는 OpenCV 라이브러리가 필요합니다.
```python
pip install opencv-python
```

# Getting Started
1. 먼저 설치한 각각의 링크에서 설치한 모델을 해당 코드의 model 디렉터리 내에 넣습니다.<br>
그리고 다음과 같이 각각의 모델 및 파라미터 파일 이름을 다음과 같이 바꿔주세요.
```python
λ cd model\
test.md

λ ls
coco.caffemodel  coco.prototxt  mpi.caffemodel  mpi.prototxt  test.md
```

2. input 디렉터리 내에 움직임을 탐지할 이미지 혹은 비디오 파일을 넣어줍니다.<br>
Image: jpg or png or jpeg<br>
Video: mp4 or avi<br>

3. 이미지를 탐지할 것이라면 image.py, 비디오를 탐지할 것이라면 video.py를 실행시켜 주세요.
```python
>>> python image.py
OR
>>> python video.py
```
4. 생성된 미디어 파일은 output 디렉터리에서 확인할 수 있습니다.
