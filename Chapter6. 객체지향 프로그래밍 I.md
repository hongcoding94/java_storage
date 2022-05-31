# Chapter6. 객체지향 프로그래밍 I

## 목차

1. [객체지향언어](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%EC%96%B8%EC%96%B4 "객체지향언어")
    - [1-1. 객체지향언어의 역사](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%EC%96%B8%EC%96%B4%EC%9D%98-%EC%97%AD%EC%82%AC "객체지향언어의 역사")
    - [1-2. 객체지향언어](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%EC%96%B8%EC%96%B4-1 "객체지향언어")
2. [클래스와 객체](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EC%99%80-%EA%B0%9D%EC%B2%B4 "클래스와 객체")
    - [2-1. 클래스와 객체의 정의와 용도](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EC%99%80-%EA%B0%9D%EC%B2%B4%EC%9D%98-%EC%A0%95%EC%9D%98%EC%99%80-%EC%9A%A9%EB%8F%84 "클래스와 객체의 정의와 용도")
    - [2-2. 객체와 인스턴스](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%9D%EC%B2%B4%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4 "객체와 인스턴스")
    - [2-3. 객체의 구성요소 - 속성과 기능](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%9D%EC%B2%B4%EC%9D%98-%EA%B5%AC%EC%84%B1%EC%9A%94%EC%86%8C---%EC%86%8D%EC%84%B1%EA%B3%BC-%EA%B8%B0%EB%8A%A5 "객체의 구성요소 - 속성과 기능")
    - [2-4. 인스턴스의 생성과 사용](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EC%9D%98-%EC%83%9D%EC%84%B1%EA%B3%BC-%EC%82%AC%EC%9A%A9 "인스턴스의 생성과 사용")
    - [2-5. 객체 배열](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%9D%EC%B2%B4-%EB%B0%B0%EC%97%B4 "객체 배열")
3. [변수와 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%B3%80%EC%88%98%EC%99%80-%EB%A9%94%EC%84%9C%EB%93%9C "변수와 메서드")
    - [3-1. 선언위치에 따른 변수의 종류](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%84%A0%EC%96%B8%EC%9C%84%EC%B9%98%EC%97%90-%EB%94%B0%EB%A5%B8-%EB%B3%80%EC%88%98%EC%9D%98-%EC%A2%85%EB%A5%98 "선언위치에 따른 변수의 종류")
    - [3-2. 클래스변수와 인스턴스변수](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EB%B3%80%EC%88%98%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EB%B3%80%EC%88%98 "클래스변수와 인스턴스변수")
    - [3-3. 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%A9%94%EC%84%9C%EB%93%9C "메서드")
    - [3-4. 메서드의 선언과 구현](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%A9%94%EC%84%9C%EB%93%9C%EC%9D%98-%EC%84%A0%EC%96%B8%EA%B3%BC-%EA%B5%AC%ED%98%84 "메서드의 선언과 구현")
    - [3-5. 메서드의 호출](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%A9%94%EC%84%9C%EB%93%9C%EC%9D%98-%ED%98%B8%EC%B6%9C "메서드의 호출")
    - [3-6. return문](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#return%EB%AC%B8 "return문")
    - [3-7. JVM의 메모리구조](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#jvm%EC%9D%98-%EB%A9%94%EB%AA%A8%EB%A6%AC%EA%B5%AC%EC%A1%B0 "JVM의 메모리구조")
    - [3-8. 기본형 매개변수와 참조형 매개변수](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B8%B0%EB%B3%B8%ED%98%95-%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98%EC%99%80-%EC%B0%B8%EC%A1%B0%ED%98%95-%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98 "기본형 매개변수와 참조형 매개변수")
    - [3-9. 참조형 반환타입](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%B0%B8%EC%A1%B0%ED%98%95-%EB%B0%98%ED%99%98%ED%83%80%EC%9E%85 "참조형 반환타입")
    - [3-10. 재귀호출(recursive call)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%9E%AC%EA%B7%80%ED%98%B8%EC%B6%9Crecursive-call "재귀호출(recursive call)")
    - [3-11. 클래스 메서드(static메서드)와 인스턴스 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%ED%81%B4%EB%9E%98%EC%8A%A4-%EB%A9%94%EC%84%9C%EB%93%9Cstatic%EB%A9%94%EC%84%9C%EB%93%9C%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4-%EB%A9%94%EC%84%9C%EB%93%9C "클래스 메서드(static메서드)와 인스턴스 메서드")
    - [3-12. 클래스 멤버와 인스턴스 멤버간의 참조와 호출](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%ED%81%B4%EB%9E%98%EC%8A%A4-%EB%A9%A4%EB%B2%84%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4-%EB%A9%A4%EB%B2%84%EA%B0%84%EC%9D%98-%EC%B0%B8%EC%A1%B0%EC%99%80-%ED%98%B8%EC%B6%9C "클래스 멤버와 인스턴스 멤버간의 참조와 호출")
4. [오버로딩(overloading)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9overloading "오버로딩(overloading)")
    - [4-1. 오버로딩이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%B4%EB%9E%80 "오버로딩이란?")
    - [4-2. 오버로딩의 조건](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%98-%EC%A1%B0%EA%B1%B4 "오버로딩의 조건")
    - [4-3. 오버로딩의 예](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%98-%EC%98%88 "오버로딩의 예")
    - [4-4. 오버로딩의 장점](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%98-%EC%9E%A5%EC%A0%90 "오버로딩의 장점")
    - [4-5. 가변인자(varargs)와 오버로딩](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B0%80%EB%B3%80%EC%9D%B8%EC%9E%90varargs%EC%99%80-%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9 "가변인자(varargs)와 오버로딩")
5. [생성자(constructor)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%83%9D%EC%84%B1%EC%9E%90constructor "생성자(constructor)")
    - [5-1. 생성자란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%83%9D%EC%84%B1%EC%9E%90%EB%9E%80 "생성자란?")
    - [5-2. 기본 생성자(default constructor) ](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EA%B8%B0%EB%B3%B8-%EC%83%9D%EC%84%B1%EC%9E%90default-constructor "기본 생성자(default constructor) ")
    - [5-3. 매개변수가 있는 생성자](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98%EA%B0%80-%EC%9E%88%EB%8A%94-%EC%83%9D%EC%84%B1%EC%9E%90 "매개변수가 있는 생성자")
    - [5-4. 생성자에서 다른 생성자 호출하기 - this(), this](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%83%9D%EC%84%B1%EC%9E%90%EC%97%90%EC%84%9C-%EB%8B%A4%EB%A5%B8-%EC%83%9D%EC%84%B1%EC%9E%90-%ED%98%B8%EC%B6%9C%ED%95%98%EA%B8%B0---this-this "생성자에서 다른 생성자 호출하기 - this(), this")
    - [5-5. 생성자를 이용한 인스턴스의 복사](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%83%9D%EC%84%B1%EC%9E%90%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EC%9D%98-%EB%B3%B5%EC%82%AC "생성자를 이용한 인스턴스의 복사")
6. [변수의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%B3%80%EC%88%98%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94 "변수의 초기화")
    - [6-1. 변수의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%B3%80%EC%88%98%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94-1 "변수의 초기화")
    - [6-2. 명시적 초기화(explicit initialization)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%AA%85%EC%8B%9C%EC%A0%81-%EC%B4%88%EA%B8%B0%ED%99%94explicit-initialization "명시적 초기화(explicit initialization)")
    - [6-3. 초기화 블럭(initialization block)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EC%B4%88%EA%B8%B0%ED%99%94-%EB%B8%94%EB%9F%ADinitialization-block "초기화 블럭(initialization block)")
    - [6-4. 멤버변수의 초기화 시기와 순서](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I.md#%EB%A9%A4%EB%B2%84%EB%B3%80%EC%88%98%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94-%EC%8B%9C%EA%B8%B0%EC%99%80-%EC%88%9C%EC%84%9C "멤버변수의 초기화 시기와 순서")

---
## 객체지향언어

  ##### 객체지향언어의 역사
  
  
  ##### 객체지향언어
  
   - 객체지향언의 주요 특징
   > - 코드의 재사용성이 높다.<br/>
   >  ▶ 새로운 코드를 작성할 때 기존의 코드를 이용하여 쉽게 작성할 수 있다.<br/>
   > 
   > - 코드의 관리가 용이하다.<br/>
   >  ▶ 코드간의 관계를 이용해서 적은 노력으로 쉽게 코드를 변경할 수 있다.<br/>
   > 
   > - 신뢰성이 높은 프로그래밍을 가능하게 한다.<br/>
   >  ▶ 제어자와 메서드를 이용해서 데이터를 보호하고 올바른 값을 유지하도록 하며,<br/> &nbsp; &nbsp; &nbsp; 코드의 중복을 제거하여 코드의 불일치로 인한 오동작을 방지할 수 있다.

## 클래스와 객체 
  
  ##### 클래스와 객체의 정의와 용도
  
  - 클래스와 객체의 개념 및 용도
  > - 클래스의 개념 <br/>
  >  ▶ 객체를 만들어 내기 위한 **종이 설계도 또는 프레임** <br/>
  >  ▶ 변수와 메서드의 집합
  > - 클래스의 용도 <br/>
  >  ▶ 클래스는 객체를 생성하는데 사용 <br/> <br/>
  > - 객체의 개념 <br/>
  >  ▶ 소프트웨어에서 구현할 대상 <br/>
  >  ▶ 클래스에 선언된 모양을 그대로 투상화 하는 것 <br/>
  > - 객체의 용도 <br/>
  >  ▶ 객체가 가지고 있는 기능과 속성에 따라 다름
  
  - 예시
  <table>
    <tr>
        <th>클래스 (제품설계도)</th>
        <th>객체 (제품)</th>
    </tr>
    <tr>
        <td>TV 설계도</td>
        <td>TV</td>
    </tr>
    <tr>
        <td>붕어빵 기계</td>
        <td>붕어빵</td>
    </tr>
  </table>
  
  ##### 객체와 인스턴스
  
  - 인스턴스의 개념과 용도
  > - 인스턴스의 개념 <br/>
  >  ▶ 설계도(클래스)를 바탕으로 **소프트웨어에서 구현된 구체적인 실체**<br/>
  > - 인스턴스의 용도 <br/>
  >  ▶ 인스턴스는 객체에 포함된다고 볼 수 있다.<br/> &nbsp; &nbsp; &nbsp; 즉, 객체를 소프트웨어에 실체화하면 인스턴스화라고 한다.<br/>
  >  ▶ 실체화된 인스턴스는 메모리에 할당된다.

  **!Tip0.** [클래스, 객체, 인스턴스의 차이](https://gmlwjd9405.github.io/2018/09/17/class-object-instance.html "클래스, 객체, 인스턴스의 차이")

  ##### 객체의 구성요소 - 속성과 기능
  
 -  객체의 구성 요소
 >    - 객체의 속성 <br/>
 >     ▶ 속성의 정의
 >          <br/> - 무에서 필요로 한다.
 >          <br/> - 의미상 더 이상 분리되지 않는다.
 >          <br/> - 엔터티를 설명하고 인스턴스의 구성요소가 된다.
 >    - 객체의 속성(Property) 종류
 >      - 멤버 변수(Member Variable)
 >      - 특성 (attribute)
 >      - 필드 (filed)
 >      - 상태 (state) 
 >    - 예시
 >      - 스마트폰의 구현도 - 크기, 길이, 높이, 색상, 해상도 등등
 >    ![객체의 속성](https://t1.daumcdn.net/cfile/tistory/25608F42589045692E)
 >     <br/>
 >    - 객체의 기능 <br/>
 >     ▶ 기능의 정의
 >          <br/> - 객체들이 각각 도 맡아서 코드를 수행 
 >    - 개체의 기능(Function) 종류
 >      - 메서드 (method)
 >      - 함수 (Function)
 >      - 행위 (behavior)
 >    - 예시
 >      - 스마트폰의 기능 - 전원on/off, 잠금해제, 볼륨up/down 등등
 >    ![객체의 기능1](https://t1.daumcdn.net/cfile/tistory/2753E146589045E815)
 >     <br/>
 >    ![객체의 기능2](https://t1.daumcdn.net/cfile/tistory/264738405890463720)
  
  ##### 인스턴스의 생성과 사용
  
  - 인스턴스 생성과 사용 방식
  ```java
  /* 객체와 인스턴스 */
    public class Main {
      public static void main(String[] args) {
        Machine phone, desktop; // '객체'

        // 인스턴스화
        phone = new Machine(); // phone은 Machine 클래스의 '인스턴스'(객체를 메모리에 할당)
        desktop = new Machine(); // desktop은 Machine 클래스의 '인스턴스'(객체를 메모리에 할당)
      }
    }
  ```
  **!Tip1.** [클래스와 인스턴스](https://whatisthenext.tistory.com/36 "클래스와 인스턴스")
  
  ##### 객체 배열
  
  ![image](https://user-images.githubusercontent.com/66407386/170925295-b89691a5-deea-4f20-b03b-0696fa4bbf61.png)
  
  **!Tip2.** [객체배열](https://www.scientecheasy.com/2021/10/arrays-of-objects-in-java.html/ "객체배열")


## 변수와 메서드
  
  ##### 선언위치에 따른 변수의 종류
  
  - 선언위치에 따른 변수
  >    - 인스턴스 변수 <br/>
  >    ▶ 클래스의 인스턴스를 만들기 위해 클래스 영역에 선언 <br/>
  >    &nbsp; &nbsp; &nbsp; 인스턴스 변수의 값을 읽어오거나 저장하기 위해서 먼저 인스턴스를 생성 <br/>
  >    &nbsp; &nbsp; &nbsp; **독립적인 저장공간을 가지므로 서로 다른 값을 가질 수 있음** <br/>
  >     - 클래스 변수 <br/>
  >     ▶ 인스턴스 변수 앞에 static을 붙이면 클래스 변수를 선언 가능 <br/>
  >     &nbsp; &nbsp; &nbsp; 모든 인스턴스가 공통된 저장공간을 공유하며 인스턴스를 생성하지 않고 바로 사용 가능  <br/>
  >     &nbsp; &nbsp; &nbsp; **클래스가 메모리에 로딩될 떄 생성되어 종료시까지 유지되며 public이** <br/>
  >     &nbsp; &nbsp; &nbsp; **있다면 같은 프로그램 내에서 접근 할 수 있는 전역변수의 성격을 얻는다.** <br/>
  >     - 지역 변수 <br/>
  >     ▶ 메서드 내에 선언되어 메서드 내에서만 사용할 수 있으며 메소드가 조율되면 소멸한다. <br/>
  >     &nbsp; &nbsp; &nbsp; **for문 while문에서 사용된 지역변수도 블럭("{}")을 벗어나면 소멸** <br/>
  
  ##### 클래스변수와 인스턴스변수
  
  - 클래스변수와 인스턴스 변수
  > 인스턴스 변수는 인스턴스가 생성될 때마다 생성되며 인스턴스 마다 각기 다른 값을 유지할 수 있지만, <br/>
  > 클래스 변수는 모든 인스턴스가 하나의 저장 공간을 공유하므로 항상 공통된 값을 갖는다. <br/>
  
  ##### 메서드
  
  - 메소드란?
  > 메서드(Method) 또는 멤버함수(Member Function)는 객체 지향 프로그래밍에서 객체와 관련된 서브 루틴이며 데이터와 <br/>
  > 멤버 변수에 대한 접근 권한을 갖는다. <br/>
  >   - 메서드를 사용하는 이유 <br/>
  >      - **소스 코드의 가독성** <br/>
  >      ▶ 메소드를 사용하여 비슷한 성격의 행동을 모아서 보여주면 다른 사람이 코드를 봤을 때 더 쉽게 이해하기 편해진다. <br/>
  >      - **소스 코드의 재사용성** <br/>
  >      ▶ 메소드를 사용하여 해당 메소드를 호출하면 그 동작을 수행하게 구현할 수 있습니다 <br/>
  
  ##### 메서드의 선언과 구현
  
  - 메소드 선언 방법
  > ```java
  > public static 리턴타입(자료형, void) 메서드명() {
  >      메서드 작성
  >      return 리턴 데이터;
  >  }
  > ```
  > 리턴 타입에는 int, String, boolean등 자료형을 넣어주며, <br/>
  > 리턴 타입에 **void가 들어가는 경우 return 받는 데이터가 없는 것을 의미하기 때문에 return을 할 필요가 없다.** <br/>
  
  **!Tip3.** [접근제어자](https://88240.tistory.com/448 "접근제어자")
  
  ##### 메서드의 호출
  
  - 메서드 호출
  > ```java
  > public class Person {
  >     /* 변수 */
  >     int age;
  >     String name;
  >
  >     /* 메서드 */
  >     public void eat(String name, int age) {
  >         // eat()이 실행될 때 작업할 내용을 여기에 작성
  >         System.out.println(age + "살의 " + name + "은(는) 음식을 먹는다");
  >     }
  > }
  > 
  > public class Main {
  >   public static void main(String[] args) {
  >       Person person = new Person();
  >       person.eat("정아무개", 29);
  >   }
  > }
  > ```
  >  - 출력 결과 : 29살 정아무개는 음식을 먹는다.
  
  ##### return문
  
  - return이란?
  > 반환값이 있을 떄만 return문을 작성했지만 반환값의 유무와 관계없이 <br/>
  > 모든 메서드에는 하나 이상의 return문이 있어야한다. <br/>
  > void일 때, return문이 오류가 나지 않는 이유는 컴파일러가 자동으로 추가해서 넘어가기 때문이다.
  
  ##### JVM의 메모리구조
  
  - 자바 프로그램의 실행 단계 <br/>
  ![JVM의 메모리구조](https://user-images.githubusercontent.com/66407386/171080811-f51c3527-71cc-4aee-9991-f11577725206.png "JVM의 메모리구조")
  
  - 진행 과정
  1. 자바 컴파일러에 의해 자바 소스파일은 바이트 코드로 변환
  2. 바이트 코드를 JVM에서 읽어 들이면서 여러 과정을 통해 OS에 상관없이 실행 할 수 있도록 처리

  > JVM 특징 - 운영체제에 종속적이라는 특징이 나타난다.

  - JVM 메모리 구조
  > JVM의 구조
  >   - GC(Garbage Collector) <br/>
  >     ▶ GC는 힙 메모리 영역에 생성된 객체들 중에서 참조되지 않은 객체들을 탐색 후 제거하는 역할 <br/>
  >   - Execution Engine <br/>
  >     ▶ Class Loader를 통해 JVM 내의 Runtime Data Area에 배치된 바이트 코드들을 명령어 단위로 읽어 실행 <br/>
  >   - Class Loader <br/>
  >     ▶ JVM 내로 클래스 파일을 로드하고, 링크를 통해 배치하는 작업을 수행하는 모듈 <br/>
  >     &nbsp; &nbsp; &nbsp; 런타임 시에 동적으로 클래스를 로드한다.
  >   - Runtime Data Area <br/>
  >     ▶ JVM의 메모리 영역으로 자바 애플리케이션을 실행 할 때 사용되는 데이터들을 기록하는 영역 <br/>
  >     &nbsp; &nbsp; &nbsp; - 영역의 종류 <br/>
  >     &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;    - Method Area <br/>
  >     &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;    - Heap Area <br/>
  >     &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;   - Stack Area <br/>
  >     &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;    - PC Register <br/>
  >     &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;    - Native Method Stack <br/>
  
  ![JVM 메모리 구조](https://user-images.githubusercontent.com/66407386/171094310-e9f6c5fd-b7ae-4b29-a655-b5126221fdeb.png "JVM 메모리 구조")
  
  **!Tip4.** [JVM메모리 구조란?](https://steady-coding.tistory.com/305 "JVM메모리 구조란?")
  
  ##### 기본형 매개변수와 참조형 매개변수
  
  <table>
    <tr>
        <th>종류</th>
        <th>내용</th>
    </tr>
    <tr>
        <td>기본형 매개변수</td>
        <td>변수의 값을 읽기만 할 수 있다. (read only)</td>
    </tr>
     <tr>
        <td>참조형 매개변수</td>
        <td>변수의 값을 읽고 변경할 수 있다. (read & write)</td>
    </tr>
  </table>
  
  ##### 참조형 반환타입
  
  ##### 재귀호출(recursive call)
  
  ##### 클래스 메서드(static메서드)와 인스턴스 메서드
  
  ##### 클래스 멤버와 인스턴스 멤버간의 참조와 호출
  
## 오버로딩(overloading)
  
  ##### 오버로딩이란?
  
  ##### 오버로딩의 조건
  
  ##### 오버로딩의 예
  
  ##### 오버로딩의 장점
  
  ##### 가변인자(varargs)와 오버로딩

## 생성자(constructor)
  
  ##### 생성자란?
  
  ##### 기본 생성자(default constructor)
  
  ##### 매개변수가 있는 생성자
  
  ##### 생성자에서 다른 생성자 호출하기 - this(), this
  
  ##### 생성자를 이용한 인스턴스의 복사
  
## 변수의 초기화
  
  ##### 변수의 초기화
  
  ##### 명시적 초기화(explicit initialization)
  
  ##### 초기화 블럭(initialization block)
  
  ##### 멤버변수의 초기화 시기와 순서
  
## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition
  2. [블로그] 더블에스님의 객체와 인스턴스, 객체의 구성요소(속성과 기능) - https://doublesprogramming.tistory.com/68
  3. [블로그] [Master Neokay님의 자바 객체 배열 | 자바 입문강좌 18](https://smoothiecoding.kr/%EC%9E%90%EB%B0%94-%EA%B0%9D%EC%B2%B4-%EB%B0%B0%EC%97%B4/ "Master Neokay님의 자바 객체 배열 | 자바 입문강좌 18")
