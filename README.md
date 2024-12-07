# mediproject

의료 데이터를 기반으로 딥러닝을 적용해본 프로젝트입니다.

캐글 및 공개된 의료 데이터셋(1GB-30GB)를 활용하였고


1. 반려동물 근골격계 질환 분류(X-ray)
2. 흉부 X-ray 기반 성별 분류
3. 위 용종 분류
### 4. 치아 질환 분류(Object Detection) - 포트폴리오 프로젝트입니다
5. 피부암 분류 실습(Segmentation)
6. 식물 질병 분류(Self-supervised Learning)




### 데이터 EDA
1. 데이터 분포 확인
2. 의료 데이터에 대한 이해(CT, X-ray 데이터, 복셀, DICOM)
   

### 데이터 전처리
1. 데이터 Load (torch 변환)
2. 메타데이터 Annotation 매핑
3. merge, dropna
5. 데이터 균형화 -> class weight 조정, 업/다운 샘플링, augmentation, SMOTE기법
6. 범주형 데이터 : 원핫인코딩, 임베딩
7. train, val, test 셋 분리
8. 이미지 Augmentation(torchvision, Albumentation) 시각화
9. 샘플 제한, random화

### 모델 훈련
1. 모델 아키텍쳐 구조(테일, 백본, 헤드)
2. Batch normalization 값 조정.
3. Loss Function과 출력층 정으
4. WanB API활용 모델 성능 시각화 및 추적

### 분류 모델 성능 평가
1. Precision, Recall, F1 score 출력


### 해본것.
1. Softmax 대신 Tanh
2. 어설픈 가중치 초기화는 세그멘테이션 훈련을 불안정하게 함
3. lossfunction에 sgd 활용한것. Adam이 효과가 좋았음
