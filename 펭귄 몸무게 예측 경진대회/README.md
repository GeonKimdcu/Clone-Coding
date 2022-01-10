## [Dacon] 펭귄 몸무게 예측 경진대회<br>

---

### 출처 
1. DACONIO님 코드 (https://www.dacon.io/competitions/official/235862/codeshare/4031?page=1&dtype=recent)
2. DACONIO님 코드 (https://www.dacon.io/competitions/official/235862/codeshare/4071?page=1&dtype=recent)
<br>

### 데이터 소개

#### Files] 
① penguins.csv - 성인 Adélie, Chinstrap 및 Gentoo 펭귄의 크기 및 성별을 포함한 데이터입니다. <br>
Ref. https://www.kaggle.com/resulcaliskan/penguins
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
- 1번 코드: 방정식으로 회귀식을 유도해 간단하게 몸무게 값 예측.
- 2번 코드: K-fold Cross Validation을 활용해 선형 회귀분석으로 몸무게 값 예측.
