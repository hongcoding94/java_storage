# Chapter07. 객체지향 프로그래밍 II

## 목차
1. [상속(inheritance)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%83%81%EC%86%8Dinheritance "상속(inheritance)")
    - [1-1. 상속의 정의와 장점](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%83%81%EC%86%8D%EC%9D%98-%EC%A0%95%EC%9D%98%EC%99%80-%EC%9E%A5%EC%A0%90 "상속의 정의와 장점")
    - [1-2. 클래스간의 관계 - 포함관계](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EA%B0%84%EC%9D%98-%EA%B4%80%EA%B3%84---%ED%8F%AC%ED%95%A8%EA%B4%80%EA%B3%84 "클래스간의 관계 - 포함관계")
    - [1-3. 클래스간의 관계 결정하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%ED%81%B4%EB%9E%98%EC%8A%A4%EA%B0%84%EC%9D%98-%EA%B4%80%EA%B3%84-%EA%B2%B0%EC%A0%95%ED%95%98%EA%B8%B0 "클래스간의 관계 결정하기")
    - [1-4. 단일상속(single inheritance)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%8B%A8%EC%9D%BC%EC%83%81%EC%86%8Dsingle-inheritance "단일상속(single inheritance)")
    - [1-5. Object클래스 - 모든 클래스의 조상](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#object%ED%81%B4%EB%9E%98%EC%8A%A4---%EB%AA%A8%EB%93%A0-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%A1%B0%EC%83%81 "Object클래스 - 모든 클래스의 조상")
2. [오버라이딩(overriding)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9overriding "오버라이딩(overriding)")
    - [2-1. 오버라이딩이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9%EC%9D%B4%EB%9E%80 "오버라이딩이란?")
    - [2-2. 오버라이딩의 조건](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9%EC%9D%98-%EC%A1%B0%EA%B1%B4 "오버라이딩의 조건")
    - [2-3. 오버로딩 vs. 오버라이딩](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%98%A4%EB%B2%84%EB%A1%9C%EB%94%A9-vs-%EC%98%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%EB%94%A9 "오버로딩 vs. 오버라이딩")
    - [2-4. super](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#super "super")
    - [2-5. super() - 조상 클래스의 생성자](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#super---%EC%A1%B0%EC%83%81-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%83%9D%EC%84%B1%EC%9E%90 "super() - 조상 클래스의 생성자")
3. [package와 import](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#package%EC%99%80-import "package와 import")
    - [3-1. 패키지(package)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%ED%8C%A8%ED%82%A4%EC%A7%80package "패키지(package)")
    - [3-2. 패키지의 선언](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%ED%8C%A8%ED%82%A4%EC%A7%80%EC%9D%98-%EC%84%A0%EC%96%B8 "패키지의 선언")
    - [3-3. import문](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#import%EB%AC%B8 "import문")
    - [3-4. import문의 선언](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#import%EB%AC%B8%EC%9D%98-%EC%84%A0%EC%96%B8 "import문의 선언")
    - [3-5. static import문](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#static-import%EB%AC%B8 "static import문")
4. [제어자(modifier)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%A0%9C%EC%96%B4%EC%9E%90modifier "제어자(modifier)")
    - [4-1. 제어자란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%A0%9C%EC%96%B4%EC%9E%90%EB%9E%80 "제어자란?")
    - [4-2. static - 클래스의, 공통적인](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#static---%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EA%B3%B5%ED%86%B5%EC%A0%81%EC%9D%B8 "static - 클래스의, 공통적인")
    - [4-3. final - 마지막의, 변경될 수 없는](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#final---%EB%A7%88%EC%A7%80%EB%A7%89%EC%9D%98-%EB%B3%80%EA%B2%BD%EB%90%A0-%EC%88%98-%EC%97%86%EB%8A%94 "final - 마지막의, 변경될 수 없는")
    - [4-4. abstract - 추상의, 미완성의](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#abstract---%EC%B6%94%EC%83%81%EC%9D%98-%EB%AF%B8%EC%99%84%EC%84%B1%EC%9D%98 "abstract - 추상의, 미완성의")
    - [4-5. 접근 제어자(access modifier)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%A0%91%EA%B7%BC-%EC%A0%9C%EC%96%B4%EC%9E%90access-modifier "접근 제어자(access modifier)")
    - [4-6. 제어자(modifier)의 조합](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%A0%9C%EC%96%B4%EC%9E%90modifier%EC%9D%98-%EC%A1%B0%ED%95%A9 "제어자(modifier)의 조합")
5. [다형성(polymorphism)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%8B%A4%ED%98%95%EC%84%B1polymorphism "다형성(polymorphism)")
    - [5-1. 다형성이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%8B%A4%ED%98%95%EC%84%B1%EC%9D%B4%EB%9E%80 "다형성이란?")
    - [5-2. 참조변수의 형변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B0%B8%EC%A1%B0%EB%B3%80%EC%88%98%EC%9D%98-%ED%98%95%EB%B3%80%ED%99%98 "참조변수의 형변환")
    - [5-3. instanceof연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#instanceof%EC%97%B0%EC%82%B0%EC%9E%90 "instanceof연산자")
    - [5-4. 참조변수와 인스턴스의 연결](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B0%B8%EC%A1%B0%EB%B3%80%EC%88%98%EC%99%80-%EC%9D%B8%EC%8A%A4%ED%84%B4%EC%8A%A4%EC%9D%98-%EC%97%B0%EA%B2%B0 "참조변수와 인스턴스의 연결")
    - [5-5. 매개변수의 다형성](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%A7%A4%EA%B0%9C%EB%B3%80%EC%88%98%EC%9D%98-%EB%8B%A4%ED%98%95%EC%84%B1 "매개변수의 다형성")
    - [5-6. 여러 종류의 객체를 배열로 다루기](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%97%AC%EB%9F%AC-%EC%A2%85%EB%A5%98%EC%9D%98-%EA%B0%9D%EC%B2%B4%EB%A5%BC-%EB%B0%B0%EC%97%B4%EB%A1%9C-%EB%8B%A4%EB%A3%A8%EA%B8%B0 "여러 종류의 객체를 배열로 다루기")
6. [추상클래스(abstract class)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B6%94%EC%83%81%ED%81%B4%EB%9E%98%EC%8A%A4abstract-class "추상클래스(abstract class)")
    - [6-1. 추상클래스란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B6%94%EC%83%81%ED%81%B4%EB%9E%98%EC%8A%A4%EB%9E%80 "추상클래스란?")
    - [6-2. 추상메서드(abstract method)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B6%94%EC%83%81%EB%A9%94%EC%84%9C%EB%93%9Cabstract-method "추상메서드(abstract method)")
    - [6-3. 추상클래스의 작성](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B6%94%EC%83%81%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%9E%91%EC%84%B1 "추상클래스의 작성")
7. [인터페이스(interface)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4interface "인터페이스(interface)")
    - [7-1. 인터페이스란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EB%9E%80 "인터페이스란?")
    - [7-2. 인터페이스의 작성](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98-%EC%9E%91%EC%84%B1 "인터페이스의 작성")
    - [7-3. 인터페이스의 상속](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98-%EC%83%81%EC%86%8D "인터페이스의 상속")
    - [7-4. 인터페이스의 구현](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98-%EA%B5%AC%ED%98%84 "인터페이스의 구현")
    - [7-5. 인터페이스를 이용한 다중상속](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EB%8B%A4%EC%A4%91%EC%83%81%EC%86%8D "인터페이스를 이용한 다중상속")
    - [7-6. 인터페이스를 이용한 다형성](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EB%8B%A4%ED%98%95%EC%84%B1 "인터페이스를 이용한 다형성")
    - [7-7. 인터페이스의 장점](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98-%EC%9E%A5%EC%A0%90 "인터페이스의 장점")
    - [7-8. 인터페이스의 이해](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%EC%9D%98-%EC%9D%B4%ED%95%B4 "인터페이스의 이해")
    - [7-9. 디폴트 메서드와 static메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%94%94%ED%8F%B4%ED%8A%B8-%EB%A9%94%EC%84%9C%EB%93%9C%EC%99%80-static%EB%A9%94%EC%84%9C%EB%93%9C "디폴트 메서드와 static메서드")
8. [내부 클래스(inner class)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4inner-class "내부 클래스(inner class)")
    - [58-1. 내부 클래스란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4%EB%9E%80 "내부 클래스란?")
    - [8-2. 내부 클래스의 종류와 특징](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%A2%85%EB%A5%98%EC%99%80-%ED%8A%B9%EC%A7%95 "내부 클래스의 종류와 특징")
    - [8-3. 내부 클래스의 선언](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%84%A0%EC%96%B8 "내부 클래스의 선언")
    - [8-4. 내부 클래스의 제어자와 접근성](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%A0%9C%EC%96%B4%EC%9E%90%EC%99%80-%EC%A0%91%EA%B7%BC%EC%84%B1 "내부 클래스의 제어자와 접근성")
    - [8-5. 익명 클래스(anonymous class)](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%9D%B5%EB%AA%85-%ED%81%B4%EB%9E%98%EC%8A%A4anonymous-class "익명 클래스(anonymous class)")

9. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter07.%20%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20II.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")

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

- 오버라이딩이란?
> 부모 클래스에서 이미 정의된 메소드를 자식 클래스에서 같은 시그니쳐를 갖는 메소드로 다시 정의
> 상속 받은 메서드에서 더 나아가 자식클래스 본인에 맞는 데이터 변경하는 경우가 있는데 조상의 메서드를 받아 오는 것을 오버라이딩이라 한다.
> 즉, **상속받은 부모 클래스의 메소드를 재정의하여 사용하는 것** 

##### 오버라이딩의 조건

- 오버라이딩의 조건
> 1. 동작만을 재정의하는 것이기에 메소드의 선언부는 기존 메소드와 완전히 같아야한다. <br/>
> &nbsp; &nbsp; &nbsp; 메소드의 반환 타입은 부모 클래스의 반환타입으로 타입이라면 변경 할 수 있음 <br/>
>   - 예시
>   ```java
>   package hello.helloWrold.Main.java
>   
>   public class Main {
>       public static void main(String[] args) {
>           // Person 클래스의 인스턴스 생성
>           Person p1 = new Person();
>           p1.setName("정아무개");
>           p1.showInfo();
>           System.out.println();
>
>           // BusinessPerson 클래스의 인스턴스를 생성
>           BusinessPerson p2 = new BusinessPerson();
>           p2.setName("정아무개");
>           p2.setCompany("(주)한국IT");
>           p2.showInfo();
>       }
>   }
>   
>   package hello.helloWrold.Maino.java
>   
>   public class MainVo {
>       private String name;
>       
>       public String getName() {
>           return name;
>       }
>       
>       public void setName(String name) {
>           this.name = name;
>       }
>
>       public void showInfo() {
>           System.ouyt.println("이름 : " + name);
>       }
>       
>       public final void whoAreYou() {
>           System.out.println("이름 : ");
>       }
>   }
>   
>   package hello.helloWrold.BusinessMain.java
>   
>   public class BusinessMain extends MainVo {
>       private String company;
>       
>       public String getCompany() {
>           return company;
>       }
>       
>       public void setCompany(String company) {
>           this.company = company;
>       }
>       
>       @Override
>       public void showInfo() {
>           System.out.println("이름 : 회사 : " + company);
>       }
>       
>       // Overloading
>       public void showInfo(int id) {
>           System.out.println("id : " + id);
>           showInfo();
>       }
>       
>       @Override // 오류 -> "Cannot override the final method from Person" error 발생
>       public void whoAre You() {
>           super.WhoAreyou();
>       }
>   }
>   ```
>   // 실행 결과
>   이름 : 정아무개
>   이름 : 정아무개           회사 : (주)IT
>   
> 2. 부모 클래스의 메소드 보다 접근제어자를 더 좁은 범위로 변경할 수 없다.
> 3. 부모 클래스의 메소드보다 더 큰 범위의 예외를 선언할 수 없다.

##### 오버로딩 vs. 오버라이딩

- 오버로딩 VS 오버라이딩
> 오버로딩 - 기존에 없는 새로운 메소드를 추가하는 것
> 오버라이딩 - 상속 받은 메소드를 재정의 하는 것

<table>
    <tr>
        <th>구분</th>
        <th>Overriding</th>
        <th>Overloading</th>
    </tr>  
    <tr>
        <td>접근 제어자</td>
        <td>부모 클래스의 메소드의 접근 제어자보다<br/>더 넓은 범위의 접근 제어자를 자식 클래스의<br/>메소드에서 설정할 수 있다.</td>
        <td>모든 접근 제어자를 사용할 수 있다.</td>
    </tr>
    <tr>
        <td>리턴형</td>
        <td>동일해야 한다.</td>
        <td>달라도 된다.</td>
    </tr>
    <tr>
        <td>메소드명</td>
        <td>동일해야 한다.</td>
        <td>동일해야 한다.</td>
    </tr>
    <tr>
        <td>매개변수</td>
        <td>동일해야 한다.</td>
        <td>달라야만 한다.</td>
    </tr>
    <tr>
        <td>적용 범위</td>
        <td>상속관계에서 적용된다.</td>
        <td>같은 클래스 내에서 적용된다.</td>
    </tr>
</table>    

- Overloading 장점
> 장점
>   - 가독성이 증가합니다.
>   - 하나의 이름만 기억하면 되므로 오류의 가능성을 많이 줄일 수 있다.
>   - 메소드의 이름만 보고 이름이 같으니, 같은 기능이라고 예측한다.
>   메서드 이름을 절약할 수 잇다.

- Override 장점
>   - 오버라이드 메소드 하나로 여러 객체를 다루고 객체마다 다른 기능을 사용할 수 있다

##### super

- super
> 자식 클래스가 부모 클래스로부터 상속받은 멤버를 참조 할 때 사용하는 참조 변수.<br/>
> 클래스 내의 멤버변수와 지역변수의 이름이 같을 경우 구분을 위한 this를 사용하듯이<br/>
> 부모 클래스와 자식 클래스의 멤버의 이름이 같을 경우 super를 사용<br/>
> this와 super는 인스턴스의 주소값을 저장하는데 static 메소드(class Method)와는 무관하게 사용

```java
package hello.helloWorld.Java.java

public class Java {
	public static void main(String[] args) {
		Child child = new Child();
		child.childMethod();
	}
}

package hello.helloWorld.Parent.java

public class Parent {
	int x = 10;
}

package hello.helloWorld.Child.java

public class Child extends Parent {
	int x = 20;

	void childMethod() {
		System.out.println("x=" + x);
		System.out.println("this.x=" + this.x);
		System.out.println("super.x=" + super.x);
	}
}

// 출력결과
// x = 20
// this.x = 20
// super.x = 10
```

##### super() - 조상 클래스의 생성자

 - super()
 > 부모 클래스의 생성자를 호출하는 메서드 상속받은 자식 클래스가 부모 클래스의 멤버를 <br/>
 > 사용할 경우가 있을 수도 있으므로 **부모 클래스를 우선적으로 초기화**해야한다.<br/>
 > 즉, **자신의 클래스의 또다른 생성자, this() 또는 부모클래스의 생성자, super()를 호출**해줘야 한다.

```java
public class JavaApp {
	public static void main(String[] args) {
		Point3D point3d = new Point3D();    // Point3D() 생성자로 초기화 및 인스턴스 생성
		System.out.println("point3d.x=" + point3d.x);
		System.out.println("point3d.y=" + point3d.y);
		System.out.println("point3d.z=" + point3d.z);
	}
}

public class Point {
	int x = 10;
	int y = 20;

	Point(int x, int y) {
		// 생성자의 첫줄에 다른 생성자를 호출하지 않았기 때문에,
		// 컴파일러가 이 부분에 super()를 호출합니다.
		// 부모 클래스이므로 Object 클래스의 super()가 호출됩니다.
		this.x = x;
		this.y = y;
	}
}

public class Point3D extends Point {
	int z = 30;

	Point3D() {
		this(100, 200, 300);	// 자신의 클래스의 또다른 생성자 호출
	}

	Point3D(int x, int y, int z) {
		super(x, y);	// 부모 클래스 생성자 호출
		this.z = z;
	}	
}

// 출력결과
// point3d.x=100
// point3d.y=200
// point3d.z=300
```

## package와 import

##### 패키지(package)

- 패키지이란?
> Package는 클래스나 인터페이스를 관련된 것들을 모아준다. <br/>
> 보통 package가 없는 클래스나 인터페이스는 만들지 않는다.
> <br/>

- 자바의 패키지 구조 / 패키지 - 디렉토리 <br/>
![PACKAGE](https://user-images.githubusercontent.com/66407386/171619156-5e34c51e-6f21-442e-a78b-b263328c70b4.png)

> - 패키지 구조 <br/>
> ▶ 클래스 : 클래스 파일(* .class) <br/>
> ▶ 패키지 : 폴더 <br/>
> ▶ 하위 패키지 : 하위폴더

- 패키지의 특성
> - 하나의 소스파일에는 첫 번째 문장으로 단 한번의 패키지 선언만을 허용한다.
> - 모든 클래스는 반드시 하나의 패키지에 속해야 한다.
> - 패키지는 점(.)을 구분자로 하여 계층구조로 구성할 수 있다.
> - 패키지는 물리적으로 클래스 파일(.class)을 포함하는 하나의 디렉토리이다.

##### 패키지의 선언

- Package 선언
> - 소스파일 첫 문장에 한번 선언하며 하나의 소스파일에 단 한번만 선언가능 
> ```java
> // 선언 방식 
> package "패키지명";
> ```
> - 같은 소스파일 클래스들은 모두 같은 패키지에 속한다
> - 패키지 선언이 없으면 이름 없는 패키지에 속하게 된다. -> Default Package
> - 클래스명과 쉽게 구분하기 위해 소문자로 선언
> ```java
> // 예제
> package hello.helloworld.package.java
>    // `` 해당 내용 작성
> ```
> - 간단한 프로그램이나 애플릿은 패키지를 지정하지 않아도 별 문제 없지만, 큰 프로젝트나 Java API와 <br/> 
>  같은 클래스 라이브러리를 작성하는 경우는 미리 패키지를 구성하여 적용하여야 함

##### import문

- import문
> 컴파일러에게 소스파일에 사용된 클래스의 패키지에 대한 정보를 제공
> - 사용하고자 하는 클래스의 패키지를 미리 명시하면 소스코드에 사용되는 클래스 이름에서 패키지명은 생략 가능
> - package와 달리 한 소스파일에 여러 번 선언 가능

##### import문의 선언

```java
import 패키지명,클래스명;
// 혹은
import 패키지명.* ;
   // `` 해당 내용 작성
```

- 선언방식
> 클래스명을 쓰는 것과 모든 클래스를 사용할 수 있는 * 의 성능 차이
> - import 문은 컴파일 시에 처리되므로 프로그램의 성능에 영향이 없습니다. <br/>
> 하지만 사용할 클래스를 작성하는 것이 무엇을 썻는지 알 수 있어서 가독성에 좋습니다.
```java
// 예제 1
package hello.helloWrold.main.java

import java.util.ArrayList;
import java.util.Calendar;
   `` 해당 내용 작성
   
// 예제 2
package hello.helloWrold.main.java

import java.util.*;
   // `` 해당 내용 작성
```

##### static import문

 - static import
 > static 멤버를 사용할 때 클래스 이름을 생략할 수 있게 해준다.
 > ```java
 > import static java.lang.Math.* ; // Math 클래스의 모든 static 멤버 사용
 > import static java.lang.System.out; 
 >
 > class Main {
 >  public static main(String[] args){
 >	out.println(random());
 >  }
 > }
 > ```

**!Tip4.** [static import 사용 방법](https://offbyone.tistory.com/283 "static import 사용 방법")

## 제어자(modifier)

##### 제어자란?

- 제어자란?
> 클래스와 클래스 멤버의 선언 시 사용하여 부가적인 의미를 부여하는 키워드

- 접근 제어자의 종류
> ▶ public - 접근 제한이 없음 <br/> 
> ![image](https://user-images.githubusercontent.com/66407386/171772312-156ab46d-2d4f-4f8c-ac67-88c4045529c5.png)
> <br/> ▶ protected - 같은 클래스,패키지 혹은 자손 클래스에서 접근 가능 <br/> 
> ![image](https://user-images.githubusercontent.com/66407386/171772335-7e2dbb8e-4987-450d-9071-e4b9439614e4.png)
> <br/> ▶ default - 같은 클래스,패키지에서 접근 가능 <br/> 
> ![image](https://user-images.githubusercontent.com/66407386/171772325-6fafbb0f-1c08-46c2-aa96-80f587eb6cf5.png)
> <br/> ▶ private - 같은 클래스 내에서만 접근가능 <br/> 
> ![image](https://user-images.githubusercontent.com/66407386/171772263-794d87c3-6fad-4819-9866-fd4d68fe71c8.png)

<table>
	<tr>
		<th>제어자 명</th>
		<th>같은 클래스</th>
		<th>같은 패키지</th>
		<th>자손 클래스</th>
		<th>전체</th>
	</tr>
	<tr>
		<td>public</td>
		<td>O</td>
		<td>O</td>
		<td>O</td>
		<td>O</td>
	</tr>
	<tr>
		<td>protected</td>
		<td>O</td>
		<td>O</td>
		<td>O</td>
		<td></td>
	</tr>
	<tr>
		<td>default</td>
		<td>O</td>
		<td>O</td>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td>private</td>
		<td>O</td>
		<td></td>
		<td></td>
		<td></td>
	</tr>
</table>

##### static - 클래스의, 공통적인

-  static의 의미 역할
> - static의 의미
> '클래스의' 또는 '공통적인'의 의미를 가지고 있다.
> - static의 역할
> <br/> ▶ 인스턴스 변수는 하나의 클래스로 부터 생성되었더라도 각기 다른 값을 유지하지만, 클래스변수(static 멤버 변수)는<br/>
> 인스턴스에 관계 없이 같은 값을 갖는다.
> <br/> ▶ 그 이유는 하나의 변수를 모든 인스턴스가 공유하기 때문이며 static이 붙은 멤버변수와 메서드, 그리고<br/>
> 초기화 블럭은 신스턴스가 아닌 클래스에 관계된 것이기 때문에 인스턴스를 생성하지 않고도 사용할 수 있음
> <br/> ▶ static이 사용될 수 있는 곳 : 멤버변수, 메서드, 초기화 블럭

- 예시 
> ```java
> class StaticTest {
>     static int width = 200; //클래스 변수
>     static int height = 120; //클래스 변수
>     
>     static {
>         //static 변수의 복잡한 초기화 수행 (초기화 블록)
>     }
>     
>     static int max(int a, int b) { //클래스 메서드
>         return a > b ? a : b;
>     }
> }
> ```

##### final - 마지막의, 변경될 수 없는


##### abstract - 추상의, 미완성의


##### 접근 제어자(access modifier)


##### 제어자(modifier)의 조합



## 다형성(polymorphism)

##### 다형성이란?

 - 다형성이란?
 > - 하나의 코드가 여러 자료형으로 구현되어 실행되는 것
 > - 같은 코드에서 여러 실행 결과가 나옴
 > - 정보은닉, 상속과 더불어 객체지향 프로그래밍의 가장 큰 특징 중 하나
 > - 객체지향 프로그래밍의 유연성, 재활용성, 유지보수성에 기본이 되는 특징
 > - 조상클래스 타입의 참조변수로 자손 클래스의 인스턴스를 참조 가능

![image](https://user-images.githubusercontent.com/66407386/171991654-8cf9468f-0ccb-4e0c-b21a-5d70d7ffb773.png)

 **!Tip5.** [다형성 이해도 높이기](https://jjine926.tistory.com/68?category=934233 "다형성 이해도 높이기")

##### 참조변수의 형변환

 - 참조변수의 형변환
 > 서로 다른 데이터 타입 간 표현이나 연산을 위해 데이터의 타입을 바꿔야 하는 경우가 있는데 
 > 데이터의 타입을 바꾸는 걸 형변환이라 한다.

 - 형변환 종류
 > - int ▶String
 >   ```java
 >   package hello.helloWorld.Main.java {
 >     public class main (String[] args) {
 >       String str = 100 + ""; // 100dms "100"으로 변환
 >     }    
 >   }  
 >   ```
 > - String ▶ int 
 >   ```java
 >   package hello.helloWorld.Main.java {
 >     public class main (String[] args) {
 >       int number = Integer.parseInt("100");  // "100"이 100으로 변환. 
 >     }    
 >   }  
 >   ```

 - 참조 변수 간 형변환
 > 참조 변수 간의 형변환은 상속 관계에 있는 타입에 한해서 가능 <br/>
 > 즉, 자손 타입 <-> 조상 타입 간 형변환이 가능한데, 두 경우 역시 표현 문법이 다르다.
 >
 > - 참조 변수 간 형변환
 >   - 자손 타입 ▶ 조상 타입 (형변환이 생략)
 >   - 조상 타입 ▶ 자손 타입 (형변환이 생략되지 않음)

 - 예제
 ```java
 class Car { // 조상 클래스 Car
    String color;
    int door;
 
    void drive(){}
    void stop() {}
 }
 
 class FireEngine extends Car { // 자손 클래스 FireEngine
     void water(){}
 }
 
 public static void main(String[] args) {
     Car car = null; // Car 타입의 참조변수 car에 null 값 선언
     FireEngine fe = new FireEngine(); // FireEngine 타입의 참조변수 fe로 FireEngine 객체 생성
     FireEngine fe2 = null; // FireEngine 타입의 참조변수 fe2로에 null 값 선언 
 
     car = fe; 
         /*조상 <- 자손 형변환. "(데이터 타입)값" 같은 형식의 형변환 생략함.
         조상타입의 참조변수로 자손의 인스턴스를 참조. 
         기본형 변수의 형변환에서 작은 자료형에서 큰 자료형의 형변환은 생략이 가능하듯이, 
         참조형 변수의 형변환에서는 자손타입의 참조변수를 조상타입으로 형변환하는 경우에는 형변환을 생략.*/
     car.drive(); // okay.
     car.water(); // error. FireEngine 클래스에만 있는 water() 메서드는 사용 못함. 

     fe2 = (FireEngine)car; 
     	/* 자손 <- 조상 형변환. 
         자손타입의 참조변수로 조상의 인스턴스를 참조 (FireEngine)로 형변환.*/
     fe2.drive(); // okay.
     fe2.water(); // okay.
 }
```

##### instanceof연산자

 - 연산자
 > - 프로그램 실행시 참조 데이터형을 검사하기 위해 사용되는 연산자
 > - 형변환이 가능한지 묻는 연산자

 - instanceof 반환 내역
 > 오른쪽 피연산자인 클래스 또는 인터페이스로부터 생성되었다면 true 그렇지 않으면 false 를 반환

 - instanceof 사용방법
 > ```java
 > package hello.helloWorld.Main.java
 >
 > public class main {
 >  public static void main(String[] args) {
 > 
 >    System.out.println(A instanceod B);
 >    // A : (인스턴스 이름)
 >    // B : (클래스 or 인터페이스 이름)
 >  }
 > }
 > ```

##### 참조변수와 인스턴스의 연결



##### 매개변수의 다형성



##### 여러 종류의 객체를 배열로 다루기



## 추상클래스(abstract class)

##### 추상클래스란?

 - 추상클래스란?
 > 하나 이상의 추상 메소드(abstract method)를 포함하는 클래스이다.
 > 추상 메소드는 선언만 있고 본체는 없는 함수이며 선언부에 'abstract'라는 키워드를 붙인다.
 > 추상 메소드가 포함되었다면 클래스도 추상 클래스이므로 클래스명 앞에도 'abstract' 키워드를 붙여야한다.

##### 추상메서드(abstract method)

 - 추상메서드란?
 > 클래스간의 공통점을 찾아내서 공통의 부모를 설계하는 작업
 >    - 반의어(?)
 >       - 구체화 : 상속을 통해 클래스를 설계, 확장하는 작업 
 
 - 추상메서드를 선언하는 이유
 > 설계자가 특정 메서드를 각 클래스 별로 재 구현을 원하지만 부모 클래스에서 일반 메서드로 구현하면 자식 클래스에서 <br/>
 > 구현을 하지 않는 경우가 발생할 수 있다. <br/>
 > 이런 메서드를 추상 메서드로 선언하면 자식 클래스는 재 구현을 강요받는다.

 - 추상 메서드의 장점
 > 1. 부모클래스에서 공통 부분을 구현과 설계가 완료되면 자식 클래스에서 상속받아 기능을 확장 시 좋다.
 > 2. 자식 클래스에서 추상메서드를 반드시 구현하도록 강요한다. (프로그램의 표준화 정도 증가)
 > 3. 공통 사항이 한곳에서 관리되어 개발 및 유지보수에 용이하다.

- 추상메서드 선언 방법
> - 클래스나 메소드 앞에 abstract를 붙여서 추상 클래스 or 추상 메소드임을 명시
> - 클래스에 추상 메소드가 포함되어 있는 경우 반드시 클래스에 abstract를 작성해야 함
> - abstract는 접근 제어자 앞이나 뒤에 사용할 수 있음

- 추상메서드 선언 방법
```java
// ① abstract를 접근 제어자 앞에 작성
abstract 접근 제어자 class 클래스명 {
    abstract 접근 제어자 반환형 메소드명();
}

// ② abstract를 접근 제어자 뒤에 작성
접근 제어자 abstract class 클래스명 {
    접근 제어자 abstract 반환형 메소드명();
}
```

##### 추상클래스의 작성

- 추상클래스
> 추상 메소드를 하나라도 가지고 있는 클래스를 추항 클래스라고 지칭함.
> 즉, 일반 클래스에는 추상 메소드가 있을 수 없음

- 추상클래스의 장점
> - 추상 클래스에서 설계가 완료되면 자식 클래스에서 상속을 받아서 기능을 확장하는데 용이
> - 지식 클래스에 추상 메소드의 구현을 강요하기 때문에 표준화 정도를 높임
> - 클래스들의 공통 사항을 한곳에서 관리 할 수 있기 때문에 개발 및 유지보수가 편해짐

- 추상클래스의 선언 방법
```java
abstract class Player { //추상클래스
    abstract void play(int pos);
    abstract void stop();
}
class AudioPlayer extends Player {
    void play(int pos) { }	//추상메서드를 구현
    void stop() {}		//추상메서드를 구현
}
abstract class AbstractPlayer extends Player {
	void play(int pos) {}	//추상메서드를 구현
}
```

## 인터페이스(interface)

##### 인터페이스란?

 - 인터페이스란?
 > 자식 클래스가 여러 부모 클래스를 상속받을 수 있다면, 다양한 동작을 수행할 수 있다는 장점을 가지게 된다.<br/>
 > 하지만 클래스를 이용하여 다중 상속을 할 경우 메소드 출처의 모호성 등 여러가지 문제가 발생 할 수 있어<br/>
 > 자바에서는 클래스를 통한 다중 상속을 지원하지 않는다.<br/>
 > 다중 상속의 이점을 버릴 수는 없기에 자바에서는 인터페이스라는 것을 통해 다중 상속을 지원한다.<br/>
 > **다른 클래스를 작성할 때 기본이 되는 틀을 제공하면서, 다른 클래스 사이의 중간 매개 역할까지 담당하는 일종의 추상 클래스를 의미**

 - class와 interface의 차이점
 <table>
  <tr>
	  <th>순서 / 내용</th>
	  <th>Class</th>
	  <th>interface</th>  
  </tr>
  <tr>
	  <td>1</td>
	  <td>인스턴스화 할 수 있다.<br/>즉, 개체를 생성 가능</td>
	  <td>인스턴스화 할 수 없다.<br/>즉, 개체 생성이 불가능</td>
  </tr>
  <tr>
	  <td>2</td>
	  <td>상속은 지원 하지만 다중상속을 지원하지 않는다.</td>
	  <td>상속은 지원 하지 않지만 다중 상속을 지원한다.</td>
  </tr>
  <tr>
	  <td>3</td>
	  <td>생성자를 포함 할 수 있다.</td>
	  <td>생성자를 포함 할 수 없다.</td>
  </tr>
  <tr>
	  <td>4</td>
	  <td>추상 메서드를 포함할 수 없다.</td>
	  <td>추상 메서드만 포함 한다.</td>
  </tr>
  <tr>
	  <td>5</td>
	  <td>변수 및 메서드는 제어 지정자를 사용하여 선언한다.</td>
	  <td>변수와 메서드는 고용으로 선언되어야 한다.</td>
  </tr>
 </table>	

##### 인터페이스의 작성
 
 - 인터페이스 선언
 > ```java
 > 접근제어자 interface 인터페이스이름 {
 >    public static final 타입 상수이름 = 값;
 >    ...
 >    public abstract 메소드이름(매개변수목록);
 >    ...
 > }
 > ```
 > 단, 클래스와는 달리 인터페이스의 모든 필드는 public static final이어야 하며, 모든 메소드는 public abstract이어야 합니다.<br/>
 > 이 부분은 모든 인터페이스에 공통으로 적용되는 부분이므로 이 제어자는 생략할 수 있습니다.
 

##### 인터페이스의 상속

##### 인터페이스의 구현

 - 인터페이스의 구현 문법
 > ```java
 >  class 클래스이름 implements 인터페이스이름 { ... }
 > ```

 - 예제 
 > ```java
 > interface Animal { public abstract void cry(); }
 > 
 > class Cat implements Animal {
 >     public void cry() {
 >         System.out.println("냐옹냐옹!");
 >     }
 > }
 >  
 > class Dog implements Animal {
 >     public void cry() {
 >         System.out.println("멍멍!");
 >     }
 > }
 > 
 > public class Polymorphism03 {
 >     public static void main(String[] args) {
 >         Cat c = new Cat();
 >         Dog d = new Dog();
 >         c.cry();
 >         d.cry();
 >     }
 > }
 > ```
 > 출력 결과
 > <br/>냐옹냐옹!
 > <br/>멍멍!

##### 인터페이스를 이용한 다중상속

 - 다중상속
 > 하나의 부모 클래스를 상속할 수 있지만 인터페이스는 다중 상속이 가능하다.<br/>
 > extends 키워드와 콤마를 이용해서 여러 개 인터페이스를 지정한다.
 > ```java
 > package hello.helloWorld.Main.java
 > 
 > public class Main() {
 > 	public interface A extends B, C{
 > 		public void strMsg();
 > 		public void numCnt();
 > 	} 
 > }
 > ```

##### 인터페이스를 이용한 다형성

 - 인터페이스를 이용한 다형성 
 > 몰루

##### 인터페이스의 장점

 - 인터페이스의 장점
 > - 개발 시간을 단축 시킬 수 있다.
 > <br/>▶ 서로 다른 개발자들이 각각의 부분을 완성할 때까지 기다리지 않고 부분을<br/> 나눠서 작성된 코드를 컴파일 할 수 있다.
 > - 클래스간 결합도를 낮출 수 있다.
 > <br/>▶ 코드의 종속성을 줄이고 유지보수성을 향상시킨다.
 > - 표준화가 가능하다.
 > <br/>▶ 클래스의 기본틀을 제공하여 개발자들에게 정형화된 개발을 강요

##### 인터페이스의 이해



##### 디폴트 메서드와 static메서드



## 내부 클래스(inner class)

##### 내부 클래스란?

 - 내부 클래스란?
 > 단어로 표현을 하자면 inner 내부의 라는 의미를 내포하고 있다. <br/>
 > 따라서 하나의 클래스 내부에 선언된 또 다른 클래스를 의미하며 <br>/>
 > 내부 클래스는 외부 클래스에 대해 두개의 클래스가 서로 긴밀한 관계를 맺고 있을 때 선언할 수 있다. 

##### 내부 클래스의 종류와 특징

 - 내부 클래스의 종류
 > 1. 정적 클래스 (static class)
 > 	- 외부 클래스 영역에 선언된 클래스 중에서 static 키워드를 가지는 클래스를 정적 클래스
 > 	<br/>▶ 외부 클래스의 인스턴스 멤버들과 관련된 작업에 사용될 목적으로 선언
 > 	
 > 2. 인스턴스 클래스 (instance class)
 > 	- 외부 클래스 영역에 선언된 클래스 중에 static 키워드를 가지지 않는 클래스를 인스턴스 클래스
 > 	<br/>▶ 외부 클래스의 static멤버, 특히 static메서드에서 사용될 목적으로 선언
 > 
 > 3. 지역 클래스 (local class)
 > 	- 외부 클래스의 메소드나 초기화 블록에 선언된 클래스
 > 	<br/>▶ 선언된 영역 내부에서 사용
 > 
 > 4. 익명 클래스 (anonymous class)
 > 	- 달리 이름을 가지지 않은 클래스<br/>
 > 	  즉, 선언과 동시에 객체를 생성하므로, 단 하나의 객체만을 생성하는 일회용 클래스
 > 	<br/>▶ 일회성

![image](https://user-images.githubusercontent.com/66407386/172124920-94b9375a-f662-40b3-9fb5-7f19123cf6fd.png)

##### 내부 클래스의 선언

 - 내부 클래스 종류들의 선언 방식
	 - 내부 클래스
	 > ```java
	 > public class Outer {
	 >  변수;
	 >  메소드;
	 >  
	 >  public class Inner {
	 >  
	 >  }
	 > }
	 > 
	 > // 객체 생성
	 > Outer 객체1 = new Outer();
	 > Outer.Inner 객체2 = 객체1.new Inner();
	 > ```

	 - 정적 클래스
	 > ```java
	 > public class Outer {
	 >   변수;
	 >   메소드;
	 >   
	 >   public static class Inner {
	 >   
	 >   }
	 > }
	 > 
	 > // 객체 생성
	 > outer.Inner 객체 = new outer.Inner();
	 > ```

	 - 지역 클래스
	 > ```java
	 > public class outer {
	 >   변수;
	 >   메소드1;
	 >   
	 >   메소드2() {
	 >      지역 변수;
	 >      
	 >      public class Inner {
	 >      
	 >      }
	 >   }
	 > }
	 > ```

	 - 익명 클래스
	 > ```java
	 > public class Inner {
	 >   변수;
	 >   메소드;
	 > }
	 > public class Outer {
	 >   변수;
	 >   메소드1;
	 >   
	 >   메소드2 {
	 >     지역변수;
	 >     
	 >     new inner() {
	 >       override된 내용들..
	 >     }
	 >   }
	 > }


##### 내부 클래스의 제어자와 접근성



**!Tip6.** [내부 클래스의 제어자와 접근성](https://velog.io/@oyeon/7-4550-%EB%82%B4%EB%B6%80-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%A0%9C%EC%96%B4%EC%9E%90%EC%99%80-%EC%A0%91%EA%B7%BC%EC%84%B1 "내부 클래스의 제어자와 접근성")

##### 익명 클래스(anonymous class)


## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [블로그] 영보님의 접근제어자 - https://qh5944.tistory.com/133
3. [블로그] shaking님의 [JAVA] 제어자(modifier) - static, final, abstract - https://88240.tistory.com/447
4. [홈페이지] geeksforgeeks 공식문서 - https://www.geeksforgeeks.org/interfaces-in-java/
