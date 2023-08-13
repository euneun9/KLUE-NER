# KLUE-NER(한국어 NER 데이터셋에 대한 예측 모델)

## 개요
- 개체명 인식(Named Entity Recognition, NER)
- 토큰 분류 문제
- 제로샷 교차 언어 전이→ 한 언어에서 학습
: 한 언어에서 미세 튜닝된 모델이 추가 훈련 없이 다른 언어에 적용된다는 의미
→ 코드 스위칭 모델에 적합 : 한 대화에서 둘 이상의 언어나 사투리를 바꿈
- 제로샷 전이
    
    한 레이블 집합에서 모델 훈련 후 다른 레이블 집합에서 평가하는 작업
    
    GPT-3 등에서는 후족작업에 미세튜닝하지 않고 평가하는 상황
  
다중 언어 개체명 인식에 관한 코드 : 
https://github.com/rickiepark/nlp-with-transformers/blob/main/04_multilingual-ner.ipynb

------
## 코드 내용
다중 언어 개체명 인식에 관한 코드를 한국어 NER 데이터셋에 대한 예측 모델로 수정
dataset: klue
model: skt/kogpt2-base-v2
