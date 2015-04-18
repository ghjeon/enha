## 목차

    

1 개요

2 특징

3 발전

4 한국에서의 ScummVM

5 ScummVM에서 지원하는 게임엔진 및 게임

6 ScummVM에서 지원 안하는 게임

## 1 개요 ¶

SCUMM Virtual Machine  

  

<del>어드벤처 게임의 MAME.</del> 고전 게임
[에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md)의 일종이라고 할 수 있지만 흔한
에뮬레이터들과는 성격이 좀 다르다. 이름의 유래대로 본래는 [SCUMM](SCUMM.md) 게임들을 현대의 컴퓨터에서 실행시키는
목적으로 개발되었다. 그 뒤로 이런저런 잡다한 것들이 붙으면서 이제는 과거에 컴퓨터용으로 나온 [어드벤처게임](%EC%96%B4%EB%93%9C%EB%B2%A4%EC%B2%98%20%EA%B2%8C%EC%9E%84.md)을 모조리 다
실행시키는 것을 목표로 하고 있는 듯하다.

## 2 특징 ¶

SCUMM이 원래부터 다양한 기종으로의 이식을 전제로 해서 만들어진 엔진이기 때문에 ScummVM의 원래 취지도 SCUMM 게임들을 현대의
하드웨어에 맞춰서 이식한다는 것에서 시작했다. 다른 에뮬레이터들이 주로 하드웨어를 분석해서 하드웨어가 가진 기능을 재현하는 것을 목표로
하고있다면 ScummVM은 소프트웨어를 분석해서 현대의 하드웨어 환경에서 실행할 수 있도록 재컴파일 하는 것이라고 보면 된다. 하드웨어가
아니라 게임엔진을 재구성하는 것. 그렇기 때문에 다른 에뮬레이터들은 원래의 [ROM](ROM.md) 혹은 디스크를 원본 그대로 떠낸
이미지가 필요하지만 ScummVM은 게임의 데이터 파일만 있으면 된다.`[1]` 그런 면에서 보자면 에뮬레이터가 아니라고 할 수 있지만
ScummVM에서 지원하는 게임들이 대부분 현재에는 없는 하드웨어 환경에서 실행되도록 만들어진 탓에 일부 하드웨어 에뮬레이션 기능이 추가되어
있으므로 에뮬레이터가 아니라고 하기도 뭣하다.

  

ScummVM이 지원하는 대부분의 게임들은 [DOSBox](DOSBox.md) 등 다른 에뮬레이터로도 실행 가능한 것들이다. 그렇지만
굳이 ScummVM을 쓰는 이유는 다른 에뮬레이터들은 하드웨어 전체를 에뮬레이트하고 그 안에서 프로그램을 다시 실행시키는 복잡한 구조로
되어있지만 ScummVM은 현재의 하드웨어에서(직접 지원이 안되는 일부만 에뮬레이트하고) 바로 실행되도록 만든 것이므로 속도가 넘사벽으로
빠르고 자원을 훨씬 적게 쓴다. [DOS](DOS.md) 말기나 초기의 윈도우9x 게임을 DOSBox로 돌리려면 상당한 컴퓨팅 파워가
필요하지만 ScummVM은 어지간한 구형 컴퓨터에서도 쌩쌩하게 돌아간다. 윈도우9x용 프로그램인 경우 XP 이상에서 실행시킨다고 호환성
설정이나 패치같은 거 안해도 된다.  
또한가지 장점은 ScummVM에서 지원하는 게임이라면 여러가지 기종용으로 나온 다른 버전들을 해당 기종의 에뮬레이터를 일일이 갖추지 않아도
ScummVM 하나로 다 돌려볼 수 있다는 점. 물론 각각의 전용 에뮬레이터를 사용하는 것에 비하면 재현도는 조금 떨어지지만 대신에 다른
에뮬레이터로는 할 수 없는 기능을 사용할 수 있고 좀 더 편리한 실행환경을 제공한다.`[2]`  
단점은 일부 게임들의 경우 데이터 파일을 추출해내는 절차가 복잡해서 초보자들에게는 어려울 수도 있다는 것. 화면 효과 등이 그리 다양하지
않다는 것. DOS용과 윈도우용 게임을 제외한 나머지 플랫폼용으로 나온 게임 버전들에 대한 지원이 한정적이거나 부정확하다는 것 등이
있다.<del>어차피 DOS나 윈도우 이외의 다른 세계가 있다는 걸 아는 사람이 별로 없으니 이건 단점이 아닐수도...</del>

  

## 3 발전 ¶

스웨덴 출신의 프로그래머 Ludvig Strigeus가 2001년 10월에 0.01 버전을 처음 발표해 현재 10년이 넘었다. 처음에는 이름
그대로 SCUMM 게임만을 대상으로 하고 있었지만 여러 사람들이 붙으면서 다양한 게임 엔진이 추가되어 2011년 현재에는 100가지가 넘는
게임을 지원하는 엄청난 크기로 성장했다. Revolution Software같은
[대인배](%EB%8C%80%EC%9D%B8%EB%B0%B0.md) 회사들은 자기네가 만든 고전 게임들에 대한 자료까지 제공하며
적극적으로 프로젝트를 지원하기도 했다.  
0.2 버전에서 '마법사 사이먼(Simon the Sorcerer)'을 지원한 것을 시작으로 SCUMM이 아닌 게임이 추가되기 시작했다.
SCUMM 게임의 수는 한정되어 있기 때문에 이미 SCUMM에 대한 지원이나 업데이트는 오래전에 끝이난 거나 다름없는 상태이고 지금은 버전이
올라갈때마다 새로운 게임 엔진이 추가되고 있다.  
2007년 6월에 나온 0.10.0 버전부터 [시에라](%EC%8B%9C%EC%97%90%EB%9D%BC%20%EC%97%94%ED%84%B0%ED%85%8C%EC%9D%B8%EB%A8%BC%ED%8A%B8.md)의 AGI 엔진이 추가되고 2010년 10월 1.2.0
버전에는 SCI 엔진이 추가되면서 사실상 시에라에서 나온 거의 모든 어드벤처 게임이 실행가능하게 된다. 어드벤처의 전성기를 이끌었던 양대
라이벌 회사의 거의 모든 게임이 다 돌아가게 되었으니 이제는 **Scumm**VM이라는 이름이 유명무실해진 지경. 지금도 계속해서 새로운
게임엔진을 업데이트하고 있다. 하나의 엔진이 도입되면 그 엔진을 이용한 게임은 거의 다 추가된다고 볼 수 있는데 그러다 보니 어드벤처가 아닌
게임들도 몇개인가 포함되어 있다.`[3]`

  

## 4 한국에서의 ScummVM ¶

  

ScummVM이 원래 원프로그램 소스를 분석해 개조하는 방식이므로 이를 이용해 루카스 게임들의 한국어판을 만드는 용도로 사용되어 일찌감치
한국어판이 나왔다. 그덕에 현재 대부분의 루카스 어드벤처 게임들이 한글화된 상태.  
그런데 해외에서 SCUMM만이 아닌 다양한 어드벤처 게임을 지원하는 멀티 프로그램쪽으로 방향을 트는 동안에도 국내에서는 오로지 SCUMM
게임 전용 실행기로만 취급을 해서 SCUMM 이외 다른 게임들은 한국어판에서는 아예 빼버리고 지원을 안하는 경우도 있었다. 원본
ScummVM이 SCUMM에 대한 추가지원이 사실상 끝나고 새로운 게임엔진을 계속 업데이트하는 형태가 된 뒤로는 사실상 한국어판
ScummVM의 개발도 중단된 상태. ScummVM에서 시에라 게임도 지원된다는 사실을 아예 모르는 경우가 태반이다.

  

## 5 ScummVM에서 지원하는 게임엔진 및 게임 ¶

  * SCUMM - [SCUMM](SCUMM.md) 항목 참조.
  * AGI 및 SCI - 시에라에서 만든 거의 모든 DOS용 어드벤처 게임들.  

  * AGOS - 마법사 사이먼 1,2, [엘비라](%EC%97%98%EB%B9%84%EB%9D%BC.md) 1,2, Personal Nightmare 등
  * GOB - 고블린 시리즈, Bargon Attack, Lost in Time, 윈의 모험 등.  

  * MADE - 맨홀, Leather Goddesses of Phobos 2, 조크 행성 등  

  * 그외에...  

Beneath a Steel Sky  
Broken Sword 1,2  
Cruise for a Corpse  
미래전쟁  
[디스크월드](%EB%94%94%EC%8A%A4%ED%81%AC%EC%9B%94%EB%93%9C.md) 1,2  
Dragon History  
Drascula: The Vampire Strikes Back  
아마존의 여왕  
지구의 상속  
Nippon Safes Inc.  
키란디아의 전설 1,2,3  
Touche: The Adventures of the Fifth  
7번째 손님  
링월드  

## 6 ScummVM에서 지원 안하는 게임 ¶

  

  * MADS - [마이크로프로즈](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%ED%94%84%EB%A1%9C%EC%A6%88.md)에서 만든 어드벤처 게임엔진. 아마존의 비밀, 돌아온 악령, 마스터 루의 수수께끼 등에 사용됨. 지원할 계획이 아주 없는 것은 아니지만 개발하겠다고 나선 사람이 없어 진행이 안되고 있다고 함.  

  * [어둠속에 나홀로](%EC%96%B4%EB%91%A0%20%EC%86%8D%EC%97%90%20%EB%82%98%20%ED%99%80%EB%A1%9C%201.md) \- 한때 추가하자는 움직임이 있었으나 ScummVM은 2D 게임만을 다루어야 한다는 반발이 나왔고, 개발자들 중 대빵급 인물이 **어둠속에 나홀로는 어드벤처가 아니라 액션게임이다**라는 <del>뻘소리</del>주장을 하는 바람에 제외됨.<del>그럼 야구게임이나 롤플레잉 게임은 왜 들어가 있는 건데?</del>  

  * Another World - 이쪽도 논란끝에 결국 제외됨.  

`\----`

`[1]` 원본 그대로의 상태라면 오히려 실행이 안되는 경우가 많다.  
`[2]` 게임기용 버전인 경우 게임기라는 특성상 여러가지 제약이 있는데 ScummVM에서는 그런 제약 없이 컴퓨터용 버전과 거의 같은
환경으로 게임을 할 수 있다.  
`[3]` '키란디아의 전설'과 같은 엔진을 사용하는 롤플레잉 게임 '지혜의 땅'이라든가.
