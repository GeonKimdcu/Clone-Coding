## [Dacon] 펭귄 몸무게 예측 경진대회<br>

---

### 출처: DACONIO님 코드 (https://www.dacon.io/competitions/official/235862/codeshare/4031?page=1&dtype=recent)
<br>

### 데이터 소개

#### Files] 
① movies_train.csv - 2010년대 한국에서 개봉한 한국영화 600개에 대한 감독, 이름, 상영등급, 관객수 등의 정보가 담긴 데이터<br>
② movies_test.csv - 관객수를 제외하고 movies_train과 동일<br>
③ submission.csv - 제출 파일의 형식<br>
<br>

#### Column_name Description]
1. Species: 펭귄의 종을 나타내는 문자열<br>
2. Island : 샘플들이 수집된 Palmer Station 근처 섬 이름<br>
3. bill_length_mm : 펭귄 옆모습 기준 부리의 가로 길이<br>
4. bill_depth_mm : 펭귄 옆모습 기준 부리의 세로 길이<br>
5. flipper_length_mm : 펭귄의 팔(날개) 길이 <br>
6. Sex : 펭귄의 성별 <br>
7. body_mass_g : 펭귄의 몸무게(g)

<br>

### 대회 규칙
- 평가지표: RMSE
- 해당 평가 산식을 써야 함.
```
def RMSE(true, pred):
    score = np.sqrt(np.mean(np.square(true-pred)))
    return score
```


### 요약
- GradientBoostingRegressor, NGBRegressor, LGBMRegressor, XGBRegressor, CatBoostRegressor, RandomForestRegressor 총 6가지 모델의 앙상블 기법으로 최종 결과 도출.
