# 실시간 도로상황 인식 ai개발

- 표지판, 차량 등 총 117개의 클래스

- 목표 mAP 80%이상

## ISSUE


- AI MODEL : YoloV5 -> 모델변경 불가

- 기존 AI모델링 진행업체 최고 수치 42.7%

- 총 117개의 CLASS중 일부 CLASS만 데이터가 밀집되어 있으며, 전체적으로 고르게 분포되어 있지않음
  


## 진행상황 최신 23년 7웛 10일

| EPOCH | 기존 업체 (mAP) | 4월 3일(mAP)        | 4월 3일(mAP)       |
| ----- | --------------  | ------------------- |------------------- |
| BEST  | 42.7%           | 0.675%              | 81.4%              |

### ORIGINAL DATA

- Class num -> 117EA

- Class count min -> 1

- Class count max -> 13,000

    ![original_class](https://github.com/Ztrillion/object_detection/blob/master/plots/original_class.png)

- Boxplot

  ![original_boxplot](https://github.com/Ztrillion/object_detection/blob/master/plots/original_boxplot.png)



## preprocessing data

- Class count min -> 1
- Class count max -> 3500

![prep_class](https://github.com/Ztrillion/object_detection/blob/master/plots/prep_class.png)

- Boxplot

![prep_boxplot](https://github.com/Ztrillion/object_detection/blob/master/plots/prep_boxplot.png)

---

- 데이터 맥스값을 조절하고 분포를 조금만 맞췄는데도 불구하고 성능지표 37프로 이상 상승
- CLASS가 117개 이지만 original data 자체가 클래스 편향이 심하고 밀도가 낮아 모델 성능의 한계가 있음. 
- **<u>수집과 가공단에 class count 3,000개 미만인 class부터 모두 1,000개씩 수집 및 가공 요청</u>**
- 4월말 데이터 분포 확인 후 mAP지표 확인
