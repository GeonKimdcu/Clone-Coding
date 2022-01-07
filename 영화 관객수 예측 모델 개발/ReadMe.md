## [Dacon] 영화 관객수 예측 모델 개발 <br>

---

### 출처: 기세현님 코드 (https://dacon.io/competitions/open/235536/codeshare/2721?page=1&dtype=recent)
<br>
### 데이터 소개
**Files]** <br>
① movies_train.csv - 2010년대 한국에서 개봉한 한국영화 600개에 대한 감독, 이름, 상영등급, 관객수 등의 정보가 담긴 데이터<br>
② movies_test.csv - 관객수를 제외하고 movies_train과 동일<br>
③ submission.csv - 제출 파일의 형식<br>
<br>
**Column_name Description**] <br>
1 title : 영화의 제목
2 distributor : 배급사
3 genre : 장르
4 release_time : 개봉일
5 time : 상영시간(분)
6 screening_rat : 상영등급
7 director : 감독이름
8 dir_prev_bfnum : 해당 감독이 이 영화를 만들기 전 제작에 참여한 영화에서의 평균 관객수(단 관객수가 알려지지 않은 영화 제외)
9 dir_prev_num : 해당 감독이 이 영화를 만들기 전 제작에 참여한 영화의 개수(단 관객수가 알려지지 않은 영화 제외)
10 num_staff : 스텝수
11 num_actor : 주연배우수
12 box_off_num : 관객수 
