# Activity-Detection-using-IMU-sensor
## 환경설정
```bash
sudo apt install python3-venv
cd ~/projects
python3 -m venv ENV_NAME
source ENV_NAME/bin/activate

pip install tensorrt matplotlib numpy pandas seaborn scipy sklearn keras tensorflow

...
deactivate
```

<img src="pics/2.jpg">

IMU (관성 측정 장치) 센서와 딥 러닝의 힘을 이용한 사용자 활동 감지. 스마트 웨어러블에서 가속도계 데이터를 사용하여 지속적인 활동 감지를 수행하며, 이는 깊은 활동 모니터링 및 예측 시스템에 사용될 수 있습니다.

사용하는 데이터 세트는 여러 사람들이 여섯 가지 다른 운동(계단 내려가기, 조깅, 앉기, 서있기, 계단 올라가기, 걷기)을 수행하는 동안 함께 가지고 다니는 스마트폰에서 측정된 가속도계 데이터의 모음입니다. 각 운동에 대해 x, y, z 축의 가속도와 타임스탬프 및 사람 ID가 캡처되었습니다.

이러한 사용 가능한 데이터를 사용하여 신경망을 훈련시켜 스마트폰을 가지고 있는 사람이 여섯 가지 활동 중 어느 것을 수행하는지 해석할 수 있습니다. 기존 데이터로 신경망을 훈련한 후, 새로운 데이터가 주어졌을 때 정확하게 활동 유형을 예측할 수 있습니다.

사용 가능한 데이터를 기반으로 DL 모델은 각각의 여섯 가지 활동을 구분하는 방법을 학습합니다. 그런 다음 새로운 데이터를 신경망에 넣으면 어떤 활동을 사용자가 해당 시점에 수행하고 있는지 알수 있습니다.


<img src='pics/3.jpg'>
