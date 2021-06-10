---
title:  "1. 데이터 분석의 단계별 목적 이해하기 (분석 싸이클 이해)"
toc: true
toc_sticky: true

categories:
  - time_Series
---
## 데이터 싸이언티스트?/애널리스트?/엔지니어?/비즈니스고객? 관점에서:
1. **데이터수집**: 소스별 데이터 추출 및 저장(Loading)
2. **데이터전처리**: 기초통계(Descriptive Statistics) + 붙이기(Curation) + 없애기(Remove) + 채우기(Fill) + 필터(Filter) + 변경하기(Transform)
3. **데이터정리**: 데이터한곳에담기(Data Warehouse) + 바꾸기및정리(Data Mart) + 분리(Data Split)
4. **데이터분석**: 기초통계(Descriptive Statistics) + 모델링(Algorithm) + 검증(Evaluation) + 에러분석(Error Analysis)
5. **결과정리**: 시각화(Visualization/Dashboard) + 의사결정(Decision Support) + 지식화(Knowledge) + 공유(Reporting)

![AnalysisCycle1](/assets/AnalysisCycle1.png)

![AnalysisCycle2](/assets/AnalysisCycle2.png)

![AnalysisCycle3](/assets/AnalysisCycle3.png)

## 데이터분석 현실 관점에서:

![Analysis_Real1](/assets/Analysis_Real1.PNG)

![Analysis_Real2](/assets/Analysis_Real2.PNG)

-----
- **데이터분석 현실요약:**
> **"데이터분석 설계(1단계)"는 "모델링(2단계)"보다 훨씬 중요합니다. 그리고 "분석종료(3단계)"는 또다른 새로운 시작입니다**
> - **예시1)** “퇴사할 사람을 찾아주세요”  vs  “입사할 사람을 찾아주세요“
> - **예시2)** “삼성전자 주식을 사야 할까요 말아야 할까요?”  vs  “내일 삼성전자 주식은 얼마일까요?"

![Analysis_Process](/assets/Analysis_Process.png)

-----

- **요구사항(질문) 예시:**
> - "아이폰 고객은 왜 갤럭시 고객보다 충성도가 높은지 분석해봐~" 라고 질문을 다 듣기도/이해하기도/생각하기도 전에 프로젝트가 시작됩니다
> - "AI를 활용해서 생산공정의 이상을 조기 탐지하고 비용을 줄여봐~" 라고 질문을 다 듣기도/이해하기도/생각하기도 전에 프로젝트가 시작됩니다
> - "타겟 마케팅을 하기위해 누구한테 프로모션을 해야하는지 알려줘봐~" 라고 질문을 다 듣기도/이해하기도/생각하기도 전에 프로젝트가 시작됩니다

0. **문제정의**: 무엇을 분석할지 정한다
    > 무엇을 분석할지 각자 생각이 모두 다르다(솔직히 아무도 모른다)  
    > 무엇을 분석할지 모르지만 일단 도구(R? Python? 플랫폼? 아마존? 외주?)부터 마련한다  
    > 무엇을 분석할지 모르지만 완료일정과 계획이 준비가 되어있다  
    > 어쨌건 있다고 생각하고 시작한다  
    > (데이터분석 프로젝트는 이미 착수했다고 보고가 되었다)  

1. **데이터수집**: ~~소스별 데이터 추출 및 저장(Loading)~~
    > 데이터 PC에 있는줄 알았는데 A4용지에 있어서 누구 시켜서 파일로 바꾼다    
    > 데이터를 구했는데 빅데이터는 아니고 그냥 엑셀 파일 몇개다  
    > 데이터 파일을 열었더니 다 빈칸이고 딱봐도 오타 투성이다  
    > 근데 이 데이터로 충분한지 아무도 모르지만 어쨌건 (있는줄/충분한줄 알았는데) 시작한다  
    > (빅데이터를 기반으로 한 데이터 수집이 완료가 되었다고 보고가 되었다)  

2. **데이터전처리**: ~~기초통계(Descriptive Statistics) + 붙이기(Curation) + 없애기(Remove) + 채우기(Fill) + 필터(Filter) + 변경하기(Transform)~~
    > 무엇을 분석할지 모르고 데이터는 없지만 전처리에 돌입한다  
    > 일단 이상해 보이는 데이터를 다 지워본다 (남는게 없다..)  
    > 임의로 데이터를 채워본다 (어짜피 아무도 모르니까..)
    > 할게 많을 줄 알았는데 별로 할게 없음을 깨닿는다  
    > (데이터가 무결점으로 잘 준비되어 있다고 보고가 되었다)

3. **데이터정리**: ~~데이터한곳에담기(Data Warehouse) + 바꾸기및정리(Data Mart) + 분리(Data Split)~~
    > (대부분 개인PC로 충분하겠지만) 일단 서버/플랫폼에 데이터를 올린다  
    > (뭔가 중요한걸 해야할것 같은데..) 서버/플랫폼 사양정도 체크해보며 있는다  
    > (데이터 플랫폼에 데이터가 이관되고 곧 분석에 착수할거라고 보고가 되었다)

4. **데이터분석**: ~~기초통계(Descriptive Statistics) + 모델링(Algorithm) + 검증(Evaluation) + 에러분석(Error Analysis)~~
    > 무엇을 분석하고 무슨 데이터를 사용해야 되는지 모르지만 분석을 시작한다  
    > 기초통계는 사람수?클릭수? 등 "횟수(count)"면 충분하다  
    > 도구(R? Python? 플랫폼? 아마존? 외주?) 활용/쪼아서 제일 최신 알고리즘을 적용해보려 살펴본다  
    > (뭔가 안되면..) 우선 1차 회귀분석? 상관관계? 어디서 들어본걸 해서 그림부터 그려본다  
    > (뭔가 중요한 단계인것 같은데..) 더이상 할수 있는게 없음을 깨닿는다  
    > (분석이 완료되어 인싸이트가 곧 쏟아질 것이라고 보고가 되었다)  

5. **결과정리**: ~~시각화(Visualization/Dashboard) + 의사결정(Decision Support) + 지식화(Knowledge) + 공유(Reporting)~~
    > 무엇을 분석하고 무슨 데이터를 사용하고 무슨 결과가 있는진 모르겠지만 결과를 정리한다  
    > (완료일정이 내일이라 퇴사/퇴학이 필요한게 아닌지 잠이 오지 않는다)  
    > (신기한건 모든 단계는 작동/구현되었고 각 단계 개발자들은 성과를 보고한다)  
    > (Kaggle과 데이터분석은 다름을 알게된다)  

## 데이터 싸이언티스트 실무 관점에서:

![Analysis_Cycle](/assets/Analysis_Cycle.png)

0. **문제정의**: 무엇을 분석할지 정한다
    - 문제정의가 없으면 분석은 시작할 필요가 없다  
        > **문제정의에 많은 고민을 해야 한다**  
        > **문제정의에 모든 구성원이 동의할 수 있도록 끊임없이 커뮤니케이션 해야 한다**  
        > **1회성이 문제정의가 아니라 필요시 끊임없이 진화/변경시켜야 한다**  

1. **데이터수집**: 소스별 데이터 추출 및 저장(Loading)
    - 데이터가 없으면 분석은 시작할 필요가 없다
    - 문제 답의 보기후보가 데이터에 없으면 분석을 시작할 필요가 없다(어떤 연령이 TV를 보는지 알고 싶은데 데이터에 연령이 없으면 불가)
        > **알고리즘/기술보다 데이터수집부터 시작하기 위한 작업을 착수해야 한다**
        > **데이터는 많을수록 좋지만 양보다(Row) 질(Column)을 늘려야 분석을 한 의미가 생긴다**
        > **보기가 데이터에 없으면 문제정의부터 새롭게 수정해야 한다**
        > - Loading 목적: 각 소스별로 데이터를 수집함

2. **데이터전처리**: 기초통계(Descriptive Statistics) + 붙이기(Curation) + 없애기(Remove) + 채우기(Fill) + 필터(Filter) + 변경하기(Transform)  
    > - Descriptive Statistics 목적: 하기 4개의 전처리 의사결정을 위한 기준으로 주로 활용
    > - Curation 목적: 각 소스별 데이터를 하나의 Database로 붙임  
    > - Remove & Fill 목적: 데이터 오류를 제거하가나 비어있는 데이터를 채움  
    > - Filter 목적: 분석범위에 관련된 보기(Feature)들만을 추려냄  
    > - Transform 목적: 사람이 이해가 가능한 방식으로 데이터 자체를 변경함  

3. **데이터정리**: 데이터한곳에담기(Data Warehouse) + 바꾸기및정리(Data Mart) + 분리(Data Split)
    - 데이터수집/전처리/정리 까지 전체 업무의 80% 이상을 차지한다
        > **1회성 수집/전저리/정리로 끝나지 않고 끊임없이 업데이트하고 진화시켜야 한다(이는 분석알고리즘이 해주지 않는다)**  
        > - Data Warehouse 목적: 전처리 단계를 거친 1개의 Database를 주로 보관 및 무결점 유지 목적
        > - Data Mart 목적: Warehouse를 변경하지 않고 복사하여 조금 더 목적에 맞게 전처리를 거침
        > - Data Split 목적: 주로 과거(Train Data)와 미래(Test Data)를 구분하여 저장/알고리즘에 활용

4. **데이터분석**: 기초통계(Descriptive Statistics) + 모델링(Algorithm) + 검증(Evaluation) + 에러분석(Error Analysis)  
    - 수학적으론 어려울 수 있지만 수동적으로 대응/활용이 가능하다
    - 알고리즘(또는 기계)은 정해진 검증수단을 따를뿐 우리의 문제에 관심이 없다
        > **각 알고리즘의 사용 목적에 대한 명확한 이해와 결과해석을 집중해서 습득해야 한다**  
        > **어떤 알고리즘 성능 뛰어난지 검증(Evaluation)은 결국 사람이기에 많은 고민을 해야 한다**
        > **알고리즘 적용시작이 중요한게 아니라 언제 끝내야 하는지 고민해야 한다**
        > - Descriptive Statistics 목적: 어떤 분석 알고리즘을 선정할지 또는 Input/Output 형태를 결정하는 기준으로 활용
        > - Algorithm 목적: Input/Output의 형태 또는 분석목적에 따라 정해지는 편
        > - Evaluation 목적: 현 알고리즘 성능 확인 및 다음 업데이트를 위한 기준 설정
        > - Error Analysis 목적: 모든 데이터의 패턴/특징을 알고리즘이 반영하고 있음을 이해하기 위한 기준

5. **결과정리**: 시각화(Visualization/Dashboard) + 의사결정(Decision Support) + 지식화(Knowledge) + 공유(Reporting)
    > **0~4 단계를 무한대로 반복 및 각 단계를 업데이트하며 인싸이트를 뽑아낼 수 있어야 한다**
    > - Visualization/Dashboard/Decision/Knowledge/Reporting 목적: 주로 고객에 맞춘 설명력을 제공하기 위함으로 일반화된 방향은 없음

# 분석을 이해하고 공감하는 자세 및 방향
**"거짓말의 3가지 종류: 거짓말, 새빨간 거짓말, 그리고 통계 (by 마크 트웨인)"**

> - **전혀 이해되지 않는 어려운 수식을 나열하고 분석을 하여 결론을 내버렸는데 아무리 생각해도 내 상식과는 다를 경우가 자주 있다!**  
> - **어떤 데이터를 어떤 방식으로 가공했고, 어떤 방법으로 도출했는지 아이들에게 충분히 가르칠 수 있으나, 전문가라는 사람이 일반 성인들에게 자신의 측정 방식을 제대로 이해시킬 수 없다는건 수상한것이 아닌가?**  
> - **세상 사람들은 뭔가 복잡하고 어려운 과학기법을 썼다고 하면 이상하리만치 맹신하는 경향이 있다**  

## 통계의 한계
- 모집단(Population)의 특성을 통계로 설명하는 것은 굉장히 괜찮은 접근이다
- 표본(Sample)과 모집단(Population)의 특성이 꼭 같을 수는 없고 상당히 위험한 발상이다
    - 표본을 통해 모집단을 추정하려는 방식과 모집단 자체의 특성을 분석하려는 방식 중 무엇이 좋은건지는 누구도 알 수가 없다
- 하나의 표본으로 모집단의 평균을 정확히 알 수는 없지만 추측은 가능하다
    - 빅데이터라 하여도 데이터 분석이 필요한 이유는 빅데이터도 결국 표본일 가능성이 높기 때문이다
- 통계는 결국 표본의 통계 특성을 통해 모집단의 통계 특성을 "추측"하는 것이다
    - 추측이기에 장담할 수 없고 확률이론을 가져와 얼추 95% 정도 맞을 가능성으로 추정을 하지만 5%의 틀렸을 가능성은 반드시 존재한다
    - 내가 올바른 추정을 했다 하더라도 95%의 신뢰구간이 너무 커서 별로 쓸모가 없을 수도 있다
- 통계의 큰 함정: 만약 Sample을 추출하는 과정이 틀렸으면 중심극한정리(Central Limit Theorem)는 동작하지 않는다
    - 이상적인 Sample 추출은 거의 불가능하다
- Sample이 왜곡되어 있으면 통계분석 결과는 과학적으로 유의미하지 않을 수 있다
    - 현실은 의도적인 편향된 Sample로 인한 결과물들을 믿으며 자주 접하고 살고 있다는 것이다
- 모집단이 시간에 따라 변화한다면, 과거에 추출한 샘플은 현재를 설명하지 못한다
    - 시간의 흐름에 따른 모집단의 변화를 추정하면 좋겠지만.. 이건 불가능이다
    - 현실은 분석결과를 과거/현재/미래에도 그럴거라고 믿음으로 살고 있다는 것이다(단지 과거 결과일 뿐이다)
- 많은 전문가들이 통계의 한계를 전문적인 이유로 설명하지 못하더라도 본능적으로 왜곡될 수 있음을 인지하고 있다
    - 일반인들이 통계정보를 믿기 힘든 것은 어쩌면 당연한 일이다


## 통계의 강점
- 통계는 대규모 조사의 어려움을 획기적으로 줄일 수 있다
- 통계는 다소 개인차가 있는 어떤 집단에 대해서도 공통적인 특징을 추출할 수 있다
    - 일반인/환자들의 약물 효능이 통계적으로 유의미한지 비교를 통해 인간에게 통상적으로 미치는 특성을 해석할 수 있다
- 통계적 추정을 하는데 말고 다른 방법으로 활용이 가능하다
    - 내일의 주식 가격 예측은 불가능하지만 통계를 통해 주가의 적정 범위를 추정하는 것은 가능하다(주식에 어떤 변화가 발생하지 않을 경우)
    - 시장의 변화나 사고 발생에 빠르게 대응이 가능하도록 유인으로 활용할 수 있다


## 통계를 올바르게 사용하는 방법

**"분석은 잘못쓰면 새빨간 거짓말, 잘쓰면 누구도 알 수 없는 강력한 무기"**   
**"거짓말에서 출발한 스스로의 무결점 입증과정"**

- **모집단의 편향:** 타인으로부터 어떤 모집단의 표본을 받았을 때, 그 타인의 이해관계를 살펴야 한다
    - 경제인연합회에서 제공하는 불법시위 데이터와 민주노총에서 제공하는 불법시위 데이터는 다른 결과를 유발할 수 있다
    - 전혀 이해관계가 없는 집단에서 추출한 데이터를 활용하거나 누구도 믿을 수 없다면 직접 추출해야 한다
- **샘플의 편향:** 아무리 공정하게 추출하려고 해도 편향이 없을 수 없음을 인지해야 한다
    - 똑같은 설문지에 똑같은 질문을 하더라도 고령 남성이 질문할 때와 젋은 여성이 질문할 때 답이 다를 수 있다
    - 질문지가 특정 답변을 유도하도록 설계되었다면, 그로 인해 수집된 데이터는 신뢰하기 어렵다
    - 아이스크림을 좋아하는지 질문도 여름이냐 겨울이냐에 따라 결과는 달라진다
- **수집오류의 편향:** 사람의 심리가 배제되는 조사 방식이라도 편향이 생길 수 있다
    - 카지노 룰렛 머신의 빨간공과 검은공의 반지름이 미미하게 다를수도 있다
    - 모든 공이 똑같아도 기계의 재질이나 미끄러움은 일정하지 않을 수 있다
    - 공도 기계도 문제가 없더라도 룰렛근처 콧김 하나라도 결과를 바꿀 수 있다
    - 카지노가 있는 지역에 수맥이 있어 미세하게 자기장의 편향으로 결과가 바뀔 수 있다
    - 편향 제거는 불가능에 가깝지만 편향 정도를 측정하고 이해하고 억제하는 기술은 통계에서 중요한 방향 중 하나이다
- **필연성 증명 불가:** 통계적 분석 결과는 아무것도 장담하지 않는다
    - 분석 결과는 높아봐야 95% 또는 99%의 신뢰성을 가질뿐 절대 100%에 도달할 수 없다
    - 99%라고 해도 이는 모든 가정들이 옳았고, 그래서 CLT가 제대로 작동했다는 가정을 전재로 한다(가정이 틀렸다면?..)
    - 글로벌 금융기관들은 99.9% 위험대 대비하도록 정책법을 적용하고 있음에도 리먼 브라더스 파산은 일어났다
    - 이는 0.1%의 사건이 벌어진거라고 할 수 있을까? 대부분 전문가들은 100% 일어날 필연적 사건이라고 한다
    - 두 집단의 관계가 유의미하더라도, 우연히 맞아떨어진 것 이거나 실제로 아무 상관이 없을 수도 있다
- **기술 보다 객관적 근거들을 늘려가는 과정:** 올바른 통계분석 및 활용은 통계에만 의존하지 않는 자세다
    - 분석의 바람직한 순서는 우선 어떤 현상을 잘 관찰/인지하고 잘 생각해서 어떤 결론을 도출하는 것이다
    - 그 후 통계를 활용하여 이 결론을 증명하려는 것이다
        - 반대로 통계분석으로 어떤 현상(또는 인싸이트)을 우연히 발현한 후 왜 그런지 결론을 지을 수도 있다
        - 이는 통계가 필연성을 증명하지 못하다 보니 근거부족 문제에서 벗어나기가 어렵다
    - 더욱 다양한 형태의 통계분석으로 근거를 보강하고 통계가 아닌 다른 기법들로도 지속적으로 근거를 보강해야 한다
    - 통계의 장점/한계를 인지하고 통계가 필연성을 증명하지 못한다는 사실을 반드시 명심하는 것이다

## 데이터싸이언티스트 스킬셋 3종

> **1) 데이터분석 관련지식(이론)**  
> **2) 프로그래밍 활용능력(실습)**  
> **3) 설득 및 설명능력(현실)**  

**1) 데이터분석 관련지식(이론)**  
> **순수 인문학 또는 예술과 관련된 학문이 아니면 대부분 "수학"과 "컴퓨터"는 모든 학문에서 적극 활용되는 도구**
> - 수학
> - 컴퓨터공학
> - 통계학
> - 경영과학
> - 계량경제학
> - 금융공학
> - 물리학
> - 각종 엔지니어링

**2) 프로그래밍 활용능력(실습)**
> **엑셀과 통계분석 툴로도 가능하지만, 모든 상황에 유연한 대응과 자동화를 위해 최소 1개이상의 언어능력 필요**

**3) 설득 및 설명능력(현실)**  
> - **인문학적 소양:** 데이터 해석 + 가치발견 + 가설검증 + 상대에게 설명
> - **시각화:** 기술과 예술의 중간단계로 미적감각 + 연습 + 컴퓨터활용능력
> - **프리젠테이션:** 설명 능력으로 상대가 듣고싶은 주제발견 + 표현문구 연구 + 스토리라인 구현 + 컴퓨터활용능력
(내말에 현혹시키기 위함이 아님)