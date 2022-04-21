# 1. 대회 소개
- 대회의 데이터셋은 자유 이용 저작물인 공포 장르 작가들이 쓴 소설 작품 텍스트들이다.   
대회의 목표은 테스트 셋의 문장들의 작가를 정확하게 구분하는 것이다.   
다음은 문장들과 작가들이 매칭되어있는 train 데이터의 예시이다.   
![img](https://user-images.githubusercontent.com/63547654/164422407-b29a5b58-aec1-4dde-b0eb-fb860dcdd3df.jpg)

- 작가는 다음과 같이 3명이다.   
Edgar Allan Poe (EAP)   
HP Lovecraft (HPL)   
Mary Wollstonecraft Shelley (MWS)   

- 대회 사이트 :https://www.kaggle.com/competitions/spooky-author-identification/overview

 

# 2. 데이터 셋 살펴보기
- 파일설명   
train.csv - the training set   
test.csv - the test set   
sample_submission.csv - a sample submission file in the correct format   

- 각 칼럼 설명   
id - a unique identifier for each sentence   
text - some text written by one of the authors   
author - the author of the sentence (EAP: Edgar Allan Poe, HPL: HP Lovecraft; MWS: Mary Wollstonecraft Shelley)   
 

# 3. 스코어 점수 계산 방식, 제출파일 형식
multi-class logarithmic loss를 사용한다.
![다운로드](https://user-images.githubusercontent.com/63547654/164423024-cb70d251-0f30-46ff-8195-e7fcb0f0f698.jpeg)

다음과 같이 각 문장의 각 클래스에 대한 확률을 제출하면 된다. 제출파일에서 score식을 계산해 순위가 매겨진다.
![다운로드](https://user-images.githubusercontent.com/63547654/164423162-d2e04388-3fcb-4e61-9201-dd7d33cc9f67.jpeg)

 

 
# 4. 대회참여기간, 상금 
December 15, 2017 - Final submission deadline
