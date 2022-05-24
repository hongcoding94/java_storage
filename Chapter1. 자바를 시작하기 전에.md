# Chapter1. 자바를 시작하기 전에

1. [자바(Java Programming Language)](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94java-programming-language "자바(Java Programming Language)")
   - [자바란 무엇인가?](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80 "자바란 무엇인가?")
   - [자바 버전업 역사](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94-%EB%B2%84%EC%A0%84%EC%97%85-%EC%97%AD%EC%82%AC "자바 버전업 역사")
2. [자바개발환경 구축하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EA%B0%9C%EB%B0%9C%ED%99%98%EA%B2%BD-%EA%B5%AC%EC%B6%95%ED%95%98%EA%B8%B0 "자바개발환경 구축하기")
3. [자바로 프로그램 작성하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter1.%20%EC%9E%90%EB%B0%94%EB%A5%BC%20%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md#%EC%9E%90%EB%B0%94%EB%A1%9C-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EC%9E%91%EC%84%B1%ED%95%98%EA%B8%B0 "자바로 프로그램 작성하기")

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

### 자바 버전업 역사
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

## 자바개발환경 구축하기

1. JDK 설치

 ![alt JDK 설치] (/66407386/170048744-6e764072-adb6-4f27-ad45-956437f46f60.png)


2. 



## 자바로 프로그램 작성하기
