# Chapter1 : 도메인 주소 설계란?


## 1.1 도메인 주도 설계란 무엇인가? *P2*
- 개발자가 소프트웨어를 개발하면서 가치 있는 지식과 그렇지 않은 지식을 잘 구분하려면 어떤 능력이 필요할까? 당연한 말이지만, 먼저 소프트웨어 이용자의 세계를 이해해야 한다. ( P2 )
- 도메인 주도 설계는 지식을 코드에 녹여 넣을 수 있게 하는 개념이다.

## 1.2 도메인 지식에 초점을 맞춘 설계 기법 *P3*
- 도메인은 영역이란 뜻이다. 특히 소프트웨어 개발에서 말하는 도메인은 '프로그램이 쓰이는 대상 분야' 라는 의미로 쓰인다.

### 1.2.1 도메인 모델링이란 무엇인가? *P5*
- 모델은 현실에 일어나느 사건 혹은 개념을 추상화환 개념이다. 추상이란 여러 사물 혹은 개념에서 공통적인 것을 뽑아 파악하는 것으로, 현실의 모든 것을 반영하는 것이 아니다. 상황에 따라 취사 선택이 필요하다. 무엇을 버리고 무엇을 취할지는 도메인에 따라 결정된다.
ex) 도구로서의 펜과 상품으로서의 펜

- 코드로 나타낼 대상을 소프트웨어가 맡은 바 역할을 다하기 위해 필요한 정보로 한정 한다면, 현실적으로 실현하는 데 문제가 없다.
- **도메인 주소 설계에서는 도메인 개념을 모델링한 모델을 도메인 모델 이라고 한다.**

### 1.2.2 지식을 코드로 나타내는 도메인 객체 *P6*
- 도메인 모델으르 소프트웨어 형태의 동작하는 모듈로 나타낸것이 도메인 객체이다.
- 도메인에 대한 날카로운 통찰은 구현 과정에서도 얻을 수 있다. *P7*

### Summary
- ** 도메인 주도 설계는 개발 극초기에도 어느 정도 효과를 볼 수 있지만, 도메인 주도 설계의 진정한 가치가 드러나는 것은 변화에 대응해 소프트웨어를 수정 할때다.**

