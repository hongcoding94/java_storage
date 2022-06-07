# Chapter8. 예외처리(Exception Handling)

## 목차
  1. [예외처리(exception handling)](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%ACexception-handling "예외처리(exception handling)")
      - [1-1. 프로그램 오류](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EC%98%A4%EB%A5%98 "프로그램 오류")
      - [1-2. 예외 클래스의 계층구조](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EA%B3%84%EC%B8%B5%EA%B5%AC%EC%A1%B0 "예외 클래스의 계층구조")
      - [1-3. 예외처리하기 try-catch문](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC%ED%95%98%EA%B8%B0-try-catch%EB%AC%B8 "예외처리하기 try-catch문")
      - [1-4. try-catch문에서의 흐름](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#try-catch%EB%AC%B8%EC%97%90%EC%84%9C%EC%9D%98-%ED%9D%90%EB%A6%84 "try-catch문에서의 흐름")
      - [1-5. 예외의 발생과 catch블럭](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8%EC%9D%98-%EB%B0%9C%EC%83%9D%EA%B3%BC-catch%EB%B8%94%EB%9F%AD "예외의 발생과 catch블럭")
      - [1-6. 예외 발생시키기](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8-%EB%B0%9C%EC%83%9D%EC%8B%9C%ED%82%A4%EA%B8%B0 "예외 발생시키기")
      - [1-7. 메서드에 예외 선언하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EB%A9%94%EC%84%9C%EB%93%9C%EC%97%90-%EC%98%88%EC%99%B8-%EC%84%A0%EC%96%B8%ED%95%98%EA%B8%B0 "메서드에 예외 선언하기")
      - [1-8. finally블럭](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#finally%EB%B8%94%EB%9F%AD "finally블럭")
      - [1-9. 자동 자원 반환 try-with-resources문](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%9E%90%EB%8F%99-%EC%9E%90%EC%9B%90-%EB%B0%98%ED%99%98-try-with-resources%EB%AC%B8 "자동 자원 반환 try-with-resources문")
      - [1-10. 사용자정의 예외 만들기](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%82%AC%EC%9A%A9%EC%9E%90%EC%A0%95%EC%9D%98-%EC%98%88%EC%99%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0 "사용자정의 예외 만들기")
      - [1-11. 예외 되던지기(exception re-throwing)](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8-%EB%90%98%EB%8D%98%EC%A7%80%EA%B8%B0exception-re-throwing "예외 되던지기(exception re-throwing)")
      - [1-12. 연결된 예외(chained exception)](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%97%B0%EA%B2%B0%EB%90%9C-%EC%98%88%EC%99%B8chained-exception "연결된 예외(chained exception)")
  
  ## 예외처리(exception handling)
  
  ##### 프로그램 오류
  
   - 프로그램 오류에 대하여
   > 프로그램 실행 중 어떠한 원인으로 인한 오작동하거나 비정상적으로 종료되는 경우<br/>
   > 결과를 초래하는 원인을 프로그램 에러 또는 오류라고 지칭한다.<br/>
   > 발생시점에 따라 에러와 오류를 구분한다.
   
   - 에러와 오류의 종류
   >  - 에러의 종류
   >    - 컴파일 에러(compile error) : 컴파일 시에 발생하는 에러
   >    - 런타임 에러(runtime error) : 실행 시에 발생하는 에러
   >    - 논리적 에러(logical error) : 실행은 되지만 의도와 다르게 동작하는 것
   >  - 오류의 종류
   >    - 에러(error) : IOException, OutOfMemoryError, StackOverflowError와 같이 수습될 수 없는 심각한 오류
   >    - 예외(exception) : 코드에 의해 수습될 수 있는 다소 미약한 오류
  
   ![]()
  
   **!Tip0.** [OutOfMemoryError에 대한 정보](https://dahye-jeong.gitbook.io/java/java/advanced/2021-01-23-outofmemoryerror)
  
  ##### 예외 클래스의 계층구조
  
  ##### 예외처리하기 try-catch문
  
  ##### try-catch문에서의 흐름
  
  ##### 예외의 발생과 catch블럭
  
  ##### 예외 발생시키기
  
  ##### 메서드에 예외 선언하기
  
  ##### finally블럭
  
  ##### 자동 자원 반환 try-with-resources문
  
  ##### 사용자정의 예외 만들기
  
  ##### 예외 되던지기(exception re-throwing)
  
  ##### 연결된 예외(chained exception)
  
## 참고 문서 / 블로그
0. [서적] 남궁성님의 Java의 정석 3rd Edition

