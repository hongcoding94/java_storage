# Chapter6. 객체지향 프로그래밍 I

## 목차

1. [객체지향언어](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%EC%96%B8%EC%96%B4 "객체지향언어")
    - [1-1. 객체지향언어의 역사](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%EC%96%B8%EC%96%B4%EC%9D%98-%EC%97%AD%EC%82%AC "객체지향언어의 역사")
    - [1-2. 객체지향언어](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%EC%96%B8%EC%96%B4-1 "객체지향언어")
2. [클래스와 객체](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EC%99%80-%EA%B0%9D%EC%B2%B4 "클래스와 객체")
    - [2-1. 클래스와 객체의 정의와 용도](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EC%99%80-%EA%B0%9D%EC%B2%B4%EC%9D%98-%EC%A0%95%EC%9D%98%EC%99%80-%EC%9A%A9%EB%8F%84 "클래스와 객체의 정의와 용도")
    - [2-2. 객체와 인스턴스](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%9D%EC%B2%B4%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4 "객체와 인스턴스")
    - [2-3. 객체의 구성요소 - 속성과 기능](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%9D%EC%B2%B4%EC%9D%98-%EA%B5%AC%EC%84%B1%EC%9A%94%EC%86%8C---%EC%86%8D%EC%84%B1%EA%B3%BC-%EA%B8%B0%EB%8A%A5 "객체의 구성요소 - 속성과 기능")
    - [2-4. 인스턴스의 생성과 사용](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EC%9D%98-%EC%83%9D%EC%84%B1%EA%B3%BC-%EC%82%AC%EC%9A%A9 "인스턴스의 생성과 사용")
    - [2-5. 객체 배열](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%9D%EC%B2%B4-%EB%B0%B0%EC%97%B4 "객체 배열")
    - [2-6. 클래스의 또 다른 정의](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EB%98%90-%EB%8B%A4%EB%A5%B8-%EC%A0%95%EC%9D%98 "클래스의 또 다른 정의")
3. [변수와 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%B3%80%EC%88%98%EC%99%80-%EB%A9%94%EC%84%9C%EB%93%9C "변수와 메서드")
    - [3-1. 선언위치에 따른 변수의 종류](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%84%A0%EC%96%B8%EC%9C%84%EC%B9%98%EC%97%90-%EB%94%B0%EB%A5%B8-%EB%B3%80%EC%88%98%EC%9D%98-%EC%A2%85%EB%A5%98 "선언위치에 따른 변수의 종류")
    - [3-2. 클래스변수와 인스턴스변수](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EB%B3%80%EC%88%98%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EB%B3%80%EC%88%98 "클래스변수와 인스턴스변수")
    - [3-3. 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%A9%94%EC%84%9C%EB%93%9C "메서드")
    - [3-4. 메서드의 선언과 구현](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%A9%94%EC%84%9C%EB%93%9C%EC%9D%98-%EC%84%A0%EC%96%B8%EA%B3%BC-%EA%B5%AC%ED%98%84 "메서드의 선언과 구현")
    - [3-5. 메서드의 호출](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%A9%94%EC%84%9C%EB%93%9C%EC%9D%98-%ED%98%B8%EC%B6%9C "메서드의 호출")
    - [3-6. return문](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#return%EB%AC%B8 "return문")
    - [3-7. JVM의 메모리구조](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#jvm%EC%9D%98-%EB%A9%94%EB%AA%A8%EB%A6%AC%EA%B5%AC%EC%A1%B0 "JVM의 메모리구조")
    - [3-8. 기본형 매개변수와 참조형 매개변수](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B8%B0%EB%B3%B8%ED%98%95-%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98%EC%99%80-%EC%B0%B8%EC%A1%B0%ED%98%95-%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98 "기본형 매개변수와 참조형 매개변수")
    - [3-9. 참조형 반환타입](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%B0%B8%EC%A1%B0%ED%98%95-%EB%B0%98%ED%99%98%ED%83%80%EC%9E%85 "참조형 반환타입")
    - [3-10. 재귀호출(recursive call)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%9E%AC%EA%B7%80%ED%98%B8%EC%B6%9Crecursive-call "재귀호출(recursive call)")
    - [3-11. 클래스 메서드(static메서드)와 인스턴스 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%ED%81%B4%EB%9E%98%EC%8A%A4-%EB%A9%94%EC%84%9C%EB%93%9Cstatic%EB%A9%94%EC%84%9C%EB%93%9C%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4-%EB%A9%94%EC%84%9C%EB%93%9C "클래스 메서드(static메서드)와 인스턴스 메서드")
    - [3-12. 클래스 멤버와 인스턴스 멤버간의 참조와 호출](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%ED%81%B4%EB%9E%98%EC%8A%A4-%EB%A9%A4%EB%B2%84%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4-%EB%A9%A4%EB%B2%84%EA%B0%84%EC%9D%98-%EC%B0%B8%EC%A1%B0%EC%99%80-%ED%98%B8%EC%B6%9C "클래스 멤버와 인스턴스 멤버간의 참조와 호출")
4. [오버로딩(overloading)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9overloading "오버로딩(overloading)")
    - [4-1. 오버로딩이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%B4%EB%9E%80 "오버로딩이란?")
    - [4-2. 오버로딩의 조건](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%98-%EC%A1%B0%EA%B1%B4 "오버로딩의 조건")
    - [4-3. 오버로딩의 예](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%98-%EC%98%88 "오버로딩의 예")
    - [4-4. 오버로딩의 장점](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9%EC%9D%98-%EC%9E%A5%EC%A0%90 "오버로딩의 장점")
    - [4-5. 가변인자(varargs)와 오버로딩](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B0%80%EB%B3%80%EC%9D%B8%EC%9E%90varargs%EC%99%80-%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9 "가변인자(varargs)와 오버로딩")
5. [생성자(constructor)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%83%9D%EC%84%B1%EC%9E%90constructor "생성자(constructor)")
    - [5-1. 생성자란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%83%9D%EC%84%B1%EC%9E%90%EB%9E%80 "생성자란?")
    - [5-2. 기본 생성자(default constructor) ](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EA%B8%B0%EB%B3%B8-%EC%83%9D%EC%84%B1%EC%9E%90default-constructor "기본 생성자(default constructor) ")
    - [5-3. 매개변수가 있는 생성자](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98%EA%B0%80-%EC%9E%88%EB%8A%94-%EC%83%9D%EC%84%B1%EC%9E%90 "매개변수가 있는 생성자")
    - [5-4. 생성자에서 다른 생성자 호출하기 - this(), this](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%83%9D%EC%84%B1%EC%9E%90%EC%97%90%EC%84%9C-%EB%8B%A4%EB%A5%B8-%EC%83%9D%EC%84%B1%EC%9E%90-%ED%98%B8%EC%B6%9C%ED%95%98%EA%B8%B0---this-this "생성자에서 다른 생성자 호출하기 - this(), this")
    - [5-5. 생성자를 이용한 인스턴스의 복사](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%83%9D%EC%84%B1%EC%9E%90%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EC%9D%98-%EB%B3%B5%EC%82%AC "생성자를 이용한 인스턴스의 복사")
6. [변수의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%B3%80%EC%88%98%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94 "변수의 초기화")
    - [6-1. 변수의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%B3%80%EC%88%98%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94-1 "변수의 초기화")
    - [6-2. 명시적 초기화(explicit initialization)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%AA%85%EC%8B%9C%EC%A0%81-%EC%B4%88%EA%B8%B0%ED%99%94explicit-initialization "명시적 초기화(explicit initialization)")
    - [6-3. 초기화 블럭(initialization block)](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EC%B4%88%EA%B8%B0%ED%99%94-%EB%B8%94%EB%9F%ADinitialization-block "초기화 블럭(initialization block)")
    - [6-4. 멤버변수의 초기화 시기와 순서](https://github.com/hongcoding94/java_storage/blob/main/Chapter6.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20I%20.md#%EB%A9%A4%EB%B2%84%EB%B3%80%EC%88%98%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94-%EC%8B%9C%EA%B8%B0%EC%99%80-%EC%88%9C%EC%84%9C "멤버변수의 초기화 시기와 순서")

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
  
  
  
  ##### 객체 배열
  
  ##### 클래스의 또 다른 정의
  

## 변수와 메서드
  
  ##### 선언위치에 따른 변수의 종류
  
  ##### 클래스변수와 인스턴스변수
  
  ##### 메서드
  
  ##### 메서드의 선언과 구현
  
  ##### 메서드의 호출
  
  ##### return문
  
  ##### JVM의 메모리구조
  
  ##### 기본형 매개변수와 참조형 매개변수
  
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

