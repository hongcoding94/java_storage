# Chapter14. 람다와 스트림

## 목차
1. [람다식](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EB%9E%8C%EB%8B%A4%EC%8B%9D)
  	- [1-1. 람다식이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EB%9E%8C%EB%8B%A4%EC%8B%9D%EC%9D%B4%EB%9E%80)
  	- [1-2. 람다식 작성하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EB%9E%8C%EB%8B%A4%EC%8B%9D-%EC%9E%91%EC%84%B1%ED%95%98%EA%B8%B0)
  	- [1-3. 함수형 인터페이스(Functional Interface)]()
  	- [1-4. java.util.function 패키지](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#javautilfunction-%ED%8C%A8%ED%82%A4%EC%A7%80)
  	- [1-5. Function의 합성과 Predicate의 결합](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#function%EC%9D%98-%ED%95%A9%EC%84%B1%EA%B3%BC-predicate%EC%9D%98-%EA%B2%B0%ED%95%A9)
  	- [1-6. 메서드 참조](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EB%A9%94%EC%84%9C%EB%93%9C-%EC%B0%B8%EC%A1%B0)
2. [스트림(stream)](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%8A%A4%ED%8A%B8%EB%A6%BCstream)
  	- [2-1. 스트림이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%8A%A4%ED%8A%B8%EB%A6%BC%EC%9D%B4%EB%9E%80)
  	- [2-2. 스트림 만들기](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%8A%A4%ED%8A%B8%EB%A6%BC-%EB%A7%8C%EB%93%A4%EA%B8%B0)
  	- [2-3. 스트림 중간연산](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%8A%A4%ED%8A%B8%EB%A6%BC-%EC%A4%91%EA%B0%84%EC%97%B0%EC%82%B0)
  	- [2-4. Optional〈T〉와 OptionalInt](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#optionalt%EC%99%80-optionalint)
  	- [2-5. 스트림의 최종연산](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%8A%A4%ED%8A%B8%EB%A6%BC%EC%9D%98-%EC%B5%9C%EC%A2%85%EC%97%B0%EC%82%B0)
  	- [2-6. collect()](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#collect)
 	- [2-7. Collector구현하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#collector%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0)
  	- [2-8. 스트림의 변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%8A%A4%ED%8A%B8%EB%A6%BC%EC%9D%98-%EB%B3%80%ED%99%98)
3. [참고문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter14.%20%EB%9E%8C%EB%8B%A4%EC%99%80%20%EC%8A%A4%ED%8A%B8%EB%A6%BC.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8)

## 람다식

##### 람다식이란?
 - 람다식이란? 
 > 함수명을 선언하고 사용하는 것이 아닌 식별자 없이 실행 가능한 함수
 > 절차형 프로그래밍, 객체지향 프로그래밍과는 사뭇 다르게 함수의 구현과 호출만으로 프로그램을 만드는 방식인 함수형
   프로그래밍에서 자주 사용
 > 자바 8부터 지원하며 람다식을 익명<s>함수</s>(객체)를 만드는 것인데 **익명함수**는 일급 객체 특징을 가지고 있다.
 >  - 익명 <s>함수</s>객체(anonymous function) : 익명함수라고 부르지만 자바에서는 함수가 혼자 존재 할 수 없기<br/>
 >                                              때문에 익명 객체라고 맞는 표현이다. 
 >  - 익명 객체를 쓰는 이유 : 한시적(일시적)으로 사용하며 후에 재사용이 되지 않는다.<br />
 >                          즉, 프로그램에서 일시적으로 한번만 사용되고 버려지는 객체라 생각하면 편하다.<br/>
 >                          때문에 재사용성이 없으며 확장성을 활용하는 것이 유지보수에 안 좋을 때 사용하는 것이다. 

 **!Tip0.** [익명 클래스](https://mommoo.tistory.com/16)
 **!Tip1.** [익명 객체](https://velog.io/@yeonnex/%EC%9E%90%EB%B0%94%EC%97%90%EC%84%9C-%EB%9E%8C%EB%8B%A4%EC%8B%9D%EC%9D%80-%EC%9D%B5%EB%AA%85%ED%95%A8%EC%88%98-%EC%9D%B5%EB%AA%85%EA%B0%9D%EC%B2%B4)
 
 - 람다식 문법 
 > ```java
 > (매개변수목록) -> {실행문}
 > 
 > // 예시
 > public interface Compare {
 >  public int compareTo(int value1, int value2);
 > }
 > 
 > public class CompareExam {
 >    public static void exec(Compara compara) {
 >      int i = 10;
 >      int k = 20;
 >      int value = compara.compareTo(i, k);
 >      
 >      System.out.println(value);
 >    }
 >    
 >    public static void main(String[] args) {
 >      exec((i, k) -> {
 >        return k - k;
 >      });
 >    }
 > }
 > ```

##### 람다식 작성하기

##### 함수형 인터페이스(Functional Interface)

 - 함수형 인터페이스(functional interface)란?
 > 1개의 추상 메소드를 갖고 있는 인터페이스를 지칭한다. 현업에서 SAM(Single Abstract Method)으로 이야기한다.

 - 함수형 인터페이스를 사용하는 이유
 > 

 - 기본 함수형 인터페이스 및 설명 그리고 예제
 > A. Runnable : 인자를 받지 않고 리턴 값도 없는 인터페이스,<br/>
 > B. Supplier : 인자를 받지 않고 T타입의 객체를 리턴<br/>
 > C. Consumer : T타입의 객체를 인자로 받고 리턴 값이 없음<br/>
 > D. Function<T[함수에 대한 입력 유형], R[함수 결과의 유형]> : T타입의 인자를 받고, R타입의 객체를 반환<br/>
 > E. Predicate : T타입 인자를 받고 결과로 Boolean<true, false>으로 리턴<br/>

##### java.util.function 패키지

- 람다와 jav.util.function패키지의 어떠한 연관성?
> 위에서 말했듯 람다식을 다루기 위한 인터페이스를 함수형 인터페이스라 말하지만 function 패키지에 일반적으로<br/>
> 자주 쓰이는 형식의 메서드를 함수형 인터페이스로 미리 정의 했기 때문이다.

- function 패키지를 사용하는 이유
> 1. 함수형 인터페이스를 계속 정의 하지 않고 재사용이 가능하다.
> 2. 메서드의 타입이 비슷하다. 제네릭 메서드로 정의하면 매개변수나 반환타입이 달라도 문제가 되지 않는다.
> 3. 함수형 인터페이스에 정의된 메서드 이름이 통일되고, 재사용성이나 유지보수에도 좋다.

**!Tip3.**[java.util.function 패키지가 제공하는 메소드 정리](https://javaplant.tistory.com/34)
 
##### Function의 합성과 Predicate의 결합

 - Predicate란?
 > argument를 받아 Bollean값을 반환하는 함수형 인터페이스
 >  ➡️ 향후 예제 만들어 보기

 - Founction과 Predicate를 

 - Function의 합성과 Predicate의 결합

##### 메서드 참조

 - 메소드 참조(Method References)란?
 > 이미 존재하는 이름을 가진 메소드를 람다로 사용하도록 참조<br />
 > 즉, 일반 함수를 람다 형태로 사용할 수 있도록 해준다. 또한 메소드를 호출(실행)하는 것이 아니라 참조만<br />
 > 하기 때문에, 이름 뒤에 소괄호는 쓰지 않는다.

 - 메서드 참조 방법
 >

## 스트림(stream)

##### 스트림이란?

 - 스트림이란?
 > 스트림과 람다를 활용하여 이전보다 간결하고 향상된 방법으로 collection으로 처리한다.<br />
 > 순차(sequential), 병렬(parallel) 두 종류가 존재<br />
 > 순차 stream은 싱글 쓰레드가 순차적으로 처리되며 병렬 stream은 fork/join 프레임워크로 <br />
 > 메서들에 의해 병렬로 처리된다.

##### 스트림 만들기

##### 스트림 중간연산

##### Optional〈T〉와 OptionalInt

##### 스트림의 최종연산

##### collect()

##### Collector구현하기

##### 스트림의 변환

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [블로그] [동현 유님의 람다와 스트림](https://letsmakemyselfprogrammer.tistory.com/105)
3. [블로그] [책 읽는 개발자_테드님의 [Java]람다(Lambda)와 java.util.function패키지](https://scshim.tistory.com/73)
4. [블로그] [ryan-han님의 자바의 정석 - 람다식(Lambda Expression)](https://ryan-han.com/post/java/java-lambda/)
