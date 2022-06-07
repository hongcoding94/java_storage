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
  
   **!Tip0.** [OutOfMemoryError에 대한 정보](https://dahye-jeong.gitbook.io/java/java/advanced/2021-01-23-outofmemoryerror)
   **!Tip1.** [예외처리 Best설명](https://catsbi.oopy.io/92cfa202-b357-4d47-8de2-b9b3968dfb2e)
  ##### 예외 클래스의 계층구조
  
  ![image](https://velog.velcdn.com/images%2Fcodepark_kr%2Fpost%2Fa70025be-d97d-4ba4-81de-bf9b8fe48d2b%2FExceptionClassHierarchy.png)
  
  - **Throwable 클래스**
  > Throwable 클래스는 모든 예외의 조상이 되는 Exception 클래스와 모든 오류의 조상이 되는 Error 클래스의 부모 클래스
  <table>
  <tr>
    <th>종류 메소드</th>
    <th>내용 설명</th>
  </tr>
  <tr>
    <td>String getMessage()</td>
    <td>해당 throwable 객체에 대한 자세한 내용을 문자열로 반환</td>
  </tr>
  <tr>
    <td>void printStackTrace()</td>
    <td>해당 throwable 객체와 표준 오류 스트림(standard error stram)에서 해당 객체의<br/> 스택 트레이스(stack trace)를 출력함</td>
  </tr>
  <tr>
    <td>String toString()</td>
    <td>해당 throwable 객체에 대한 간략한 내용을 문자열로 반환함</td>
  </tr>
  </table>
  
  - **Exception 클래스의 두 하위 클래스**
  > Exception 하위 클래스 
  >   - RuntimeException 클래스
  >   - 그 외 Exception 클래스의 자식
  
  - RuntimeException
  > 발생 원인은 프로그래머들의 실수로 발생되는 예외<br/>
  > RuntimeException 클래스를 상속받는 자식 클래스들은 치명적인 예외 상활을 발생 시키지 않는 예외들로 구성<br/>
  > try/catch문을 사용하기 보다는 프로그램을 작성하면서 예외가 발생하지 않도록 처리하는 것이 좋다.<br/>
  > *여기서 예외처리를 개발자의 판단에 맞기는 경우를 Unchecked Exception이라 부른다.*

  - RuntimeException의 예제
  >   - ArrayIndexOutOfBoundException : 잘못된 인덱스를 사용해서 배열에 접근했다는 것을 알려주기 위한 예외<br/>
  >   ▶ 예시 <br/>
  >   ```java
  >   int[] array = new int[5];
  >   int boom = array[10]; // throws the exception
  >   
  >   // ============================================== //
  >   
  >   int[] array = new int[5];
  >   // 잘못된 예제
  >   for (int index = 1; index <= array.length; index++) { // 여기서 ArrayIndexOutOfBoundException 발생!!
  >     System.out.println(array[index]);
  >   }
  >   
  >   // 올바른 예제
  >   for (int index = 0; index < array.length; index++) {
  >     System.out.println(array[index]);
  >   }
  >   ```
  >   
  >   - ArithmeticException : 예외적인 산술 조건이 발생하여 알려주기 위한 예외<br/> 
  >   ▶ 예시 <br/>
  >   ```java
  >   // 잘못된 예제
  >   public class TestException {
  >     public static void main(String[] args) {
  >       // 변수 생성
  >       int i = 1994;
  >       int j = 0;
  >       
  >       System.out.println( i / j );   // 여기서 ArithmeticException 발생!!
  >     }
  >   }
  >   
  >   // 올바른 예제 1 (if문)
  >   public class TestException {
  >     public static void main(String[] args) {
  >       // 변수 생성
  >       int i = 1994;
  >       int j = 0;
  >       if(j != 0 ) {     // 조건식으로 막혀서 해당 코드가 돌지 않기 때문에 에러발생 없음.
  >         System.out.println( i / j );
  >       }
  >     }
  >   }
  >   
  >   // 올바른 예제 2 (try/catch)
  >   public class TestException {
  >     public static void main(String[] args) {
  >       // 변수 생성
  >       int i = 1994;
  >       int j = 0;
  >       int k;
  >       
  >       try{
  >         k = i / j;
  >       } catch(ArithmeticException e) {
  >           System.out.println("ArithmeticException 발생");
  >       } finally {
  >           System.out.println("모든지 넘겨~");
  >       }
  >     }
  >   } 
  >   ```
  >   
  >   - ClassCastException : 코드가 하위 유형이 아닌 유형에 대한 참조를 캐스팅 시도했을 때 확인되지 않은 예외<br/>
  >   ▶ 예시 : 참고 블로그 - https://recordsoflife.tistory.com/583
  >   
  >   - NumberFormatException 
  >     - 숫자로 변경하는 도중 숫자형이 아닌 그외 문자열 등인 경우 예외
  >     - 변경하는 자료형보다 범위가 큰 경우
  >     - Null입력 시 예외
  >     - 문자 앞뒤로 공백이 있는 경우 <br/> 
  >   ▶ 예시 <br/> 
  >   ```java
  >   // 잘못된 예제
  >   public class TestException {
  >     
  >     public static void main(String[] args) throws Exception {
  >       String str = "";
  >       
  >         str = "1543OO";  // 숫자 1543 & 문자 OO
  >         System.out.println(Integer.parseInt(str));    // 여기서 NumberFormatException 발생
  >     }
  >   }
  >   // 올바른 예제
  >   public class TestException {
  >     
  >     public static void main(String[] args) throws Exception {
  >       String str = "";
  >       
  >       try{
  >         str1 = "1543OO";  // 숫자 1543 & 문자 OO
  >         System.out.println(Integer.parseInt(str1));    
  >       } catch(NumberFormatException e) {
  >         str2 = "2022";
  >         System.out.println(Integer.parseInt(str2));
  >       } catch(Exception e) {
  >         e.printStackTrace();
  >       }
  >     }
  >   }
  >   ```
  > 
  >   - NullPointerException : 실제 값이 아닌 null을 가지고 있는 개체 혹은 변수 등을 호출 할 경우 예외<br/> 
  >   ▶ 예시 <br/> 
  >   ```java
  >   // 잘못된 예제
  >   public class TestException {
  >     public static void main(String[] args) {
  >       String str = null;
  >       System.out.println(str); // 여기서 NullPointerException 발생
  >     }
  >   }
  >   
  >   // 올바른 예제
  >   public class TestException {
  >     public static void main(String[] args) {
  >     
  >       try{
  >           String str = null;
  >           System.out.println(str); 
  >       } catch(NullPointException e) {
  >           System.out.println("NullPointerException 발생");
  >       } funally {
  >           System.out.println("모든지 넘겨~");
  >       }
  >     }
  >   }
  >   ```

  - 그 외 Exception
  > 사용자의 실수와 같은 외적인 요인에 의해 발생하는 예외<br/>
  > Exception 클래스에 속하는 자식 클래스들은 치명적인 예외 상황을 발생시키므로, 반드시<br/>
  > try/catch문을 사용하여 예외 처리를 해야한다.<br/>
  > *여기서 예외처리를 반드시 해야하는 경우는 checked Exception이라 부른다.*
  
  - 그 외 Exception의 예제
  >   - ClassNotFoundException : 
  >   - DataFormatException : 
  >   - FileNotFoundException : 

  **즉, Exception을 불필요하게 남발하지 말고 상황에 맞게 잘 판단 하여 Exception처리를 하자.**

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
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [블로그] [codepark_kr님의 java-이론편](https://velog.io/@codepark_kr/%EC%9E%90%EB%B0%94-%EC%9D%B4%EB%A1%A0-%EC%98%88%EC%99%B8-%EC%B2%98%EB%A6%AC "") 

