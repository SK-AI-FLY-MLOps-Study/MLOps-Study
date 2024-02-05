스큐의 종류

스키마 스큐

특성 스큐

분포 스큐

→ TFDV로 확인 가능하다

## WIT what if tool

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/d383123f-94c1-4c4a-b6ba-e322fdf66eac/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/4c8c901d-6985-482c-868a-8159622ded02/Untitled.png)

datapoint editor

performance - Threshhold 구간

Feature 

- 실습
    
    데이터 시각화 분석 제공
    
    데이터 포인터를 통해 가장 가까운 Counterfactuals 탐색 가능
    
    부분 종속성 플록 탐색
    
    부분 의존도 확인
    
    모델 성능 분석
    
    Cost ratio 설정을 통한 Threshold값 제공
    

# 도커 소개

도커 개요

가상화 환경의 기초

어플리케이션을 인프라에서 분리할 수 있음 코드 작성과 프로덕션 사이의 실행 지연을 줄일 수 있음

컨테이너라고 하는 느긋하게 격리된 환경에서 앱을 패키징라고 실행할 수 있음 격리 및 보안을 통해 주어진 호스트에서 여러 컨테이너들을 동시에 실행할 수 있음

컨테이너는 가볍고 현재 호스트에 설치된 항목에 의존할 필요가 없음 컨테이너를 쉽게 동유할 수 있으면 공유하는 사람이 동일한 방식으로 작동하는 동일한 컨테이너를 갖게 됨 - 도커 레지스트리

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/fc9b2b5a-d4b9-4b9d-bd6d-4d55f119c223/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/8020c9e1-4f85-4da0-8d1b-3051adeec425/Untitled.png)

레지스트리 - 도커허브

## Docker 데몬

도커api 요청을 수신하고 이미지, 컨테이너, 네트워크 및 볼륨과 같은 도커 객체 관리

다른 데몬과 통신하여 도커 서비스를 관리할 수도 있음

## Docker 클라이언트

사용자가 도커와 상호작용하는 기본 방법

docker run과 같은 명령을 사용하면 클라이언트가 이 명령을 데몬에 전송하여 실행함

이 도커 명령은 도커 aPI를 사용함

도커 클라이언트는 둘 이상의 데몬과 통신할 수 잇다

## Docker 레지스트리

도터 이미지를 저장함 

도커 허브는 누구나 사용할 수 있는 공용 레지스트리

기본적으로 도커 허브에서 이미지를 찾도록 구성됨

자신의 개인 레지스트리를 실행할 수 있음

docker pull docker run 명령을 사용하면 구성된 레지스트리에서 필수 이미지를 가져옴

docker push 명령을 사용하면 이미지가 구성된 레지스트리로 푸시됨

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/812c9a1d-cdc4-418b-ae12-a77980895ee8/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/fedfb6d2-cec8-442f-a60a-d564fdc29db2/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/b94db266-6093-4291-ba95-d0b12a107874/Untitled.png)

도커 런 → 이미지가 인스턴스에서 실행되는 것

# 쿠버네티스

서버에 대한 스케일링하고 스케일 아웃하는 방식이 어려웠음

수평적 오토스케일링

- 실습
    
    쿠버네티스 설치
    
    kubectl 설치
    
    쿠버네티스 대시보드
    
    쿠버네티스 앱배포 실습
    
    로컬 호스트- 8200포트에 포트포워딩
    
    //왜 모든 실습은 파일 복붙으로 이루어진걸까~~~~~
    

## 쿠베플로우

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/beff2335-d7c0-48a0-b9fe-6ad3b36160e8/Untitled.png)

1. Composability 조합가능성
    
    머신러닝 실무자들에게 익숙한 데이터 사이언스 도구를 사용함
    
    기계학습의 특정 단계를 용이하게 하기 위해 독립적으로 사용되거나, end2end 파이프라인을 형성하기 위해 함께 구성될 수 있음
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/6b27853c-18e6-42f8-9d92-fa04f339b727/Untitled.png)
    
2. Portablility
    
    컨테이너 기반 설계를 갖추고 쿠버네티스 및 클라우드 네이티브 아키텍처를 활용함으로써 쿠베틀로우는 특정 개발환경에 종속될 필요가 없음
    
    랩톱에서 실험 및 프로토타입 작업을 수행할 수 있으며, 프로덕션 환경에 손쉰게 배포할 수 있음
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/4f0e92a0-31d3-4423-8f46-5cb2c46cbac8/Untitled.png)
    
3. Scalability
    
    기본 컨테이너와 기계의 수와 크기를 변경하여 클러스터의 요구에 따라 동적으로 확장할 수 있음
    
    ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/5a68ef86-12f3-4c03-a051-4c6fb1d3253e/Untitled.png)
    

대부분의 ml 툴/플랫폼에서 사용 가능

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/f13a7fb2-7913-46b0-9bb3-04fb3da9aac1/Untitled.png)

기본 개념

주요 인터페이스 - central dashboard

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/f9f932d0-e9c6-461f-a751-e25b597264d3/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/eb2d8bae-096b-4edc-8847-60614aad4cd3/Untitled.png)

데코레이터 - 이미지 - 컴포넌트 - 파이프라인 - yaml
