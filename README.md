# 프로젝트명: 게임작품명 Don't forget the memory : re

# [ 목차 ]
### 1. [컨셉](#컨셉)
### 2. [관련 이미지와 동영상](#관련-이미지-동영상)
### 3. [대표 이미지 그리고 컨셉과 대표이미지 기반 작품 묘사](#대표-이미지)
### 4. [게임 시스템 디자인](#게임-시스템-디자인)
### 5. [키보드 이벤트에 대한 흐름도](#키보드-이벤트에-대한-흐름도)

# [컨셉]

## 메인컨셉 : 여햄,모험

- 자유롭게 월드를 탐색하면서 성장하는게 주 목표

### 서브 컨셉 1 : 액션성

- 액션성을 적극적으로 도입하여 게임을 플레이하는것에대해 지루함을 감소시킴

### 서브 컨셉 2 : 성장

- 성장을 하면서 점점 다양한 컨텐츠들이 오픈하게됨

### 서브 컨셉 3 : 환경

- 다양한 오브젝트 및 장소를 만들어내 똑같은곳만 맴도는 지루함을 감소시킴

### 서브 컨셉 4 : 퀘스트

- 평범하게 다른 환경이 저절로 열리면 게임이 너무 쉬워 보이니 
- 해당퀘스트를 완료해야만 다른 환경이 오픈이되서 플레이가 지속되게끔 장려함

### 서브 컨셉 5 : 식생

- 사냥만하는 컨텐츠 외에도 다양한 식생을 추가해 채집,연구와 같은 플레이로 게임의 다양성을 이끌어냄

<br><br>

# [관련 이미지 동영상]


- 동영상
- 
<iframe width="560" height="315" src="https://www.youtube.com/embed/" frameborder="0" allowfullscreen></iframe>{% include 파일명.html id="IlXAM44ApJI url" %}  

 
<br><br>

# [대표 이미지]

![123455](https://user-images.githubusercontent.com/92343121/138663146-c109c2c6-5a1b-45a8-b38c-45d2a9e9af20.png)





<br>

## 1. 메커니즘

[도전 과제]

1.주어진 퀘스트를 클리어해야지만 다음 구역이 오픈됨

[재미 요소]

1. 단순히 전투로만 성장하는것이 아닌 다른 활동(채집,연구...)등으로로 성장하여 게임을 클리어할수있도록함
 

<br>

## 2. 이야기

[만들게 된 배경]  
코로나19로 집에 있는시간이 길어지다보니 어디론가 여행을가고싶다는 생각이 자주 들었는데
이번일 계기로 집에서도 100%는 아니지만 간접적으로라도 어딘가를 여행하고있다는 생각이 들게만드는
게임을 만들어보고싶다는 계획을 

[카메라 관점]  
2d 횡스크롤

<br>

## 3. 미적요소

[디자인][컬러]  
게임분위기가 대체적으로 밝은 색감의 분위기며 특정 구간 돌입시 분위기가 어두운색으로 반전되
게임을 플레이하는 입장에서 좀 더 몰입감을 느끼게 만들예정임

<br>

## 4. 기술

유니티

# [게임 시스템 디자인]


1. 게임 오브젝트 분해 (구성 요소 분석)

연번 | 오브젝트 이름 | 오브젝트 이미지
-- | -- | --
1 | 플레이어 |  ![12311](https://user-images.githubusercontent.com/92343121/138666046-d4c5b763-185b-408e-9596-1fdd44cd82d0.png)|
2 | 무기들 |  <img src = "https://user-images.githubusercontent.com/92343121/138687241-1e42e871-aa60-4a11-bfe3-08a5b2e736b7.png" width="200" height="200"/>
3 | 적 |  ![preview](https://user-images.githubusercontent.com/92343121/138666281-bc5cf401-5101-4471-82bc-4c91cae70688.png)|
4 | 배경 |  <img src = "https://user-images.githubusercontent.com/92343121/138686708-b545ed21-b903-4258-98cc-c30a11c94082.png" width="300" height="200"/>


# 2. 파라미터(속성) 뽑아 보기

1. 오브젝트 이름 (플레이어)

|속성|영문명칭|설명|비고|
|:----:|:----:|:----:|:----:|
|1|체력|p_Hp|플레이어의 생명력이며 0이되면 사망합니다|
|2|마력|p_Mp|플레이어의 마력이며 0이되면 스킬이발동되지 않습니다|
|3|이동속도|P_Mspeed|플레이어의 이동속도입니다|
|4|기본공격|P_normalA|플레이어의 기본공격입니다|
|5|스킬공격|P_skillA|플레이어의 스킬공격입니다|

2. 오브젝트 이름 : 아이템

|속성|영문명칭|설명|비고|
|:----:|:----:|:----:|:----:|
|1|돌|Stone|평범한 돌이며 게임진행에 필요한 오브젝트입니다|
|2|박스|Box|박스를 열어 아이템을 얻거나 발판으로 사용합니다|
|3|물|Water|평범한 물이며 게임진행에 필요한 오브젝트입니다|
|4|불|Fire|평범한 불이며 게임진행에 필요한 오브젝트입니다|
|5|힐링팩|Hillpack|힐링팩을 플레이어가 획득시 체력이 일정량 회복됩니다|
|6|마나팩|Mpack|마나팩을 플레이어가 획득시 마력이 일정량 회복됩니다|

3. 오브젝트 이름 : 적

|속성|영문명칭|설명|비고|
|:----:|:----:|:----:|:----:|
|1|슬라임|Slime|가장기본적인 적으로 쉽게 제압할 수 있는 몹입니다|
|2|거대슬라임|BSlime|크기가 커진 슬라임으로 일반슬라임보다 강력합니다|

# 3. 행동 뽑아 보기

1) 오브젝트 이름 : 플레이어

|연번|행동|설명|
|:----:|:----:|:----:|
|1|대기|아무행동도 하지않는 기본자세입니다|
|2|이동,점프|플레이어가 이동할 때 움직임이 생깁니다|
|3|공격|플레이어가 공격을하면 공격모션이 발동합니다|
|4|스킬|플레이어가 스킬공격을하면 스킬모션이 발동됩니다|
|5|죽음|플레이어 hp가 0이되면 사망합니다|

1) 오브젝트 이름 : 아이템
|연번|행동|설명|
|:----:|:----:|:----:|
|1|숨겨짐|플레이어가 찾아야지만 획득할 수 있습니다.|

1) 오브젝트 이름 : 적

|연번|행동|설명|
|:----:|:----:|:----:|
|1|이동|지정된 패턴으로 계속 움직입니다|
|2|공격|플레이어를 발견시 공격에 들어갑니다|
|3|죽음|hp가 0이되면 죽습니다|

 
# 4. 상태 뽑아 보기

1) 오브젝트 이름 : 플레이어

|순번|현상태|전이상태|전이조건|
|:----:|:----:|:----:|:----:|
|1|hp가 100일때|슬라임의공격(hp-20)|슬라임이 공격을 한 대 적중시켰을경우|
|2|hp가 100일때|거대슬라임의공격(hp-40)|거대슬라임이 공격을 한 대 적중시켰을경우|

2) 오브젝트 이름 : 아이템

|순번|현상태|전이상태|전이조건|
|:----:|:----:|:----:|:----:|
|1|새것|사라짐|플레이어가 획득 했을시 사라집니다|

3) 오브젝트 이름 : 적

|순번|현상태|전이상태|전이조건|
|:----:|:----:|:----:|:----:|
|1|hp가 100일때|플레이어의 기본공격(hp-10)|플레이어가 기본공격을 한 대 적중시켰을경우|
|2|hp가 100일때|플레이어의 스킬공격(hp 20 ~)|플레이어가 스킬공격을 한 대 적중시켰을경우|

# 5 게임의 규칙


1) 핵심 규칙
1. 플레이어는 숨겨진 아이템 오브젝트를 찾아 던전을 빠져나와야합니다
2. 플레이어는 적을의 공격을받아 hp가 0이되면 
진행상황이 모두 초기화되고 초기위치로 워프됩니다
3. 해당구역의 진행도를 일정이상 올리게되면 다음 구역으로 열리는 길이 오픈됩니다.

2) 보조 규칙

1.아이템(오브젝트는) 플레이어눈에 보이지않고 숨겨져있습니다
2.아이템을 얻기위해 통하는 길 또한 숨겨져 있어 숨겨진 루트또한 탐색해야합니다

# [키보드 이벤트에 대한 흐름도]

![키보드흐름도](https://user-images.githubusercontent.com/92343121/138695053-b65dc5f3-2f7f-4676-91b8-25f9024811bb.png)
