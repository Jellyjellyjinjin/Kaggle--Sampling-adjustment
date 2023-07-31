# Kaggle-Santander_classification
주제 : 고객이 은행 업무 경험에 만족하는지 여부를 예측

대회기간: 만료 

평가방식: ROC curve
#

이진데이터의 불균현으로 인해 여러 샘플링 기법을 실험

이진분류 모델에서의 샘플링 기법에 대한 논문을 찾아본 결과 randomsampling 방식보다 근접클래스들을 제거하거나 증폭시키는 알고리즘 방식의 기법이 성능이 좋았다.

언더 샘플링 기법 Tomek link ,오버샘플링 기법인 SMOTE,  둘을 결합한 SMOTETomek , 그리고 하이퍼파라미터 scale_pos_weight로 조정해보았다. 

결과 : 0.50051 -> 0.70049
