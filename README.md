# Data-analysis
실제 데이터를 활용한 데이터 분석


# 프로젝트 순서
|프로젝트 제목|구성원|기간|내용요약|
|------|---|---|---|
|electronic_car_data|개인|23.10.24(1일)|서울시 전기차 충전소 충전량 데이터를 활용한 충전종료시각 예측|
|sangil_dong_commercial_analysis|4인|23.10(3일)|서울 강동구 상일동 상권 분석|


## 1. 서울시 전기차 충전소 데이터 예측
> 서울시 전기차 충전소 충전량 데이터를 활용한 EDA 분석 시각화 충전종료시각 예측을 위한 pycaret 사용
- 데이터: [서울 열린데이터광장 서울시 전기차 충전소 데이터](https://data.seoul.go.kr/dataList/OA-22249/F/1/datasetView.do)

- 목적
  - 종료시각예측을 통해 실제 차량의 대기시간을 예상하고 유동 흐름을 조절 할 수 있는지 확인

- 현배터리양 columns 생성
  - 충전량을 100.0 = 100%로 두고 "충전하기 직전 차에 남아있던 전기량"을 추가
  - 현배터리양 = 100 - 충전량

 
- 충전량 outlier 제거 후 분포 확인
  |box plot|dist plot|
  |------|---|
  |<img style="margin-top: 20px" src='./image/charger_gauge.PNG'> </img>|<img style="margin-top: 20px" src='./image/charger_gauge1.PNG'> </img>|
  
 
- 학습전 최종 데이터
  <img style="margin-top: 20px" src='./image/elect_data.PNG'> </img>

## 2. 서울 강동구 상일동 상권 분석
