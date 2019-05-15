# RecSys 2019 Study Reo
[2019.03.03 ~ ing]
* hello everyone:) 
* I'm participating in `RecSys2019 Challenge` this year! I'm new to the recommeder system so I'm enthusiatic about learning RC from A to Z!"
* Anybody interested in RC like me, let's study, discuss, and play together! :)) 

## Udemy 
- [url] https://www.udemy.com/building-recommender-systems-with-machine-learning-and-ai/learn/v4/content

## Boaz Recsys Challenge Timestamp
- 2/28: lstm 이용해 시계열 피처 사용하는 방법
- 3/7: dataset EDA 공유, surprise package 쓰기 위해 데이터 가공할 방법 공유 
       공통 과제: y 파악하기, udemy강의 5,6,7강 듣기 
- 3/8: dataset 토의 (`impressions`와 `y`값의 차이, trainset(11월 1일-6일) testset(11월 7일-8일),feature engineering 방향 토의: user-based와 item-based로 구분하여), 
       basic recommedation function 구현 (item의 `n_click` 기반)
       승진 승민 과제: session-based algorithm 찾기
       보정 효선 과제: feature engineering 하기
- 3/14: ??
- 3/21: feature engineering공유, content-based (n_click, item_properties)
- 3/28: 중간발표
- 4/4: Algorithm 공유, timeline 정하기
- 4/5: 1. content based 이용해 item feature로 similarity matrix 생성(보정, 효선) 2. svd++ 모델 논문 읽고 구현
- 4/11: (전체회의) item similarity matrix와 algorithm 공유 
- 4/12: 1. collaborative filtering matrix 생성 2. MF 모델 구현
- 4/28: *Baseline Algorithm D-day : score 점수 내기
- 5/6: submission #1 : [public score 0.591]
- 5/9 : (회의) baseline model에서 ranking 높이는 방법을 회의함. -> baseline에서 interaction하지 않은 item은 item similiarity로 ranking 매기기. [역할분배: 승진: item meta data에서 item property df 만들기 / 승민: item dwelling time feature생성 / 효선: item similarity ranking function구현] (5/15 수까지 submission해서 score 내기)
- 5/11 : submission #2 : [public score 0.596] baseline + item similarity with cosine (L2)
- 5.15 : submission #3 : [public score 0.61] train.csv를 user_id 기반으로 test.csv와 합쳐 reference 빈도로 sorting
- 5/16 : (중간정검 boaz)


- 6/30: *leaderboard End

# Personal Study Timestamp
- 3/30: [Collaborative Filtering] 모델 쓰기 위해서는 user * item sparse matrix가 필요함. 어떻게 만들 것인지 공부했다. 
- 4/4: [Matrix Factorization] pca 공부, svd, svd++ 모델 공부 
- 4/5: [Matrix Factorization] surprise package에 svd 쓰기 위해 dataset (user_id, item_id, rating)만듦. /rating을 만들기 위해 고민했는데 session-based 기 때문에 다른 approach를 선택해야한다는 생각이 들었다. RNN?!/ RNN논문 읽기 
- 4/25: [EDA] 모델링을 위해 데이터 EDA 다시 실행. user action pattern을 보기위해 특정 유저들의 행동 변화를 트리바고 사이트에서 확인함.
- 5/4 : [Modeling] 모델 공부를 하다가 문득 데이터의 x와 y를 제대로 이해해야 맞는 모델을 구축할 수 있다는 생각이 들었다. 그래서 EDA를 다시 해본 결과 user가 'clickout'하기 직전까지 interaction한 item을 사겠다는 생각이 들어서 number of interaction을 기준으로 sorting 했다. [Public Score: 0.591]
