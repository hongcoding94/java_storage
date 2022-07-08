# Chapter12. 지네릭스, 열거형, 애너테이션

## 목차
1. [지네릭스(Generics)](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4generics)
    - [1-1. 지네릭스란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4%EB%9E%80)
    - [1-2. 지네릭 클래스의 선언](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EC%84%A0%EC%96%B8)
    - [1-3. 지네릭 클래스의 객체 생성과 사용](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EA%B0%9D%EC%B2%B4-%EC%83%9D%EC%84%B1%EA%B3%BC-%EC%82%AC%EC%9A%A9)
    - [1-4. 제한된 지네릭 클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A0%9C%ED%95%9C%EB%90%9C-%EC%A7%80%EB%84%A4%EB%A6%AD-%ED%81%B4%EB%9E%98%EC%8A%A4)
    - [1-5. 와일드 카드](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%99%80%EC%9D%BC%EB%93%9C-%EC%B9%B4%EB%93%9C)
    - [1-6. 지네릭 메서드](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD-%EB%A9%94%EC%84%9C%EB%93%9C)
    - [1-7. 지네릭 타입의 형변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD-%ED%83%80%EC%9E%85%EC%9D%98-%ED%98%95%EB%B3%80%ED%99%98)
    - [1-8. 지네릭 타입의 제거](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%A7%80%EB%84%A4%EB%A6%AD-%ED%83%80%EC%9E%85%EC%9D%98-%EC%A0%9C%EA%B1%B0)
2. [열거형(enums)](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%97%B4%EA%B1%B0%ED%98%95enums)
    - [2-1. 열거형이란? ](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%97%B4%EA%B1%B0%ED%98%95%EC%9D%B4%EB%9E%80)
    - [2-2. 열거형의 정의와 사용](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%97%B4%EA%B1%B0%ED%98%95%EC%9D%98-%EC%A0%95%EC%9D%98%EC%99%80-%EC%82%AC%EC%9A%A9)
    - [2-3. 열거형에 멤버 추가하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%97%B4%EA%B1%B0%ED%98%95%EC%97%90-%EB%A9%A4%EB%B2%84-%EC%B6%94%EA%B0%80%ED%95%98)
    - [2-4. 열거형의 이해](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%97%B4%EA%B1%B0%ED%98%95%EC%9D%98-%EC%9D%B4%ED%95%B4)
3. [애너테이션(annotation)](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98annotation)
    - [3-1. 애너테이션이란](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98%EC%9D%B4%EB%9E%80)
    - [3-2. 표준 애너테이션](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%ED%91%9C%EC%A4%80-%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98)
    - [3-3. 메타 애너테이션](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EB%A9%94%ED%83%80-%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98)
    - [3-4. 애너테이션 타입 정의하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98-%ED%83%80%EC%9E%85-%EC%A0%95%EC%9D%98%ED%95%98%EA%B8%B0)
4. [참고문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter12.%20%EC%A7%80%EB%84%A4%EB%A6%AD%EC%8A%A4,%20%EC%97%B4%EA%B1%B0%ED%98%95,%20%EC%95%A0%EB%84%88%ED%85%8C%EC%9D%B4%EC%85%98.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8)

## 지네릭스(Generics)

##### 지네릭스란?
    - 지네릭스란?
    > 컴파일시 타입을 체크해주는 기능 (Complie-time type check)
    > 객체의 타입 안정성을 높이고 형변환의 번거로움을 줄여줌
    
    - 장점과 단점
    >   - 장점
    >   a. 타입 안정성을 제공
    >   b. 타입 체크와 형변환을 생략할 수 있으므로 코드가 간결
    >   - 단점
    >   a. 컴파일러에선 에러를 찾지 못하고 실행됨
    >   b. 컴파일 시 실제로 안에 뭐가 들어 있는지 확이 안되어 classCastException 발생
    
##### 지네릭 클래스의 선언

    - 선언방법

##### 지네릭 클래스의 객체 생성과 사용

##### 제한된 지네릭 클래스

##### 와일드 카드

##### 지네릭 메서드

##### 지네릭 타입의 형변환

##### 지네릭 타입의 제거

## 열거형(enums)

##### 열거형이란?

##### 열거형의 정의와 사용

##### 열거형에 멤버 추가하

##### 열거형의 이해

## 애너테이션(annotation)

##### 애너테이션이란

##### 표준 애너테이션

##### 메타 애너테이션

##### 애너테이션 타입 정의하기

## 참고 문서 / 블로그
