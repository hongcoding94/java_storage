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

 **!Tip0.** [익명 클래스](https://mommoo.tistory.com/16)<br />
 **!Tip1.** [익명 객체](https://velog.io/@yeonnex/%EC%9E%90%EB%B0%94%EC%97%90%EC%84%9C-%EB%9E%8C%EB%8B%A4%EC%8B%9D%EC%9D%80-%EC%9D%B5%EB%AA%85%ED%95%A8%EC%88%98-%EC%9D%B5%EB%AA%85%EA%B0%9D%EC%B2%B4)<br />
 
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

 - 람다식 사용법
 > ```java
 > (매개변수, ...) -> { 실행문 ... }
 > ```

 - 람다식 사용 예제
 >    - 예제 
 >    ```java
 >    @FunctionalInterface
 >    interface Say{
 >        int someting(int a,int b);
 >    }
 >    class Person{
 >        public void hi(Say line) {
 >    	      int number = line.someting(3,4);
 >    	      System.out.println("Number is "+number);
 >        }
 >    }
 >    ```
 >    
 >    - 람다식 사용 안했을 때
 >    ```java
 >    Person rin = new Person();
 >    rin.hi(new Say() {
 >        public int someting(int a, int b) {
 >          System.out.println("My Name is Coding-Factory");
 >          System.out.println("Nice to meet you");
 >          System.out.println("parameter number is "+a+","+b);
 >          return 7;
 >        }
 >    });
 >    ```
 >    
 >    - 람다식 사용했을 때
 >    ```java
 >    Person rin = new Person();
 >    rin.hi((a,b) ->{
 >        System.out.println("This is Coding-Factory!");
 >        System.out.println("Tank you Lamda");
 >    	  System.out.println("parameter number is "+a+","+b);
 >        return 7;
 >    });
 >    ```
 >    
 >    ```출력 결과
 >    This is Coding-Factory!
 >    Tank you Lamda
 >    parameter number is 3, 4
 >    Number is 7
 >    ```

- 람다식의 장단점
>   - 장점
>     1. 코드를 간결하게 작성가능
>     2. 코드가 간결하며 개발자의 의도가 명확히 들어나며 가독성이 향상
>     3. 함수를 만드는 과정없이 한번에 처리 할 수 있기 때문에 코딩 작성 소요시간이 줄어든다.
>     4. 병렬프로그래밍이 용이
>     
>   - 단점
>     1. 람다를 사용하면서 만드는 무명함수는 재사용이 불가
>     2. 디버깅이 다소 어렵다.
>     3. 람다를 남발하면 코드의 가독성이 불가능하며 중복생성 가능이 매우 높음
>     4. 재귀로 만들 경우에 다소 부적합한면이 있음

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

 - Function의 합성과 Predicate의 결합
 > ```java
 > public class Main() {
 >  public static void main(String[] args) {
 >    Predicate<Integer> p = i -> i < 100;
 >    Predicate<Integer> q = i -> i < 200;
 >    Predicate<Integer> r = i -> i % 2 == 0;
 >    Predicate<Integer> notP = p.negate();	//i >= 100
 >    
 >    // 100 <= i && (i < 200 || i % 2 == 0)
 >    Predicate<Integer> all = notP.and(q.or(r));
 >    System.out.println(all.test(150));	//true
 >  }
 > }
 > ```
 >  - 이처럼 and(), or(), negate()로 여러 조건식을 하나로 합칠 수 있다.

##### 메서드 참조

 - 메소드 참조(Method References)란?
 > 이미 존재하는 이름을 가진 메소드를 람다로 사용하도록 참조<br />
 > 즉, 일반 함수를 람다 형태로 사용할 수 있도록 해준다. 또한 메소드를 호출(실행)하는 것이 아니라 참조만<br />
 > 하기 때문에, 이름 뒤에 소괄호는 쓰지 않는다.

 - 메서드 참조 방법
 > ```text
 > '클래스 이름::메서드 이름' 또는 '참조변수::메서드 이름'으로 바꿀 수 있다. 
 > ```
  
 - 생성자의 메서드 참조
 > 생성자를 호출하는 람다식 메서드 참조로 변환할 수 있다? 없다? / ⭕ - 있다.<br />
 > **매개변수가 있는 생성자라면** 매개변수의 개수에 따라 알맞은 함수형 인터페이스를 사용하면 되며<br />
 > 필요하다면 함수형 인터페이스를 새로 정의해야한다. <br /> <br />
 > ✔️ : 메서드 참조는 람다식을 static변수처럼 다룰 수 있게 해준다. **텍스트** or **코드 압축**로 사용한다.
  
## 스트림(stream)

##### 스트림이란?

 - 스트림이란?
 > 스트림과 람다를 활용하여 이전보다 간결하고 향상된 방법으로 collection으로 처리한다.<br />
 > 순차(sequential), 병렬(parallel) 두 종류가 존재<br />
 > 순차 stream은 싱글 쓰레드가 순차적으로 처리되며 병렬 stream은 fork/join 프레임워크로 <br />
 > 메서들에 의해 병렬로 처리된다.

##### 스트림 만들기

 - 스트림 만들기
 > ```java
 > import java.util.ArrayList;
 > import java.util.Iterator;
 >
 > public class Main {
 > 	public static void main(String[] args) {
 > 		// 일반적인 방식
 > 		List<String> list1 = Arrays.asList("공무원", "경찰", "검찰", "조사관");
 > 		Iterator<String> iterator = list1.iterator();
 > 		while(iterator.hasNext()) {
 > 			String job = iterator.next();
 > 			System.out.println(job);
 > 		}
 > 
 > 		// Stream 사용
 > 		List<String> list2 = Arrays.asList("공무원", "경찰", "검찰", "조사관");
 > 		Stream<String> ns = list2.stream();
 > 		stream.forEach ( ns -> System.out.println(ns) );
 > 	}
 > }
 > ```
 >	- Stream이 제공하는 대부분의 요소 처리 메소드는 함수적 인터페이스 매개 타입을 가지기<br />
 >        때문에 람다식 또는 메소드 참조를 이용해서 요소 처리 내용을 매개값으로 전달
 >      - 내부 반복자를 사용하므로 병렬 처리가 가능하다.

 - 내부 반복자와 외부 반복자란?
 > 내부 반복자<br />
 >  ➡️ 개발자가 코드로 직접 컬렉션의 요소를 반복해서 가져오는 코드패턴<br /><br />
 > 외부 반복자<br />
 >  ➡️ 컬렉션 배부에서 요소들을 반복시키며, 개발자는 요소당 처리해야 할 코드만 제공하는 코드 패턴<br />
 > &nbsp; &nbsp; &nbsp;즉, 먼티 코어 CPU를 최대한 활용하기 위해 요소들을 분배시켜 병렬 작업을 할 수 있도록<br />
 > &nbsp; &nbsp; &nbsp;효율적으로 요소를 반복시킨다.

##### 스트림 중간연산

 - 중간 연산자 : 필터링 및 맵핑등 원하는 결과만 보여주는 **중간 작업**
 <table>
  <tr>
   <th>연산</th>
   <th>변환값</th>
   <th>연산 인수</th>
   <th>함수 디스크립터</th>
   <th>설명</th>
  </tr>
  <tr>
    <td>filter</td>
    <td>Stream<T></td>
    <td>Predicate<T></td>
    <td>T -> blooean</td>
    <td>조건에 안 맞는 요소 제외</td>
  </tr>
  <tr>
    <td>map</td>
    <td>Stream<T></td>
    <td>Function<T,R></td>
    <td>T -> R</td>
    <td> </td>
  </tr>
  <tr>
    <td>limit</td>
    <td>Stream<T></td>
    <td> </td>
    <td> </td>
    <td>스트림의 일부를 잘라냄</td>
  </tr>
  <tr>
    <td>sorted</td>
    <td>Stream<T></td>
    <td>Comparator<T></td>
    <td>(T,T) -> int</td>
    <td>스트림의 요소를 정렬</td>
  </tr>
  <tr>
    <td>distinct</td>
    <td>Stream<T></td>
    <td> </td>
    <td>중복을 제거</td>
    <td> </td>
  </tr>
 </table>

 **중간 연산은 map()과 FlatMap()이 많이 사용된다.**
  
 **Tip4.** [스트림의 중간연산자 총정리](https://jamie95.tistory.com/54)<br />
 **Tip5.** [스트림 중간연산자 예제(filter 메서드)](https://dev-kani.tistory.com/28)<br />
 **Tip6.** [스트림 중간연산자 예제(distinct 메서드)](https://dev-kani.tistory.com/29?category=805336)<br />
 **Tip7.** [스트림을 이용한 가독성 좋은 코드](https://jeong-pro.tistory.com/165)

##### Optional〈T〉와 OptionalInt
  
  - Optional〈T〉와 OptionalInt
  > java.util.Optional은 JDK1.8 추가 되었으며 Optional<T\>은 지네릭 클래스로 "T타입의 객체"를 감싸는 ***래퍼 클래스***<br />
  > 때문에 Optional타입의 객체는 모든 타입의 참조변수를 담을 수 있다.<br />
  >    - 예시
  >    >```java
  >    > public final class optional<T> {
  >    >  private final T value;  // T타입의 참조변수
  >    >  // ...
  >    > }
  >    > ```
  >    > <br />
  >    > Optional 객체에 담아서 반환하며 매번 반복된 결과를 체크하지 않고 Optional에 정의된 메서드를 통해서<br />
  >    > 간단하게 처리가 가능하며 if문을 사용하지 않고 NullPoniterException이 발생하지 않는 코드를 작성 할 수 있다.
  
##### 스트림의 최종연산

  - 최종 연산 : 최종적으로 결과를 생성하는 작업
    <table>
      <tr>
        <th>최종연산의 종류</th>
        <th>역할</th>
        <th>메소드</th>
      </tr>
      <tr>
        <td>Calculating</td>
        <td>요소의 통계 및 연산</td>
        <td>sum(), count(), min(), max(), average()</td>
      </tr>
      <tr>
        <td>Reduction</td>
        <td>요소의 소모</td>
        <td>reduce()</td>
      </tr>
      <tr>
        <td>Collecting</td>
        <td>요소의 수집</td>
        <td>collect()</td>
      </tr>
      <tr>
        <td>Matching</td>
        <td>요소의 검사</td>
        <td>anyMatch(), allMatch(), noneMatch()</td>
      </tr>
      <tr>
        <td>Searching</td>
        <td>요소의 검색</td>
        <td>findFirst(), findAny()</td>
      </tr>
      <tr>
        <td>Iterating</td>
        <td>요소의 출력</td>
        <td>forEach()</td>
      </tr>
    </table>
  
  **!Tip8.** [최종연산 예제](https://choonsik-lab.tistory.com/94)
  
##### collect()
  
  

##### Collector구현하기
  
  

##### 스트림의 변환
  
  

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [포럼] [이종우님의 Java8 람다](https://www.slideshare.net/rheehot1/java8-57541617)
3. [블로그] [동현 유님의 람다와 스트림](https://letsmakemyselfprogrammer.tistory.com/105)
4. [블로그] [책 읽는 개발자_테드님의 [Java]람다(Lambda)와 java.util.function패키지](https://scshim.tistory.com/73)
5. [블로그] [ryan-han님의 자바의 정석 - 람다식(Lambda Expression)](https://ryan-han.com/post/java/java-lambda/)
6. [블로그] [qkrdmstn1014님의 Java의 정석 - chapter 14](https://velog.io/@qkrdmstn1014/Java%EC%9D%98-%EC%A0%95%EC%84%9D-chapter-14)
7. [포럼] [최범균님의 자바8 스트림API에 대해서](https://www.slideshare.net/madvirus/8-api)
8. [블로그] [injoon2019님의 자바-OptionalT와-OptionalInt](https://velog.io/@injoon2019/%EC%9E%90%EB%B0%94-OptionalT%EC%99%80-OptionalInt)
9. [홈페이지] [CodeJava의 terminal Operation Stream](https://www.codejava.net/java-core/collections/java-8-stream-terminal-operations-examples)
