# week6-Beat-the-benchmark-
참가자: 김하윤, 박샛별, 장병용 

# 1.데이터

## **Data fields**

- **id** - a unique identifier for each trip
- **vendor_id** - a code indicating the provider associated with the trip record
- **pickup_datetime** - date and time when the meter was engaged
- **dropoff_datetime** - date and time when the meter was disengaged
- **passenger_count** - the number of passengers in the vehicle (driver entered value)
- **pickup_longitude** - the longitude where the meter was engaged
- **pickup_latitude** - the latitude where the meter was engaged
- **dropoff_longitude** - the longitude where the meter was disengaged
- **dropoff_latitude** - the latitude where the meter was disengaged
- **store_and_fwd_flag** - This flag indicates whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server - Y=store and forward; N=not a store and forward trip
- **trip_duration** - duration of the trip in seconds

## 2.  feature 생성

- date/distance/count/speed

# 3. Xgboost

[[ML] 분류(Classification) - XGBoost, LightGBM](https://m.blog.naver.com/sjy5448/222613082311)

- **민감하게 조정해야하는 것**
    - booster 모양
    - eval_metric(평가함수) / objective(목적함수)
    - eta
    - L1 form (L1 레귤러라이제이션 폼이 L2보다 아웃라이어에 민감하다.)
    - L2 form
- **과적합 방지를 위해 조정해야하는 것**
    - learning rate 낮추기 → n_estimators은 높여야함
    - max_depth 낮추기
    - min_child_weight 높이기
    - gamma 높이기
    - subsample, colsample_bytree 낮추기
