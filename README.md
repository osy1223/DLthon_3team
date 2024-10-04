# DLthon_3team

### **1. 문제 정의**

***

대화의 성격을 **위협 세부 클래스 4개 또는 일반 대화** 중 하나로 예측하는 과제

- **_학습 데이터_**_는 '협박', '갈취', '직장 내 괴롭힘', '기타 괴롭힘' 등 4개 클래스 각 약 1천 개로 구성_

- **_테스트 데이터_**_는 '협_박', '갈취', '직장 내 괴롭힘', '기타 괴롭힘', '일반 대화' 등 5개 클래스 각 1백여 개로 구성

  - train data에는 없지만, test data는 일반 대화 클래스가 존재합니다. 5개 문장을 분류할 수 있게 train data에 일반 대화 데이터셋을 추가합니다.

    - 일반대화는 **합성데이터**로 구성합니다. 다양한 프롬프트로 문장을 생성하고, 이를 학습에 활용합니다.

    - \*\*\[일반대화 클래스]\*\*를 제외한 데이터의 추가나 외부 데이터 사용 불가(단, Augmentation은 가능)

    - Pre-trained model은 공개된 모델에 한하여 사용 가능(재현성을 위함)

  - 학습 결과를 확인하며 어떤 일반 대화 데이터셋이 성능을 높이는데 도움을 주는지 비교/기록합니다.

  - 실험 결과를 Ablation study형식으로 기록합니다


### **2. Dataset**

***

- Dataset은 lms에 업로드되어 있습니다. 구성은 다음과 같습니다.

  - Train data는 index, class, conversation등 3개의 컬럼으로 구성

  - Test data는 **index와 conversation만 제공**


### **3. 평가지표 = f1-score**

### **4. 대회 RULE**

***

1. 일반대화를 제외한 데이터 추가 금지(augmentation은 가능)

2. DKTC의 일상대화 데이터셋은 AIHUB 등 이용해서 확보

3. 발표일 역할 분담 내용, 실험 내용, 프로젝트 진행 과정, 시각화 등 발표자료를 만들어 발표 진행

4. Rubrics:

   1. 데이터 EDA와 데이터 전처리가 적절하게 이뤄졌는가?

   2. Task에 알맞게 적절한 모델을 찾아보고 선정했는가?

   3. 성능향상을 위해 논리적으로 접근했는가?

   4. 결과 도출을 위해 여러가지 시도를 진행했는가?

   5. 도출된 결론에 충분한 설득력이 있는가?

   6. 적절한 metric을 설정하고 그 사용 근거 및 결과를 분석하였는가?

   7. 발표가 매끄럽게 진행되었고 발표시간을 준수하였는지?
