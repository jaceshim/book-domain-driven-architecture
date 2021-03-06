# Chapter6 : 유스케이스를 구현하기 위한 '애플리케이션 서비스'

## 6.1 애플리케이션 서비스란 무엇인가? *P106*
- 애플리케이션 서비스를 한마디로 표현하면 유스케이스를 구현하는 객체라고 할 수 있다.

> 도메인 객체를 조작해서 이용자의 목적을 달성하게 이끄는 객체인 애플리케이션 서비스의 이름에 애플리케이션이라는 단어가 들어가는 것은 어찌 보면 당연할 일이다. *P106*

### 6.2.3 사용자 정보 확인 처리 구현하기 
- 도메인 객체의 행동을 호출하는 것은 애플리케이션 서비스의 책임이다. *P113*
- 도메인 객체를 외부에(package범위 밖) 공개한다는 선택은 각 처리의 코드를 단순하게 만들 수는 있지만, 그 대가로 많은 위험성을 안게 된다.
- 필자는 도메인 객체를 직접 공개하지 않는 쪽을 권한다. 도메인 객체를 비공개로 남겨두고 클라이언트에 데이터 전송을 위한 객체 (DTO, data transfer object)를 만들어 여기에 데이터를 옮겨 넣어 반환하는 방법이다.*P114*

## 6.3 도메인 규칙의 유출 
- 애플리케이션 서비스는 도메인 객체가 수행하는 태스크를 조율하는 데만 전념해야 한다. 따라서 ** **애플리케이션 서비스에 도메인 규칙을 기술해서는 안된다.** 도메인 규칙이 애플리케이션 서비스에 기술되면 같은 코드가 여러 곳에서 중복되는 현상이 나타난다. *P126*
- 도메인 객체에 규칙을 구현하면 같은 규칙을 구현한 코드가 여러 곳에 반복되는 것을 방지하고 향 후 수정 시에도 수정이 필요한 곳을 빠드려 발생하는 버그를 막을 수 있다. *P133*

## 6.4 애플리케이션 서비스와 프로그램의 응집도 
- 응집도는 모듈의 책임 범위가 얼마나 집중되어 있는지 나타내는 척도다.
- 응집도가 높으면 모듈이 하나의 관심사에 집중하고 있다는 의미이므로 모듈의 견고성, 신뢰성, 재사용성, 가독성의 측면에서 바람직하다.*P133*

## 6.5 애플리케이션 서비스의 인터페이스 
- 애플리케이션 서비스의 인터페이스를 미리 만들어 두면 이를 구현한 목업 객체를 이용해 애플리케이션 서비스의 실제 구현이 완료되기를 기다릴 필요 없이 클라이언트의 구현을 진행 할 수 있다.

## 6.6 서비스란 무엇인가? *P144*
- 서비스는 클라이언트를 위해 무언가를 해주는 존재다. 값 객체와 엔티티는 **자신을 위한 행동을 갖고 있지만** **서비스의 행동은 자신을 위한 것이 아니다.** 따라서 서비스는 어떤 사물보다는 활동이나 행동인 경우가 많다.
- 도메인 서비스와 애플리케이션 서비스는 대상 영역은 다르지만, 본직적으로 같은 것이다. 같은 서비스지만, 그 방향이 도메인이냐  애플리케이션이냐에 따라 나뉜다.

### 6.6.1 서비스는 무상태다
- 서비스는 자신의 행동을 변화시키는 것을 목적으로 하는 상태를 갖지 않는다. (상태를 갖는 경우도 일부 있음)

## Summary
- 애플리케이션 서비스를 구현할 때는 도메인 규칙에 대한 기술이 포함되지 않게 주의해야 한다.

