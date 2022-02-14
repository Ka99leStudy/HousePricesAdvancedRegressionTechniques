EDA : https://www.kaggle.com/kongnyooong/house-price-tutorial-for-korean-beginners \
다중공선성 : https://eda-ai-lab.tistory.com/8

- 220203 제출 X

- 220210 제출 **0.14400** \
전체 변수에 대하여 이상치 (IQR * 1.5) \
명목형 데이터 > None 처리 \
수치형 데이터 > 0 또는 평균값으로 대체 \
OneHotEncoding \
비슷한 변수끼리 사칙연산 수행하여 새로운 변수 생성 \
수영장, 차고, 지하실, 화로 있다/없다로 변경 \
XGBoost (random_state = 2000)

- 220211 제출 **0.15411** \
수치형/명목형 변수 각각 연관성 높은 순으로 10가지 추출 \
BsmtQual 결측치 None 처리 \
OneHotEncoding \
차고, 지하실 있다/없다로 변경 \
GrLivArea 이상치 2개 제거 \ 
XGBoost (random_state = 2000)

- 220214 제출 **0.13207** \
결측 데이터 처리 (0210과 동일) \
사칙연산, 있다/없다 \
위에 사용된 변수 제거 \
OneHotEncoding \
XGBoost (random_state = 2000)

- 220214(2) 제출 **0.12988** \
GrLivArea 이상치 2개 제거 + 220214와 동일

- 220214(3) 제출 **0.12959** \
Id 변수 제거 + 220214(2)와 동일

- 220214(4) 제출 **0.13007** \
Exterior1st, Exterior2nd 제거 + 220214(3)과 동일

- 220214(5) 제출 **0.13119** \
SalePrice 이상치 2개 제거 + 220214(3)과 동일

- 220214(6) 제출 **0.13247** \
이상치 0.01 제거 + 220214(3)과 동일

- 220214(7) 제출 **0.15618** \
GrLivArea 이상치 2개 제거 \
결측 데이터 처리 (0210과 동일) \
있다/없다 \
ID 제거 \
One-Hot Encoding \
PCA (313 > 50 > 20) \
