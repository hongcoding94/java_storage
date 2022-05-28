# Chapter4. 조건문과 반복문

## 목차
1. [조건문 - if, switch](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#%EC%A1%B0%EA%B1%B4%EB%AC%B8---if-switch "조건문 - if, switch")
    - [1-1. if문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#1-1-if%EB%AC%B8 "1-1. if문")
    - [1-2. if-else문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#1-2-if-else%EB%AC%B8 "1-2. if-else문")
    - [1-3. if-else if문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#1-3-if-else-if%EB%AC%B8 "1-3. if-else if문")
    - [1-4. 중첩 if문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#1-4-%EC%A4%91%EC%B2%A9-if%EB%AC%B8 "1-4. 중첩 if문")
    - [1-5. switch문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#1-5-switch%EB%AC%B8 "1-5. switch문")
2. [반복문 - for, while, do-while](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#%EB%B0%98%EB%B3%B5%EB%AC%B8---for-while-do-while "반복문 - for, while, do-while")
    - [2-1. for문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#2-1-for%EB%AC%B8 "2-1. for문")
    - [2-2. while문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#2-2-while%EB%AC%B8 "2-2. while문")
    - [2-3. do-while문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#2-3-do-while%EB%AC%B8 "2-3. do-while문")
    - [2-4. break문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#2-4-break%EB%AC%B8 "2-4. break문")
    - [2-5. continue문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#2-5-continue%EB%AC%B8 "2-5. continue문")
    - [2-6. 이름 붙은 반복문](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#2-6-%EC%9D%B4%EB%A6%84-%EB%B6%99%EC%9D%80-%EB%B0%98%EB%B3%B5%EB%AC%B8 "2-6. 이름 붙은 반복문")
3. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter4.%20%EC%A1%B0%EA%B1%B4%EB%AC%B8%EA%B3%BC%20%EB%B0%98%EB%B3%B5%EB%AC%B8.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")

--- 

## 조건문 - if, switch

  - 조건문이란?
  > 조건의 참, 거짓을 구분지어 서로 다른 작업을 수행을 도와주는 구문
  >     - 조건문의 종류
  >         - if문 / if-else
  >         - 중첩 if문
  >         - swith문

  ##### 1-1. if문
    
  ```java
  public class main {
    public static void main(String[] args) {
        int i = 0;
        
        //  if문 
        if() {
        
        }
        
        // if-else문
        if() {
        
        } else {
        
        }
    
    }
  }
  ```

  ##### 1-2. if-else문
  
  ##### 1-3. if-else if문

  ##### 1-4. 중첩 if문
  
  ##### 1-5. switch문
  

## 반복문 - for, while, do-while

  ##### 2-1. for문
  
  ##### 2-2. while문

  ##### 2-3. do-while문

  ##### 2-4. break문
  
  ##### 2-5. continue문
  
  ##### 2-6. 이름 붙은 반복문
  
  
## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition
