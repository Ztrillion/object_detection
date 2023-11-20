# 실시간 도로상황 인식 ai개발 연구과제

- 표지판, 차량 등 총 117개의 클래스

- 목표 mAP 80%이상

- 데이터분석을 통해 AI모델학습 결과를 공유함으로써 문제해결에 대한 주관사 컨설팅 진행


## ISSUE

- AI MODEL : YoloV5 -> 모델변경 불가

- 기존 AI모델링 진행업체 최고 수치 42.7%

- 총 117개의 CLASS중 일부 CLASS만 데이터가 밀집되어 있으며, 전체적으로 고르게 분포되어 있지않음


## 11월 20일
- mAP : 95.1%
- EPOCHS : 400
- OPTIMIZER : ADAM
- BATCH-SIZE : 20

### *TTA 소프트웨어 V&V 인증 시험 완료. 
### *Model Quantization 완료. 

## 4월 3일 

- 모델 학습 및 수집 및 가공 기준 컨설팅 진행
  - 데이터 전처리 후 모델성능 67.5%
  - 데이터 증강 및 밀집도 개선 후 mAP 성능지표와 개선 전 성능지표 비교 분석 보고서 발송
  - 표지판 특성상 데이터 증강 시 제한사항 안내


## 진행상황 최신 23년 11월 20일

| EPOCH | 기존 업체 (mAP) | 4월 3일(mAP)        | 7월 10일(mAP)       | 8월 10일(mAP)      | 11월 20일(mAP)    | 
| ----- | --------------  | ------------------- | ------------------- | ------------------ |------------------ |
| BEST  | 42.7%           | 67.5%               | 81.4%               | 92.7%              | 95.1%             |  



![train-plots](https://github.com/Ztrillion/object_detection/blob/master/plots/results.png)

