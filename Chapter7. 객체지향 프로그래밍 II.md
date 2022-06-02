# Chapter7. 객체지향 프로그래밍 II

## 목차
1. [상속(inheritance)](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%83%81%EC%86%8Dinheritance "상속(inheritance)")
    - [1-1. 상속의 정의와 장점](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%83%81%EC%86%8D%EC%9D%98-%EC%A0%95%EC%9D%98%EC%99%80-%EC%9E%A5%EC%A0%90 "상속의 정의와 장점")
    - [1-2. 클래스간의 관계 - 포함관계](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EA%B0%84%EC%9D%98-%EA%B4%80%EA%B3%84---%ED%8F%AC%ED%95%A8%EA%B4%80%EA%B3%84 "클래스간의 관계 - 포함관계")
    - [1-3. 클래스간의 관계 결정하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EA%B0%84%EC%9D%98-%EA%B4%80%EA%B3%84-%EA%B2%B0%EC%A0%95%ED%95%98%EA%B8%B0 "클래스간의 관계 결정하기")
    - [1-4. 단일상속(single inheritance)](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%8B%A8%EC%9D%BC%EC%83%81%EC%86%8Dsingle-inheritance "단일상속(single inheritance)")
    - [1-5. Object클래스 - 모든 클래스의 조상](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#object%ED%81%B4%EB%9E%98%EC%8A%A4---%EB%AA%A8%EB%93%A0-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%A1%B0%EC%83%81 "Object클래스 - 모든 클래스의 조상")
2. [오버라이딩(overriding)](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9overriding "오버라이딩(overriding)")
    - [2-1. 오버라이딩이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9%EC%9D%B4%EB%9E%80 "오버라이딩이란?")
    - [2-2. 오버라이딩의 조건](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9%EC%9D%98-%EC%A1%B0%EA%B1%B4 "오버라이딩의 조건")
    - [2-3. 오버로딩 vs. 오버라이딩](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9-vs-%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9 "오버로딩 vs. 오버라이딩")
    - [2-4. super](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#super "super")
    - [2-5. super() - 조상 클래스의 생성자](https://github.com/hongcoding94/java_storage/blob/main/Chapter7.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#super---%EC%A1%B0%EC%83%81-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%83%9D%EC%84%B1%EC%9E%90 "super() - 조상 클래스의 생성자")
3. [package와 import]( "package와 import")
    - [3-1. 패키지(package)]( "패키지(package)")
    - [3-2. 패키지의 선언]( "패키지의 선언")
    - [3-3. import문]( "import문")
    - [3-4. import문의 선언]( "import문의 선언")
    - [3-5. static import문]( "static import문")
4. [제어자(modifier)]( "제어자(modifier)")
    - [4-1. 제어자란?]( "제어자란?")
    - [4-2. static - 클래스의, 공통적인]( "static - 클래스의, 공통적인")
    - [4-3. final - 마지막의, 변경될 수 없는]( "final - 마지막의, 변경될 수 없는")
    - [4-4. abstract - 추상의, 미완성의]( "abstract - 추상의, 미완성의")
    - [4-5. 접근 제어자(access modifier)]( "접근 제어자(access modifier)")
    - [4-6. 제어자(modifier)의 조합]( "제어자(modifier)의 조합")
5. [다형성(polymorphism)]( "다형성(polymorphism)")
    - [5-1. 다형성이란?]( "다형성이란?")
    - [5-2. 참조변수의 형변환]( "참조변수의 형변환")
    - [5-3. instanceof연산자]( "instanceof연산자")
    - [5-4. 참조변수와 인스턴스의 연결]( "참조변수와 인스턴스의 연결")
    - [5-5. 매개변수의 다형성]( "매개변수의 다형성")
    - [5-6. 여러 종류의 객체를 배열로 다루기]( "여러 종류의 객체를 배열로 다루기")
6. [추상클래스(abstract class)]( "추상클래스(abstract class)")
    - [6-1. 추상클래스란?]( "추상클래스란?")
    - [6-2. 추상메서드(abstract method)]( "추상메서드(abstract method)")
    - [6-3. 추상클래스의 작성]( "추상클래스의 작성")
7. [인터페이스(interface)]( "인터페이스(interface)")
    - [7-1. 인터페이스란?]( "인터페이스란?")
    - [7-2. 인터페이스의 작성]( "인터페이스의 작성")
    - [7-3. 인터페이스의 상속]( "인터페이스의 상속")
    - [7-4. 인터페이스의 구현]( "인터페이스의 구현")
    - [7-5. 인터페이스를 이용한 다중상속]( "인터페이스를 이용한 다중상속")
    - [7-6. 인터페이스를 이용한 다형성]( "인터페이스를 이용한 다형성")
    - [7-7. 인터페이스의 장점]( "인터페이스의 장점")
    - [7-8. 인터페이스의 이해]( "인터페이스의 이해")
    - [7-9. 디폴트 메서드와 static메서드]( "디폴트 메서드와 static메서드")
8. [내부 클래스(inner class)]( "내부 클래스(inner class)")
    - [5-1. 내부 클래스란?]( "내부 클래스란?")
    - [5-2. 내부 클래스의 종류와 특징]( "내부 클래스의 종류와 특징")
    - [5-3. 내부 클래스의 선언]( "내부 클래스의 선언")
    - [5-4. 내부 클래스의 제어자와 접근성]( "내부 클래스의 제어자와 접근성")
    - [5-5. 익명 클래스(anonymous class)]( "익명 클래스(anonymous class)")

---

## 상속(inheritance)

##### 상속의 정의와 장점

- 상속의 정의
> 상속이란? <br/>
> A클래스가 상속 받고 싶은 B클래스를 선택해서 물려받는다. <br/>
> 즉, 현실세계의 자식이 부모에게 재산을 상속 받는 행위와 같다. <br/>
>   - 상속의 종류 <br/>
>   ▶ 자식 클래스[하위 클래스 or 서브 클래스] : 상속 받는 클래스 <br/>
>   ▶ 부모 클래스[상위 클래스 or 슈퍼 클래스] : 상속을 해주는 클래스

- 상속의 대상
> 부모 클래스의 필드와 메서드를 물려받게 된다.<br/>
> 주의점으로는 private 혹은 default인 경우는 상속이 불가능하다.

**!Tip0.** [접근제어자에 대하여](https://blog.crazzero.com/155 "접근제어자에 대하여")

- 상속의 장점
> 중복된 코드를 줄일 수 있고, 유지 보수가 편리하며, 통일성이 있으며 다형성을 구현 가능

- 상속의 단점
> - 개방 폐쇄 원칙(캡슐화) 약화 <br/>
> ▶ 부모 클래스의 public, protected 메소드에 접근이 가능하기 때문에 부모 클래스의 구현 사항에 의존한다.
> :rotating_light: (주의사항) <br/>
>  자식 클래스 규칙에 부합하지 않는 부모 클래스 메소드가 존재하며 그 메소드가 의도치 않게 정상적으로 작동하게된다면 자식 클래스의 규칙을 위배한 결과를 반환하여 문제 발생. <br/> <br/>
> :speech_balloon: 완벽한 캡슐화를 원한다면 상속을 포기하거나 적절한 private 사용으로 인터페이스 은닉<br/>
> &nbsp; &nbsp; &nbsp; 또는 getter / setter등을 정확하게 상속을 구현하는 것이 추천한다.
> 
> - 설계가 유연하지 않음 - 클래스간 결합 문제 <br/>
> ▶ 자식 클래스에 기능을 점진적으로 추가하며 확장하는 목적으로는 편리 하지만 자식 클래스가 <br/>
> &nbsp; &nbsp; &nbsp; 부모 클래스를 상속하면 상호 간의 의존성(결합도)이 생긴다.<br/>
> &nbsp; &nbsp; &nbsp; 그 결과 결합도가 높아지면 부모 클래스의 변경으로 인한 자식 클래스가 취약해 질 수 있으며 <br/>
> &nbsp; &nbsp; &nbsp; 부모 클래스 수정 시 모든 자식 클래스의 테스트 및 수정 작업을 해야하는 번거로움이 생긴다.
> 
> - 리스코프 치환 원칙의 위배 <br/>
> ▶ 상위에서 말했던 것처럼 잘못된 상속으로 인한 캡슐화 약화, 클래스 간 결합도 문제로 인하여 리스코프 치환 원칙에 위배가 된다. <br/>
> <br/> 
> 리스코프 치환 원칙이란? <br/>
> 상위 타입을 사용하는 메소드에 하위 타입의 객체를 매개변수로 전달할 경우에도 정상 동작 해야함을 의미 <br/>
> 즉, 부모 클래스의 메소드 동작으로 어떤 인과관계가 정해지는 메소드에 자식 클래스의 성질에 기반하여 <br/>
>  overriding한 setter 동작이 그 인과관계를 해치는 경우가 발생하는데 이러한 경우 자식 클래스가 아니라 별도의 타입으로 정의해야한다.

**!Tip1.** [자바 디자인패턴- LSP : 리스코프 치환 원칙](https://ktko.tistory.com/entry/%EC%9E%90%EB%B0%94-%EA%B0%9D%EC%B2%B4-%EC%A7%80%ED%96%A5%EC%9D%98-%EC%9B%90%EB%A6%AC-SOLID-LSP-%EB%A6%AC%EC%8A%A4%EC%BD%94%ED%94%84-%EC%B9%98%ED%99%98-%EC%9B%90%EC%B9%99 "바 디자인패턴- LSP : 리스코프 치환 원칙") <br/>
**!Tip2.** [리스코프 치환 원칙 예제](https://sas-study.tistory.com/438 "리스코프 치환 원칙 예제")

##### 클래스간의 관계 - 포함관계

참고 - [](https://feastforall.tistory.com/32)

##### 클래스간의 관계 결정하기


##### 단일상속(single inheritance)


##### Object클래스 - 모든 클래스의 조상


## 오버라이딩(overriding)

##### 오버라이딩이란?

##### 오버라이딩의 조건

##### 오버로딩 vs. 오버라이딩

##### super

##### super() - 조상 클래스의 생성자


##

#####

#####


##

#####

#####
