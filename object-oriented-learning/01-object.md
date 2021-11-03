## 절차지향과 객체지향
1) 절차지향 : 쉽고 빠르다. 근데 효율적이지 않다. 요구사항이 바뀌니까 데이터를 사용하는 방식, 필요한 데이터도 바뀌고 있다. 요구사항이 또 바뀌면, 또 그 안에서 내용을 추가해야 한다. 그러면 시간과 절차가 복잡해지고, 수정이 어려워진다.


2) 객체지향 : 객체지향은 객체를 가지고 데이터와 프로시저를 하나로 묶는다. 그리고 객체는 프로시저만 접근할 수 있게 한다. 따라서 다른 객체에서는 객체의 데이터에 바로 접근하지 못한다. 
    * 객체가 다른 객체 안의 데이터에 접근하는 것을 막는다.
    * 객체는 프로시저를 이용해서 외부에 객체를 공유해서, 서로 프로시저를 공유하는 식으로 연결된다.
    * 조금 어려울 수 있다 (데이터 프로시저를 객체로 묶어야 하므로).
    * 하지만 적응하고 나면 매우! 효율적이다. 코드를 수정하기가 수월해진다 (캡슐화).

***

## 절차 지향과 비용 문제
절차 지향을 할 때에는 계속 요구사항이 추가될 때마다 코드의 수정이 이루어져야 하기 때문에, 코드가 점점 조건이 많아져 복잡해지는 마당에 수정하기 위해서는 이곳저곳 열심히 찾아야 하고.. 실수도 잦아진다.

절차지향을 하면 처음에는 쉬운 것 같은데, 하는 과정에서 코드를 복사하게 되고, 수정을 하게되고... 너무 어렵고 비용이 많이 든다.

## 객체란?
* 객체의 핵심 -> 기능 제공 
  * 객체를 사용하는 입장에서의 객체는 '기능'으로 정의된다. 객체가 어떤 '기능'을 제공하느냐?
  * 내부적으로 가진 필드(데이터)로 정의하지 않음.
  * 예시) 소리제어기(소리기능 증가/감소 등으로 정의)

### 객체의 기능을 어떻게 정의하는가? : 기능 명세
* 기능의 명세는 메소드를 이용해서 작업한다.
* 이름 - 파라미터 - 리턴타입

```java
public class VolumeController {
    public void increase(int inc) {
    ...
    }
    public void decrease(int dec) {
    ...
    }
    public int volume() {
    ...
    }
}
```
-> '볼륨조절'이라는 기능 안에 어떤 것들을 넣을 것인지 정의

* 객체와 객체는 기능을 사용해서 연결한다. 따라서 기능을 사용하기 위해서는 메서드를 호출한다.
```python
VolumnController = VolumnController()
```

## 용어
### 메세지
* 객체와 객체의 상호작용 : 메세지를 주고 받는다고 표현한다. 메서드를 호출하는 메시지, 리턴하는 메시지, 인셉션 메시지 등...
