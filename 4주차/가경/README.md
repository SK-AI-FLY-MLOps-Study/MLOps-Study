1. 하이퍼 파라미터 옵티마이제이션
    
    HPO - 반복업무이미로 자동화의 여지가 굉장히 많음
    
    - 어떤 하이퍼 파라미터가 가장 중요한지?
    - 하이퍼 파라미터를 예쁘게 분석하고 싶은 경우
        - W&B Sweeps
            
            layer 수에 따른 파라
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/1af494b8-6967-4c98-9eea-2224c7b7170c/Untitled.png)
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/15538c85-0743-40fd-8525-a91b5d3d5250/Untitled.png)
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/b28b610d-8777-482e-94cc-f99a7c41f2b9/Untitled.png)
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ab0a0a9f-d324-4fa3-b226-acd087d096ac/c1902ccd-b457-4d53-928a-bf95cd256890/Untitled.png)
            
            그리드 서치하는 기록을 차트로 남겨준다.
            
            그리드 서치로 파라미터의 변화에 따른 최적의 조합을 찾을 수 있다.
            
2. 리서치 코드 품질 관리 자동화
    
    리서치 코드의 품질 문제가 심각함 - 코드 중복, 재연 불가, 코드 악취가 많음
    
    라이브러리 구현을 통한 추상화를 통해 코드 재사용성 높이기,
    
    너무 많은 전역 변수 없애기 - 함수를 통해 파라미터 받아오기로 변경
    
    코드 길이 줄이기
    
    import가 너무 꼬여있음 - absolute import 를 사용하자
    
    명확한 변수명 기재하기
    
3. 린트와 유닛 테스트
4. 지속적 통합
    
    지속적으로 퀄리티 컨트롤을 적용하는 프로세스를 실행하는 것 (CI)
    
    Git Action
    
    black - 자동으로 린트해주는 툴
    
    액션을 통해 PR을 보내는 경우 자동으로 린트 코드 베이스를 실행함
    
    setting에서 린트 코드 베이스를 통과해야지 머지가 되도록 설정할 수 있음
    
    코드 클라이메이트 - 코드에 대한 정적 분석 제공, 깃헙에 연동하여 코드에 리뷰를 달아주고 머지를 막아줌
    

데이터 검증

TFDV TensorFlow Data Validation

- 머신러닝 시스템에서 데이터로 인한 오류는 찾아내기 어려움
- 데이터세트에서 이상한 점을 찾는 것 - 데이터 검증
- 스키마 추론- 데이터에 대한 스키마 출력

데이터 드리프트 및 스큐

- 실제 데이터의 변화에 따라 모델의 오류가 커지는 현상
