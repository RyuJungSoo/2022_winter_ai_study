2022_winter_ai_study
===============================
[스마클 겨울방학 딥러닝 스터디 리포지토리](https://github.com/sejongsmarcle/2022_Winter_AiStudy)            
교재: [모두의 딥러닝(길벗)](https://thebook.io/080228/)                        
[교재 github](https://github.com/taehojo/deeplearning-for-everyone-2nd)                    
[matplotlib 참고 사이트](https://wikidocs.net/4763)

선형 회귀
--------------------------------------------
종속 변수 y와 한 개 이상의 독립 변수 X와의 선형 상관 관계를 모델링하는 것 - [선형 회귀](https://github.com/RyuJungSoo/2022_winter_aistudy/tree/main/3%EC%9E%A5%20%EC%84%A0%ED%98%95%ED%9A%8C%EA%B7%80)         
                                
선 긋는 법 - 최소 제곱법, 평균 제곱 오차                  

경사 하강법
------------------------------------------------
미분 기울기를 이용하여 오차를 줄여나가는 방법 - [경사 하강법](https://github.com/RyuJungSoo/2022_winter_aistudy/tree/main/4%EC%9E%A5%20%EA%B2%BD%EC%82%AC%20%ED%95%98%EA%B0%95%EB%B2%95)

로지스틱 회귀
-------------------------------------------------
예, 아니오 처럼 이진 분류(Binary Classification) 문제를 해결할 때 사용하는 방법 - [로지스틱 회귀](https://github.com/RyuJungSoo/2022_winter_aistudy/tree/main/5%EC%9E%A5%20%EB%A1%9C%EC%A7%80%EC%8A%A4%ED%8B%B1%20%ED%9A%8C%EA%B7%80)
                              
세 개 이상의 선택지 중 하나를 고르는 문제(다중 클래스 분류)를 해결할 때 사용하는 방법 - [소프트맥스](https://github.com/RyuJungSoo/2022_winter_ai_study/tree/main/10%EC%9E%A5~12%EC%9E%A5%20%EB%AA%A8%EB%8D%B8%EC%84%A4%EA%B3%84%EC%99%80%20%ED%92%88%EC%A2%85%EC%98%88%EC%B8%A1)

퍼셉트론
--------------------------------------------------
입력 값과 활성화 함수를 사용해 출력 값을 다음으로 넘기는 가장 작은 신경망 단위 -[퍼셉트론](https://github.com/RyuJungSoo/2022_winter_ai_study/tree/main/6~9%EC%9E%A5%20%ED%8D%BC%EC%85%89%ED%8A%B8%EB%A1%A0%EA%B3%BC%20%EC%97%AD%EC%A0%84%ED%8C%8C)               

가중치(w) - 기울기 a              
바이어스(b) - y 절편                
가중함 - 입력값과 가중치의 곱을 모두 더한 다음 거기에 바이어스를 더한 값               
활성화 함수 - 0과 1을 판단하는 함수              
                    
XOR문제는 다층 퍼셉트론으로 해결               
단일 퍼셉트론에 은닉층을 추가하면 다층 퍼셉트론을 설계할 수 있음

오차 역전파 및 고급 경사 하강법
----------------------------------------------------
다층 퍼셉트론에서 출력층으로부터 하나씩 앞으로 되돌아가며 각 층의 가중치를 수정하는 방법이다. 하지만 층이 늘어나면서 역전파를 통해 전달되는 기울기의 값이 점점 작아져 맨 처음 층까지 전달되지 않는 기울기 소실 문제가 발생 -> 고급 경사 하강법, 모덴텀 등 고급 경사 하강법이 필요하게 됨 - [오차 역전파 및 고급 경사 하강법](https://github.com/RyuJungSoo/2022_winter_ai_study/tree/main/6~9%EC%9E%A5%20%ED%8D%BC%EC%85%89%ED%8A%B8%EB%A1%A0%EA%B3%BC%20%EC%97%AD%EC%A0%84%ED%8C%8C)          

교차 엔트로피 (오차 함수의 한 종류)
-----------------------------------------------------
교차 엔트로피 계열의 함수는 출력 값에 로그를 취해서, 오차가 커지면 수렴 속도가 빨라지고 오차가 작아지면 수렴 속도가 감소하게끔 만든 것               
binary_crossentropy(이항 교차 엔트로피) - 이항 분류 형식일 때 사용              
categorical_crossentropy(범주형 교차 엔트로피) - 다중 분류 형식일 때 사용                

원-핫 인코딩(one-hot-encoding)
------------------------------------------------------
데이터에 문자열이 있는 경우 이를 숫자 형태로 변환시켜주는 것이 편하다. 여러 개의 Y 값을 0과 1로만 이루어진 형태로 바꿔 주는 기법을 원-핫 인코딩이라고 한다. - [원-핫 인코딩](https://github.com/RyuJungSoo/2022_winter_ai_study/tree/main/10%EC%9E%A5~12%EC%9E%A5%20%EB%AA%A8%EB%8D%B8%EC%84%A4%EA%B3%84%EC%99%80%20%ED%92%88%EC%A2%85%EC%98%88%EC%B8%A1)           

소프트맥스(softmax)
------------------------------------------------------------
총합이 1인 형태로 바꿔서 계산해 주는 함수 - [소프트맥스](https://github.com/RyuJungSoo/2022_winter_ai_study/tree/main/10%EC%9E%A5~12%EC%9E%A5%20%EB%AA%A8%EB%8D%B8%EC%84%A4%EA%B3%84%EC%99%80%20%ED%92%88%EC%A2%85%EC%98%88%EC%B8%A1)    
합계가 1인 형태로 변환하면 큰 값이 두드러지게 나타나고 작은 값은 더 작아진다.                   
