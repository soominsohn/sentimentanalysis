# Sentiment Analysis of new-media users after COVID-19 by using NLP  
#### 이화여자대학교 캡스톤디자인프로젝트B 연구트랙 그로쓰21팀 고독한 늑대 둘  
##### Participants: Soomin Sohn, Jung-A Hong  
<!-- 
더 많은 데이터는 아래 드라이브에서 확인 하실 수 있습니다.  
https://drive.google.com/drive/folders/17b7uciVGuPWjWvVdbPIvNN_j8rVDVOi_?usp=sharing   -->

## Project background  
### Problem  
1. 코로나의 발발  
코로나19는 중국의 수산물 시장에서 2019년 발현하여 2020년 1월 우리나라를 비롯해 일본, 태국 등 아시아 지역으로 확산되었고 전 세계에 퍼져 많은 사람들의 삶을 바꾸었다. 코로나19가 전세계적으로 확산됨에 따라 세계 보건 기구(World Health Organization) 2020년 1월 30일 국제적 공중보건 비상사태를 선포했으며 3월 11일에는 감염병의 가장 위험한 단계인 팬데믹을 선언했다.  

2. 코로나의 확산  
코로나의 경우 선형으로 확진자 증가세를 보이는 것이 아닌 다소 시차를 두고 확산세를 보였다. 특히 미국 등 아메리카 지역과 유럽 지역은 작년 9월 부터 12월 간 가파른 상승세를 보였으나 백신 접종이 시작됨에 따라 2021년 초 감소세가 두드러졌다. 그에 비해 아시아 지역은 작년 9월 부터 감소세에 들었다 올해 2월 부터 가파른 증가세를 보이고 있는 것을 볼 수 있다. 코로나로 인해 2021년 4월 6일 기준 총 1억 3천 여명이 감염되었고, 이 중 280만 명의 사람이 목숨을 잃었다.  
자료 출처 : World Health Organization Corona virus dashboard  

3. 코로나가 집단의 정신 건강에 미치는 영향  
오랜 기간 동안의 재난의 경험은 개인과 사회에 다양한 측면으로 부정적인 영향을 줄 뿐만아니라 재난이 종료된 후에도 후유증과 같은 효과를 불러일으킨다. 표에서 나온 바와 같이 1년 남짓의 시간 동안 국민들이 단합하는 허니문 시기가 존재하지만, 일정 시간이 지나면 지속된 통제에서 비롯된 심리적 탈진과 같은 문제가 두드러진다. 그리고 현실적인 문제가 범사회적으로 다가오면서 개개인의 스트레스 또한 걷잡을 수 없이 커지게 된다. 코로나 19 감염에 대한 일반 대중의 두려움과 심리, 우울 불안에 미치는 영향을 조사한 논문에서는 코로나로 인한 불안과 우울경험이 각각 48.8%, 29.7% 로 나온 것 토대로 보면, 코로나로 인한 정신건강의 적신호는 개개인의 문제가 아닌 사회적인 문제로 보아야 적절할 것이다.  
자료 출처: https://www.youtube.com/watch?v=w0A2C_JI7SI

4. 코로나 시기 뉴미디어의 선두로 선 유튜브  
 코로나19의 걷잡을 수 없는 확산으로 인해 사람들은 다른 사람과의 물리적 만남을 갖는 횟수가 현저히 적어졌다. 수업은 물론이고 국내외 여행, 사람들과의 모임은 권장되지 않으며 모든 사회가 비대면으로 탈바꿈 되고 있다. 전세계 적인 락다운 정책은 사람들이 가장 기본적으로 가지고 있는 인간으로서의 특성인 "관계 맺기"를 금지하고 있는 것과 마찬가지이다. 이로 인해 자연히 사람들은 사람과 사람사이의 소통의 결핍과 활동 반경의 제약으로 인해 정서적인 괴로움을 겪게 됐다. 이러한 괴로움의 탈출구로 사람들은 온라인 상에서 관계를 맺을 수 있는 소셜 미디어에 유례없는 관심을 갖게 되었다. Bazaarvoice 가 4,500 명을 대상으로 한 설문조사에서는(https://www.digitalcommerce360.com/2020/09/16/covid-19-is-changing-how-why-and-how-much-were-using-social-media/) 판데믹 상황에서 72% 의 사람들이 소셜 미디어를 더 많이 사용하고, 43% 사람들은 더 많이 게시물을 게시하는 것이 밝혀졌다. 또한 인스타그램, 틱톡, 유튜브가 가장 선호하는 플랫폼임이 나타났다. 또 달라진 것은 과거 소셜 미디어는 온라인 상에서 친구와 관계를 맺고 자신의 일상을 공유하는 것이 주를 이뤘다면 팬데믹 상황에서는 컨텐츠를 소비하는 경향이 두드러졌다는 것이다.  
  
5. 유튜브와 코로나의 상관 관계  
그 중에서도 유튜브는 사용자가 업로더와 뷰어로 나뉘고 대다수의 사람이 뷰어로써 컨텐츠를 소비하는 경향이 두드러지는 소셜미디어이다. 본 연구에서는 많은 사람들이 컨텐츠를 소비하는 유튜브의 텍스트 분석을 통해 코로나 시국의 감성 변화 양상을 효과적으로 관측할 수 있을 것이라 가정하는 바이다. 본 연구에서는 컨텐츠 자체의 감성 변화와 컨텐츠에 반응하는 뷰어의 감성 변화를 자연어 처리 기법을 통해 결과를 도출하고 이를 시각화 할 것이다.  

## Solution  
### Method  
본 연구는 세단계의 실험을 진행하였으며 각 단계에서 사용한 기술과 API및 자료는 다음과 같다.  
#### 1). 데이터 수집 단계  
동영상 리스트, 댓글 데이터 추출 -> Youtube Data API version3  
자막 데이터 추출 -> youtube transcript API  
#### 2). 데이터 전처리 단계:  
HTML태그 제거 ->Beautiful Soup  
非알파벳 제거, 알파벳 소문자화, 불용어 제거  
#### 3). 데이터 분석 단계: 
긍/부정 분석 -> TextBlob API  
감정단어 빈도 분석(Emotion 분석) -> NRC Emotion Lexicon  
분석 데이터 병합 -> Python pandas library  
분석 결과 시각화 -> Python matplot library Barchart  

### Analysis Target  
<!-- ![image](https://user-images.githubusercontent.com/83059234/135257802-fc66a482-a38c-4162-93bc-780a25488965.png) -->
<img src="https://user-images.githubusercontent.com/83059234/135257802-fc66a482-a38c-4162-93bc-780a25488965.png" width="600"/>  


### Analysis Results  
#### 1). 데이터 수집 단계  
<!-- ![image](https://user-images.githubusercontent.com/83059234/135255514-bf125139-d35a-4064-82a1-77bf18754efa.png)  -->
<img src="https://user-images.githubusercontent.com/83059234/135255514-bf125139-d35a-4064-82a1-77bf18754efa.png" width="800"/>  


#### 2). 텍스트 데이터 전처리:  
<!-- ![image](https://user-images.githubusercontent.com/83059234/135255622-9579d375-99fa-44ff-a74b-399f1443dff7.png)   -->
<img src="https://user-images.githubusercontent.com/83059234/135255622-9579d375-99fa-44ff-a74b-399f1443dff7.png" width="600"/>  


#### 3). 데이터 분석 단계:  
##### 3-1) 긍/부정 분석:  
<img src="https://user-images.githubusercontent.com/83059234/135257255-da7b5a71-4e3e-427d-9d33-ff532f6f2a5a.png" width="350"/>  
<!-- ![image](https://user-images.githubusercontent.com/83059234/135257098-09dc1839-4ff9-4888-be99-45c863d7094a.png) -->


##### 3-2) 감정단어 빈도 분석(Emotion 분석):  
<img src="https://user-images.githubusercontent.com/83059234/135257207-e29fed9b-7899-4e4b-b8e1-1a94d1d959f8.png" width="350"/>   
<!-- ![image](https://user-images.githubusercontent.com/83059234/135257207-e29fed9b-7899-4e4b-b8e1-1a94d1d959f8.png) -->


##### 3-3) 분석 결과 시각화:  
<img src="https://user-images.githubusercontent.com/83059234/135257948-64b41d2c-932b-417e-952d-5c286a79fd9a.png" width="600"/>   
<!-- ![image](https://user-images.githubusercontent.com/83059234/135257948-64b41d2c-932b-417e-952d-5c286a79fd9a.png) -->




## Codes
1. 데이터 수집  
1-1). 동영상 리스트 수집: codes/1. extractVideoList.ipynb  
1-2). 자막과 댓글 데이터 추출: codes/2. extractCaptionandComment.ipynb  

2. 데이터 전처리와 분석
2-1). 자막데이터 전처리와 긍/부정분석, emotion 분석: codes/3-1. sentiment and emotion analysis_caption.ipynb
2-3). 댓글데이터 전처리와 긍/부정분석, emotion 분석: codes/3-2. sentiment and emotion analysis_comment.ipynb  

3. 결과 분석  
3-1). 자막, 댓글 데이터 분석 결과 병합: codes/3-3. merge sentiment and emotion analysis result.ipynb  
3-2). 3-1의 분석결과 병합 데이터에 대하여 시각화: codes/4. visualize the results.ipynb  
3-3). 분석에 사용한 데이터 양 통계: codes/5. statistics.ipynb

## Results  
1. youtuberdatum
유튜버의 동영상아이디, 추출한 자막, 댓글 데이터 모음  

2. analysis_result  
긍/부정 분석 결과와 emotion 분석 결과에 대한 통계파일, 이미지 파일 모음.

## 기대효과 및 의의  

1. 판데믹이라는 특수한 상황아래 기존 설문조사만으로 진행되었던 집단 정서 연구가 빅데이터로써 확인 될 수 있음을 증명했다. 이를 통해 동시 다발적으로 생성되는 대중들의 감성, 피로도를 분석하여 국가 정책 수립 시 하나의 지표로 사용할 수 있을 것으로 기대한다.  

3. 빅데이터 분석을 통한 집단 정서 파악으로 사회적 거리두기와 같은 국가 정책의 방향성을 제안할 수 있다. 
