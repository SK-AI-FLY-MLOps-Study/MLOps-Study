# Kubeflow
01. 쿠베플로우 개요
02. 쿠베플로우의 기본 개념
03. 쿠베플로우 설치

필요한 이유
MLcode는 전체의 5%밖에 안됌
다양한 파이프라인을 관리해야함
그걸 추정하고 재사용성 높게끔 만들어놓은 오픈 소스가 kubeflow(kubernetes+flow)

1. 조합가능성  
2. 이식성  
3. 확장성

kubeflow를 사용하면 대규모 학습과 대규모 모델 관리가 가능해짐  
![image](https://github.com/SK-AI-FLY-MLOps-Study/MLOps-Study/assets/108683454/34e21c61-47c3-4024-bf5f-91a2b947e3ab)
kubernetes위에서 동작함 근데 로컬, 클라우드 다른 곳에서도 많이 동작을 함  
머신러닝툴은 원하는대로 쓸 수 있음  
센트럴 대시보드라는 것이 있음 종합적인 상황, 결과를 확인할 수 있는 이쁜  UI  

![image](https://github.com/SK-AI-FLY-MLOps-Study/MLOps-Study/assets/108683454/42212eb2-7af2-4cab-ab05-3b834f7cdaee)
컴포넌트간 통신을 Mini0을 사용하여 함 Job으로 등록하면 알아서 학습을 함  
kubeflow는 airflow랑 유사 
도커라이즈 되서 이미지가 되어서컨테니제이션 필요  
kfserving으로 서빙하고
TF.jobs로 학습  
