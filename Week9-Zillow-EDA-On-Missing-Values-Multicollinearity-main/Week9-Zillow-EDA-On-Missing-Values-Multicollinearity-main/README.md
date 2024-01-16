# Week9-Zillow-EDA-On-Missing-Values-Multicollinearity

발표자 : 

[Zillow EDA On Missing Values & Multicollinearity](https://www.kaggle.com/code/viveksrinivasan/zillow-eda-on-missing-values-multicollinearity/notebook)

- msno.bar

df_train으로 지정한 트레인 데이터셋에 대한 결측치를 바 형태의 차트로 시각화 해준다.

color 파라미터는 RGB를 지정해주는zzx 것이다.

Bar chart로 확인하면 수치적으로도 편하게 볼 수있다.

비어있는 부분이 결측치

- msno.matrix

df_train으로 지정한 트레인 데이터셋에 대한 결측치를 매트릭스로 시각화 해준다.

color 파라미터는 RGB를 지정해주는 것이다.

매트릭스가 출력되는데 흰색으로 표현된 빈칸들이 결측치이다.

<img width="1033" alt="Untitled" src="https://github.com/kaggle-study-230311/Week9-Zillow-EDA-On-Missing-Values-Multicollinearity/assets/80809190/16d5ebf2-c7d9-4792-a043-9f97c9f8efcf">

[https://hong-yp-ml-records.tistory.com/14](https://hong-yp-ml-records.tistory.com/14)

- msno.heatmap

heatmap 을 통해서 상관관계를 나타낸것이다.

1에 가까울수록 양의상관, -1에 가까울수록 음의상관 관계이다.

- df.fillna

메서드는 DataFrame에서 결측값을 원하는 값으로 변경하는 메서드입니다.

[https://wikidocs.net/153209](https://wikidocs.net/153209)

- preprocessing.LabelEncoder()

문자를 0부터 시작하는 정수형 숫자로 바꿔주는 기능을 제공합니다.

[https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=wideeyed&logNo=221592651246](https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=wideeyed&logNo=221592651246)

- .fit()

fit 메소드를 이용해 데이터 훈련

[https://atotw.tistory.com/412](https://atotw.tistory.com/412)

- .transform()

train data로부터 학습된 mean값과 variance값을 test data에 적용하기 위해 transform() 메서드를 사용합니다

[https://deepinsight.tistory.com/165](https://deepinsight.tistory.com/165)

- np.percentile()

백분위수 구하기

<img width="537" alt="Untitled 1" src="https://github.com/kaggle-study-230311/Week9-Zillow-EDA-On-Missing-Values-Multicollinearity/assets/80809190/efd84474-310f-4596-a686-7b68f1fa032f">

[https://m.blog.naver.com/wideeyed/221433769807](https://m.blog.naver.com/wideeyed/221433769807)

- xgb.DMatrix()

**DMatrix**는 넘파이 입력 파라미터를 받아서 만들어지는 XGBoost의 전용 데이터 세트입니다.

*XGBoost를 사용하기 위해서는 DMatrix 형태로 변환해 주어야 합니다*

[https://jaaamj.tistory.com/38](https://jaaamj.tistory.com/38)

[https://zephyrus1111.tistory.com/232](https://zephyrus1111.tistory.com/232)

- .get_fscore()

단순히 모든 트리에 주어진 기능의 존재를 추가하는 것

[https://cran.r-project.org/web/packages/xgboost/xgboost.pdf](https://cran.r-project.org/web/packages/xgboost/xgboost.pdf)
