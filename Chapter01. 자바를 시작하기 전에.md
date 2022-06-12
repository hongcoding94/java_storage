# Chapter01. 자바를 시작하기 전에

## 목차
1. [자바(Java Programming Language)](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94java-programming-language "자바(Java Programming Language)")
   - [자바란 무엇인가?](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80 "자바란 무엇인가?")
   - [자바 버전의 역사](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94-%EB%B2%84%EC%A0%84%EC%9D%98-%EC%97%AD%EC%82%AC "자바 버전의 역사")
   - [자바언어의 특징](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EC%96%B8%EC%96%B4%EC%9D%98-%ED%8A%B9%EC%A7%95 "자바언어의 특징")
   - [JVM(Java Virtual Machine)](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#jvmjava-virtual-machine "JVM(Java Virtual Machine)")
2. [자바개발환경 구축하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EA%B0%9C%EB%B0%9C%ED%99%98%EA%B2%BD-%EA%B5%AC%EC%B6%95%ED%95%98%EA%B8%B0 "자바개발환경 구축하기")
   - [JDK 설치](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#1-jdk-%EC%84%A4%EC%B9%98 "JDK 설치")
   - [Eclipse 설치](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#2-eclipse-%EC%84%A4%EC%B9%98 "Eclipse 설치")
4. [자바로 프로그램 작성하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EB%A1%9C-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EC%9E%91%EC%84%B1%ED%95%98%EA%B8%B0 "자바로 프로그램 작성하기")
   - [Eclipse or STS에서 Hello, World](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#1-eclipse-or-sts%EC%97%90%EC%84%9C-hello-world "Eclipse or STS에서 Hello, World")
5. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")

---
### 자바(Java Programming Language)
#### 자바란 무엇인가?
1. 자바는 객체지향 언어
    - 객체지향 프로그래밍이란 프로그램을 개발하는 기법 
        - 객체 생성 -> 조립 -> 연결 -> 모듈 or 프로그램 
    - 객체 생성을 위한 클래스를 작성한다.
    - 객체지향 언어의 특징 **캡슐화**, **상속성**, **다향성**을 완벽하게 지원

2. 이식성 ↑
    - 자바 실행환경(JRE) 설치가 되어 있는 모든 운영체제에서 실행이 가능하다.

3. 인터프린터 언어
    - 컴파일 언어이며 동시에 인터프리터 언어
    - 컴파일 언어에 가까운 속도와 시스템 독립성

4. 메모리 자동 관리
    - 개발자가 직접 메모리 접근을 할 수 없으며 자바가 직접 관리 (Tip0. JVM이란 내용 참조하기)
    - 객체 생성시 자동으로 메모리 영역 할당하며 사용 이후 GC(Garbage Collector)가 자동으로 불필요 객체를 제거 

5. 멀티 스레드 구현 esay
    - 운영체제에 따라 멀티 스레드를 구현하는 방법이 다름
    - 스레드 생성 및 제어와 관련된 라이브러리 API를 제공 때문에 운영체제 상관없이 멀티 스레드 쉽게 구현 가능
      - 라이브러리 API → [클릭](https://docs.oracle.com/javase/7/docs/api/ "클릭")
        
6. 동적 로딩을 지원
    - 필요한 시점에 클래스를 로딩하여 사용가능 즉. 전체 어플리케이션을 컴파일 하지 않아도 처리가 가능
    

**! Tip0.** JVM(Java Virtual Machine)
  - [참조0. JVM이란?](https://doozi0316.tistory.com/entry/1%EC%A3%BC%EC%B0%A8-JVM%EC%9D%80-%EB%AC%B4%EC%97%87%EC%9D%B4%EB%A9%B0-%EC%9E%90%EB%B0%94-%EC%BD%94%EB%93%9C%EB%8A%94-%EC%96%B4%EB%96%BB%EA%B2%8C-%EC%8B%A4%ED%96%89%ED%95%98%EB%8A%94-%EA%B2%83%EC%9D%B8%EA%B0%80 "JVM이란?")

### 자바 버전의 역사
> - JDK Beta (1995)
> - JDK 1.0 (1996)
> - JDK 1.1 (1997)
> - J2SE 1.2 (1998)
> - J2SE 1.3 (2000)
> - J2SE 1.4 (2002)
> - J2SE 5.0 (2004)
> - Java SE 6 (2006)
> - Java SE 7 (2011)
> - Java SE 8 (2014)

**! Tip1.** 자바의 1.7버전 이전(java SE7)과 아후(java SE8) 차이점
 - 자바 7 부터 지원되는 것들 
   - [java SE6] Pluggable Annotation
      - Lombok 등에서 사용되고 있다. (쉽게 말해 Annotation Processor 를 생각하면 된다.)
 - 자바 7 이후 지원되는 것들
    - [java SE7] try-with-resource 추가
    - [java SE7] 새로운 String 문자열 방법잉 도입
      ```java
      isBlank() : 문자열이 비거나 공백일 경우 true 반환
      lines() : 문자열을 줄 단위로 쪼개어 스트림 반환
      repeat(n) : 문자열에 대해 n번 반복하여 붙여 반환
        /*
        ex)
         - String str = "ABC";
         - String repeated = str.repeat(3); // "ABCABCABC"
         */
      stripLeading() : 문자열 앞 공백 제거
      stripTrailing() : 문자열 뒤 공백 제거
      strip() : 양쪽 공백 제거
      ```
    - [java SE7] 컴파일러가 타입을 추측할 수 있도록 지원
      ```java
      // Before Java 7
      ArrayList<Integer> arr = new ArrayList<Integer>();

      // In Java 7
      ArrayList<Integer> arr = new ArrayList<>();
      ```
   - [java SE8] Lambda

 - [참조1. java의 버전별 차이](https://velog.io/@ljo_0920/java-%EB%B2%84%EC%A0%84%EB%B3%84-%EC%B0%A8%EC%9D%B4-%ED%8A%B9%EC%A7%95 "java의 버전별 차이")

##### 자바언어의 특징

 - 객체 지향 프로그래밍(OOP - Object oriented Programming)
 > 객체지향프로그래밍의 대표적 특징은 **상속, 캡슐화(은닉), 다형성, 추상화** <br/>
 > 객체 지향 프로그래밍은 4가지 특징을 활용하여 코드의 재사용성을 증가 시키며 유지보수를 용이하게 만든다. <br/>
 >  - 상속 <br/>
 >  ▶ 부모 클래스의 변수와 메서드를 자식 클래스로 내려(상속) 받는 것 <br/>
 >  - 캡슐화 <br/>
 >  ▶ 객체의 변수 및 메서드를 외부 객체가 함부로 건드리지 못하게 감싸는 개념 (getter / setter) <br/>
 >  - 다형성 <br/>
 >  ▶ 같은 자료형에 여러가지 객체를 대입하여 다양한 결과를 얻어내는 성질 <br/>
   
   **Tip0.** [다형성의 자세한 응용 설명](https://reakwon.tistory.com/48 "다형성의 자세한 응용 설명")  <br/>

 >  - 추상화 <br/>
 >  ▶ 구체적인 사물들간의 공통점을 취하고 차이점을 버리는 일반화 즉, 불필요한 코드를 제거하고 중요한 부분을 추려내는 것

 - 자동 메모리 관리(GC)
 > JVM이 지속적으로 메모리를 감시하면서 더이상 사용되지 않는 메모리를 관리해 준다. <br/>
 > 다른 언어(C / C++)등의 경우 메모리는 개발자가 직접 메모리 관리를 처리해야하지만 Java의 경우   <br/>
 > **GC(Garbage Collection)을 통해 메모리 관리를 자동으로 수행**되기 때문에 개발자가 신경쓸 필요가 없다.  <br/>
 > 단, 개발자가 임의에 의해서 메모리를 관리 해야하는경우, **"System.gc();"** 로 GC를 호출하여 해제 할 수 있다.

 - 운영체제에 독립적
 > 자바의 개발 환경과 배포환경이 다를 경우, 프로그램을 다시 컴파일 할 필요 없이 실행가능함을 의미하며  <br/>
 > JVM에서 별도의 Java Compiler를 통해 사용자의 코드를 Byte 코드로 변환하기 때문이다.  <br/>
 > 즉. 모든 자바 프로그램은 이론적으로 CPU나 운영체제의 종류와 무관하게 동일하게 동작한다.

 - 멀티쓰레드 지원
 >  - 멀티쓰레드란?  <br/>
 >  ▶ 하나의 프로세스를 다수의 실행 단위로 구분하고 자원을 공유하고 자원의 생성과 관리의 중복성을 최소화하여  <br/>
 >  &nbsp; &nbsp; &nbsp; 수행 능력을 향상시키는 것을 멀티 쓰레드이라고 한다. <br/>
 >  &nbsp; &nbsp; &nbsp; 즉, 하나의 프로그램에 동시에 여러개의 일을 수행할 수 있도록 도와준다.
 >  - 멀티쓰레드 구현 방식
 >     - Thread 클래스(화이트 방식)
 >     - Runnable 인터페이스(블랙박스 방식)

 **!Tip1.** [멀티쓰레드 자세한 설명](https://goodgid.github.io/What-is-Multi-Thread/ "멀티쓰레드 자세한 설명")

 - 동적 로딩 지원
 > ?? 밍>?

**!Tip2.** [동적 로딩, 정적 로딩, static 키워드](https://ubange.tistory.com/223 "동적 로딩, 정적 로딩, static 키워드") <br/>
**!Tip3.** [심화 : 동적 로딩](https://velog.io/@shlee7131/Java-%EB%B2%88%EC%99%B8-%EB%8F%99%EC%A0%81-%EB%A1%9C%EB%94%A9 "심화 : 동적 로딩") 

##### JVM(Java Virtual Machine)

- JVM이란?
> Java Virtual Machine은 OS에 종속 받지 않고 CPU가 Java를 실행 시키기 위해서 가상 컴퓨터이다. 
> 
![컴파일 과정](https://user-images.githubusercontent.com/66407386/170973677-857268ef-5770-4b7f-85db-f2f1320568ba.png "컴파일 과정")
<br/>

![JVM 구성요소](https://user-images.githubusercontent.com/66407386/170974326-23a25d45-09fb-40d9-b131-383378c6c367.png "JVM 구성요소")

**!Tip4.** [JVM은 무엇이며 자바 코드는 어떻게 실행하는 것인가](https://doozi0316.tistory.com/entry/1%EC%A3%BC%EC%B0%A8-JVM%EC%9D%80-%EB%AC%B4%EC%97%87%EC%9D%B4%EB%A9%B0-%EC%9E%90%EB%B0%94-%EC%BD%94%EB%93%9C%EB%8A%94-%EC%96%B4%EB%96%BB%EA%B2%8C-%EC%8B%A4%ED%96%89%ED%95%98%EB%8A%94-%EA%B2%83%EC%9D%B8%EA%B0%80 "JVM은 무엇이며 자바 코드는 어떻게 실행하는 것인가")
 
## 자바개발환경 구축하기

### 1. JDK 설치
![JDK 환경변수](https://user-images.githubusercontent.com/66407386/170052007-a72c361e-2bca-468d-9cb1-c48e7e2ed74f.png)

### 2. Eclipse 설치

![Eclipse 설치](https://user-images.githubusercontent.com/66407386/170057550-78dca0b8-df57-4d72-a334-8789c0e1919e.png)



**! Tip2.** 새로운 프로젝트 생성방법)
  - [참조2. 새로운 프로젝트 생성방법](https://i-am-seongni.tistory.com/18 "새로운 프로젝트 생성방법")


## 자바로 프로그램 작성하기


### 1. Eclipse or STS에서 Hello, World
   > #### Hello, World
   > ```java
   > package hello.helloworld.java
   > 
   > public class helloworld() {
   >    public static void main(String[] args) {
   >       System.out.println("Hello, World");
   >    }
   > }
   > ```
   > #### 결과물
   > ![Hello, world](https://user-images.githubusercontent.com/66407386/170055145-7fbfaf35-ebaf-4e83-9513-b6a99049970e.png)

---
## 참고 문서 / 블로그
0. [서적] 남궁성님의 Java의 정석 3rd Edition 
1. [블로그] 재밌는 Coding 하기님의 윈도우 JDK(Java Development Kit) 설치 - https://hyuntaekhong.github.io/blog/install-JDK/ <br/>
2. [블로그] pinggoopark님의 이클립스 설치하기 - https://pinggoopark.tistory.com/44
