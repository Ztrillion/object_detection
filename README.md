# 실시간 도로상황 인식 ai개발

- 표지판, 차량 등 총 117개의 클래스

- 목표 mAP 80%이상

## ISSUE


- AI MODEL : YoloV5 -> 모델변경 불가

- 기존 AI모델링 진행업체 최고 수치 42.7%

- 총 117개의 CLASS중 일부 CLASS만 데이터가 밀집되어 있으며, 전체적으로 고르게 분포되어 있지않음
  


## 진행상황 최신 23년 7웛 10일

| EPOCH | 기존 업체 (mAP) | 4월 3일(mAP)        | 7월 10일(mAP)      |
| ----- | --------------  | ------------------- |------------------- |
| BEST  | 42.7%           | 67.5%               | 81.4%              |

### ORIGINAL DATA

- Class num -> 117EA

- Class count min -> 1

- Class count max -> 13,000

    ![original_class](https://github.com/Ztrillion/object_detection/blob/master/plots/original_class.png)




## preprocessing data

- Class count min -> 1

![prep_class](https://github.com/Ztrillion/object_detection/blob/master/plots/prep_class.png)
