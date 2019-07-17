---
title: 챗봇UX 6편, 학익진(鶴翼陣), 챗봇 대화모델 구성 전략
tags: [blog, chatbot-biz, Chatbot-UX]
keywords: blog
summary: 분명 챗봇 대화모델을 디자인하고 있었는데 학익진? 
sidebar: blog_sidebar
permalink: blog_012_UX06_strategy.html
folder: blog

---

## 대화모델 배치는 곧 UX전략
대화형 인터페이스*는 그래픽 인터페이스**와 다르게 가시적이지 않다. 챗봇이나 음성봇을 시도하고 있는 많은 기업들이 이 부분에 대해 어려움을 느끼고 있다. 대화AI의 대화모델을 분류하고 A4에 스케치를 해보았다. 오잉. 다 그리고 나니 학익진이 되었다. 메인 시나리오가 맨 앞에 서고, 그 뒤로는 FAQ가 원을 그리듯 포진했다. 그 뒤에는 일상 대화가 기다리고 있다. 결국 우리가 대화AI라는 시스템을 통해 해결하고자 하는 목적이 있고 대화모델 하나하나가 대응할 수 있는 콘텐츠 단위이고, 이를 배치하는 전략이라는 것을 알게 되었다. 

{% include note.html content="* 대화형 인터페이스 (CUI, Conversational User Interface) <br/> 챗봇이나 음성봇과 같은 자연어로 대화를 주고받는 방식으로 컴퓨터와 상호작용하는 사용자 인터페이스" %}
{% include note.html content="** 그래픽 인터페이스 GUI, Graphic User Interface<br/> Text, Image, 버튼, 폴더, 커서 등 시각적 메타포를 활용하여 인지시키고 클릭, 터치와 같은 입력을 통해 상호작용하는 사용자 인터페이스 " %}

{% include image.html file="blog/012_turtleship_01.jpg" alt="사용자가 왼쪽에 있고 학익진을 펼치고 있는 거북선 함대가 오른쪽에 배치" caption="USER가 적선(敵艦), 이에 맞서는 대화 AI의 대화모델들" %}
 
배 한 척 한 척은 사용자가 말한 내용의 의도(Intent) 단위로 대응할 수 있는 하나하나의 스킬이다. 어떤 스킬은 단답형(Single Turn)으로 대답하는 스킬이고, 어떤 스킬은 되묻기를 필요한 만큼 반복하여(Multi-Turn) 답변이나 처리를 위해 필요한 정보를 사용자로부터 얻어낸다. 각각의 배들이 어떻게 적선(敵艦)을 상대하는지 살펴보자.

## 메인 시나리오 중심 전략

최근 챗봇으로 모든 것을 해주는 것의 한계를 느끼고 핵심 업무를 담당시키고, 최초 만남 인사에서 자신의 역할을 잘 소개하여 무작위 공격에서 벗어나는 시도가 많다. 이는 챗봇이나 AI스피커 등의 대화AI서비스를 제공하는 업체에게 효율적인 솔루션이다. 동시에 사용자에게도 도움이 된다. 말하는 로봇이라고 대화로 마냥 즐겁게 해 준다고 기대했다가 실망하게 하는 것이 아니라 본론으로 유도하는 것이다. 사용자는 최초의 대화에서 자신이 원하는 것을 얻을 수 있다고 판단되면 대화를 시도하고, 아니면 그만둔다.

{% include image.html file="blog/012_turtleship_02.jpg" alt="사용자가 왼쪽에 있고 학익진을 펼치고 있는 거북선 함대가 오른쪽에 배치, 사용자가 메인시나리오로 바로 들어간다." caption="잘 만든 대화AI는 바로 본론으로 들어간다. 아니, 들어가게 만든다." %}

거두절미, 본론 직행은 서로 Win-Win이다. 사용자는 시간낭비를 최소화하고 서비스 제공자는 사람이 처리해줄 것을 로봇이 대신해주었다는 점에 덧붙여 불필요한 서버 리소스까지 줄일 수 있다. 


## 문의가 많을 수밖에 없는 고관여 서비스라면? 전환 전략

렌터카나 자동차 리스, 인테리어, 세무, 법무, IT솔루션과 같이 고객이 초기에 알아야 하는 것이 많고 선택사항이 많은 고관여 서비스라면 FAQ(자주 묻는 질문, Frequently Asked Question)를 통해 궁금증을 해소시켜줄 수 있다. 고관여 서비스를 제공하고 있는 사업자 또는 업체의 영업사원들의 이야기를 들어보면 어떤 경우에는 설명만 45분간 진행하고 구매로 이어지지 않는 경우도 허다하다고 한다. 우리 회사 세무사도 세금과 세법을 이해시키는 데 많은 시간을 소비한다고 한다. 자기 입장에서는 뻔한 문의사항이지만 고객 입장에서는 정말 궁금하다. 이런 경우에는 대화AI가 자주 문의되는 질문에 대해서 답변을 해주면서 고객을 학습시킬 수 있다. 고객은 그 분야에 상당한 지식을 얻게 되고 일부 선택사항은 마음속으로 정하게 된다. 이렇게 육성된 고객은 영업사원과의 상담에서 구매 의사결정을 빠르게 진행할 수 있다. 영업사원 입장에서도 반복적인 문의사항에 답변하는 수고가 줄어들게 된다. 

{% include image.html file="blog/012_turtleship_03.jpg" alt="사용자가 FAQ를 연쇄적으로 거친 후에 메인시나리오(거북선)으로 돌아옴" caption="연쇄적인 FAQ처리 후에 메인시나리오로 전환" %}

특히 Text형 챗봇의 경우 꼬리에 꼬리를 무는 문의사항을 처리하기에 용이하다. 어떤 문의사항에 답변은 다음 문의사항을 떠올리게 하는 경우가 많다. 가령 대학교 학사 챗봇에게 겨울방학이 언제냐고 물어보고, 대답을 들었다고 치자. 이때, 학생은 계절학기 신청은 언제까지 인지 궁금할 수 있다. 이때, 예상 질문으로 챗봇이 "계절학기 신청 일정은?"이라는 버튼을 제시한다면, 사용자는 키보드 타이핑(약 29타)을 하지 않고 버튼 클릭 한 번으로 궁금증을 해소할 수 있다. 상당한 궁금증 해소 후에는 최종적인 메인시나리오로 전환한다. 결국 실제 사업에 도움이 되는 영업기회 접수, 서비스 신청, 견적요청 등 메인시나리오 후보다.

단비에이아이의 랜딩페이지(https://danbee.Ai)에 있는 챗봇은 기본적으로 챗봇에 대해 소개하고, 챗봇이 어떤 일을 할 수 있는지 안내한다. 그리고 회원가입을 해서 서비스를 써볼 수 있도록 유도한다. 그 외에 사용법에 대한 FAQ는 버튼으로 노출되어 있지는 않지만 받아칠 준비를 항상 하고 있다. 

{% include image.html file="blog/012_turtleship_06_danbeewebsite.jpg" alt="danbee.Ai홈페이지" caption="단비 홈페이지에서 일하고 있는 단비봇. FAQ에 응답하는 동시에 챗봇 제작 의뢰를 접수받는다." %}

## 일상 대화도 목적 달성으로 전환하는 지혜
일상 대화 속에서 챗봇의 목적을 달성할 수 있도록 돌려주는 것도 가능하다. 날씨에 대한 이야기도 대화AI의 목적과 관련된 대화로 전환 가능하다. "비 온다"라는 고객의 일상 대화 멘트에 영화챗봇은 "비 오는 날은 영화관에서 데이트 어떠세요?", 배달음식 챗봇은 "비 오는 날은 역시 치맥!", 챗봇 회사는 "비 오는 날도 챗봇!"이라고 던질 수 있는 것이다. 

{% include image.html file="blog/012_turtleship_07_smalltalk.jpg" alt="채팅창에서 비가 온다고 하면, 챗봇이 비오는 날엔 챗봇 만들자고 하는 대화 예시" caption="실제 단비봇에게 비 온다고 하면 나오는 메시지" %}

또 다른 예를 들어보겠다.  대학교 학사 문의사항에 응답하는 챗봇에게 "방학 때 뭐하지?"라고 물어봤을 때, "여러 가지를 시도해 보세요!"라고 답변하고 끝낼 수 있지만, 방학 때 할 수 있는 것들을 카드 형태로 보여주면. <겨울 방학 때 뭐할지 고민되는 대학생>이라는 매우 세부적인 Segment에 있는 고객을 대상으로 광고가 된다. 학사팀은 챗봇이라는 창구를 통해 대학생을 위한 다양한 교육과 경험의 기회를 제공할 수 있다.

{% include image.html file="blog/006_level_4_carousel.gif" alt="겨울방학때 뭐하지? 라고 물어본 사용자에게 계절학기 수강신청, 캐나다 어학연수, 유럽배낭여행등을 추천하고 있는 챗봇 대화 예시" caption="잡담을 영업기회로. 대화 맥락기반 추천" %}


{% include note.html content="danbee.Ai에서는 이러한 광고를 대화 맥락 기반 광고(CCBA, Conversational Context Based Advertisement)라고 한다." %}

{% include image.html file="blog/012_turtleship_04.jpg" alt="사용자가 잡담을 시도했다가 다시 메인시나리오로 돌아오는 전략지도" caption="일상대화, Small Talk으로 가더라도 다시 메인시나리오로 돌리자." %}

잡담을 본론으로 바꾸는 기술은 영업사원들의 기술이다. 숙련된 영업사원은 너무 노골적이지 않느냐고 반문할지도 모르겠다. 하지만 사용자는 로봇이라는 것을 알고 있다. 사람이 달라붙어서 가입해라~ 사라~ 하면 부담스러울지 모르겠지만 홈페이지에 방문한 잠재고객에게 챗봇이 추천하는 서비스를 받아 보는 것은 흥미로운 경험이다. 최소한 팝업으로 면전에 들이대는 것보다는 노골적이지 않다. 

## 최후의 보루, 폴백(Fallback, 대비) 메시지

모든 질문에 답할 수 있는 사람이 없듯, 모든 질문에 답할 수 있는 챗봇도 없다. 특히 챗봇 시대의 역사적인 여명이 트는 시점이다 보니, 챗봇을 보고 실력을 테스트 하는 사람이 많다. 답할 수 없음을 겸허히 받아들이고 챗봇이 해줄 수 있는 일의 범위, 어떻게 이야기해야 잘 처리해줄 수 있는지를 친절히 알려주자(봇 알못 배려심). 그리고 메인시나리오로 전환하는 것이 옳은 전술이다. 혹시, 챗봇을 적극적으로 개선하고 있는 베타 테스팅 단계라면 개선점을 접수받는 시나리오로 전환할 수 도 있을 것이다.

{% include image.html file="blog/012_turtleship_05.jpg" alt="맨 뒤에 있는 Fallback 시나리오로 갔다가 다시 메인시나리오로 돌아오는 그림" caption="나무배에게 미사일은 가혹하다. 챗봇의 실력을 테스트하는 사람은 미사일이다." %}

어떤 챗봇은 아예 Fallback 시나리오가 없는 경우도 있다. 즉, 다시 처음부터 시작하도록 하는 것이다. 이런 경우에는 더욱 메인시나리오에 집중하게 된다. 무리한 부탁을 들어주지 않는다는 것을 단호하고 챗봇스럽게 표현했다고나 할까? 챗봇 시대의 초창기에는 아무래도 단호한 챗봇을 많이 만나게 될 것이다. 그렇다 보니 섬세한 폴백 메시지는 또 하나의 브랜딩 요소가 될 수 있다. 

## 챗봇 시대의 서막. 전략은 끝없이 진화한다.

챗봇 시대는 이제 시작이다. 모든 웹사이트, 앱에 대화AI가 붙어 사용자를 도와줄 것이다. 웬만한 사물들은 말을 알아듣고, 대응할 수 있게 될 것이다. 여기서 공유한 학익진과 기본적인 전략은 기본에 불과하다. 시간이 지날수록 대화모델 구성 전략은 발전할 것이고, 중요한 고객 대응 채널로 자리 잡을 것이다. 누군가는 만들어낼 새롭고 위대한 대화모델 디자인 전략이 기대된다. 

<hr>

### 보너스 1. 자연어 처리가 없는 대화AI의 전략
위에서 정리한 전략들은 자연어 처리를 전제하여 정리한 내용이다. 당연하게도 자연어 처리를 하지 않는 형태로 대화서비스를 할 수도 있다. 전화기를 통해서 제공되는 ARS가 대표적인 예다. 정해진 트리(Tree) 구조에 따라 버튼을 눌러 궁금증을 해소한다. 마지막엔 상담원으로 전환되거나 상담콜을 요청하기 위해 전화번호를 남기는 구조다. 전화가 아닌 Text형 서비스도 존재한다. 웹사이트에 방문하면, Text입력창이 없고 버튼을 눌러 궁금증을 해소한다. 마지막엔 ARS처럼 상담원으로 전환하거나 상담콜을 요청하기 위해 전화번호나 e-mail주소를 남긴다. 10개 이하의 문의사항만 자동 응답하게 한다고 하면, 매우 직관적이고 효율적인 방법이다. 하지만 20개가 넘어가면, 하위 메뉴를 보여주며 넘어가는 트리구조가 되며 이는 곧 [이전] [맨 처음]과 같은 시퀀스(Sequence)를 관리하는 개념이 필요하게 된다. 다시 말해, 메뉴에 안 보이더라도 자연어로 입력하면 답변이 나온다는 것이 자연어 기반 대화AI의 가장 큰 장점이다.

<hr>

### 보너스2. 학익진 구조의 대화AI만드는 절차
개발자가 아니더라도 챗봇을 만들 수 있는 챗봇 빌더가 많이 나와있다. 접수처리는 이메일을 보내주는 API나 구글 스프레드시트 등 클라우드 서비스의 API를 활용해서 구현이 가능하다. 이보다 강력한 시스템 연동이 필요하다면 개발자와 의논하자.

1. FAQ를 엑셀에 정리해서 한 번에 챗봇 빌더 서비스에 올린다. 

2. 메인시나리오를 추가한다. (필요하다면 API를 연계한다.)

3. 필요하다면 일상 대화 시나리오를 추가한다. 

4. 내부 테스트, 내부 오픈, BETA 오픈을 거쳐 부족한 FAQ와 예문을 추가하고 메인시나리오를 다듬는다. 

5. 최종적으로 BETA딱지를 뗀다. 


<hr>
작성자 : RAPA

### 함께해요! 챗봇시대:)
모든 사물, 디지털 매체와 말이 통하는 시대! danbee.Ai와 함께 반드시 오게될 챗봇시대를 열어갔으면 좋겠습니다.

{% include tip.html content="danbee.Ai는 보다 나은 챗봇, 챗봇만들기, 챗봇운영 경험을 만들기 위해 노력하고 있습니다. https://danbee.Ai 에서 여러분만의 챗봇을 🌱싹틔우세요!" %}