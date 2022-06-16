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

##### 람다식 작성하기

##### 함수형 인터페이스(Functional Interface)

##### java.util.function 패키지

##### Function의 합성과 Predicate의 결합

##### 메서드 참조

## 스트림(stream)

##### 스트림이란?

##### 스트림 만들기

##### 스트림 중간연산

##### Optional〈T〉와 OptionalInt

#####  스트림의 최종연산

##### collect()

#####  Collector구현하기

##### 스트림의 변환

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
