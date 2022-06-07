# Chapter8. 예외처리(Exception Handling)

## 목차
  1. [예외처리(exception handling)](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%ACexception-handling "예외처리(exception handling)")
      - [1-1. 프로그램 오류](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EC%98%A4%EB%A5%98 "프로그램 오류")
      - [1-2. 예외 클래스의 계층구조](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8-%ED%81%B4%EB%9E%98%EC%8A%A4%EC%9D%98-%EA%B3%84%EC%B8%B5%EA%B5%AC%EC%A1%B0 "예외 클래스의 계층구조")
      - [1-3. 예외처리하기 try-catch문](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC%ED%95%98%EA%B8%B0-try-catch%EB%AC%B8 "예외처리하기 try-catch문")
      - [1-4. try-catch문에서의 흐름](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#try-catch%EB%AC%B8%EC%97%90%EC%84%9C%EC%9D%98-%ED%9D%90%EB%A6%84 "try-catch문에서의 흐름")
      - [1-5. 예외의 발생과 catch블럭](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8%EC%9D%98-%EB%B0%9C%EC%83%9D%EA%B3%BC-catch%EB%B8%94%EB%9F%AD "예외의 발생과 catch블럭")
      - [1-6. 예외 발생시키기 / 메서드에 예외 선언하기](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8-%EB%B0%9C%EC%83%9D%EC%8B%9C%ED%82%A4%EA%B8%B0--%EB%A9%94%EC%84%9C%EB%93%9C%EC%97%90-%EC%98%88%EC%99%B8-%EC%84%A0%EC%96%B8%ED%95%98%EA%B8%B0 "예외 발생시키기 / 메서드에 예외 선언하기")
      - [1-7. finally블럭](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#finally%EB%B8%94%EB%9F%AD "finally블럭")
      - [1-8. 자동 자원 반환 try-with-resources문](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%9E%90%EB%8F%99-%EC%9E%90%EC%9B%90-%EB%B0%98%ED%99%98-try-with-resources%EB%AC%B8 "자동 자원 반환 try-with-resources문")
      - [1-9. 사용자정의 예외 만들기](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%82%AC%EC%9A%A9%EC%9E%90%EC%A0%95%EC%9D%98-%EC%98%88%EC%99%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0 "사용자정의 예외 만들기")
      - [1-10. 예외 되던지기(exception re-throwing)](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%98%88%EC%99%B8-%EB%90%98%EB%8D%98%EC%A7%80%EA%B8%B0exception-re-throwing "예외 되던지기(exception re-throwing)")
      - [1-11. 연결된 예외(chained exception)](https://github.com/hongcoding94/java_storage/blob/main/Chapter8.%20%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC(Exception%20Handling).md#%EC%97%B0%EA%B2%B0%EB%90%9C-%EC%98%88%EC%99%B8chained-exception "연결된 예외(chained exception)")
  
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
  
   **!Tip0.** [OutOfMemoryError에 대한 정보](https://dahye-jeong.gitbook.io/java/java/advanced/2021-01-23-outofmemoryerror)<br/>
   **!Tip1.** [예외처리 Best설명](https://catsbi.oopy.io/92cfa202-b357-4d47-8de2-b9b3968dfb2e)<br/>
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
  
  - Unchecked Exception 부가 설명
    > 명시적인 예외 처리를 강제하지 않기 때문에 Uncheked Exception이라고 한다.<br/>
    > 명시적인 예외 처리란 try ~ catch로 예외를 잡거나 throw로 호출한<br/>
    > 메소드에게 예외를 던지지 않는 행위를 말한다.

  **즉, Exception을 불필요하게 남발하지 말고 상황에 맞게 잘 판단 하여 Exception처리를 하자.**

  **!Tip3.** [unchecked Exception와 checked Exception에 대하여](https://steady-coding.tistory.com/583)

  ##### 예외처리하기 try-catch문

  - try/catch문
  > 반드시 실행은 되어야 하는 코드이지만 예외 처리하는 코드를 작성하여 사용자가 알수 있도록 하는 문
  > *finally블록 사용 시점*
  >   - 자원이나 DB에 커넥션 한 경우, 파일 닫기, 연결 닫기 등과 같은 **"정리 코드"를 넣는데 사용**

  - try/catch문 문법
  > ```java
  > try {
  >   // 예외발생할 가능성이 있는 문장 
  >   
  > }catch(Exception1 e1) {
  >   // Exception1이 발생했을 경우, 이를 처리하지 위한 문장적는다.
  >   // 보통 이곳에 예외메세지를 출력하고 로그로 남김.
  >   
  > }catch(Exception2 e2) {
  >   // Exception2이 발생했을 경우, 이를 처리하지 위한 문장적는다.
  >   
  > }catch(ExceptionN eN) {
  >   // ExceptionN이 발생했을 경우, 이를 처리하지 위한 문장적는다.
  >   
  > }
  > ```
  
  ##### try-catch문에서의 흐름
  
   - try-catch문 흐름
   >  - try 불록에서 발생한 경우
   >    1. 발생한 예외와 일치하는 catch문이 있는 경우
   >    2. 일치하는 catch문이 있다면 catch블럭 내의 문자을 실핼하고 try/catch문을 벗어나 다음을 수행
   >    3. 일치하는 catch문이 없다면 예외는 처리되지 못 하고 console에 * .Exception 반환됨
   >  - try 블럭 안에서 발생하지 않은 경우
   >    1. catch블럭을 거치지 않고 전체 try/catch문을 빠져나가서 다음을 수행
   >  - try 블럭 밖에서 발생한 경우
   >    1. 예외는 아무 처리되지 못 하고 console에 * .Exception 반환됨
  
   - 흐름의 이해도1. 코드가 try/catch/finally 지나가는 방식
   ![image](https://user-images.githubusercontent.com/66407386/172298079-a675d3d9-fd72-404d-8247-c8beaec46b00.png)
  
   - 흐름의 이해도2. 코드가 throw Exception을 지나가는 방식
   ![image](https://user-images.githubusercontent.com/66407386/172298117-1fa95da8-e3bd-4971-afa7-ff28796b0f5d.png)
  
  ##### 예외의 발생과 catch블럭
  
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
  >           System.out.println("마지막에 한번은 요것도~");
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
  >           System.out.println("마지막에 한번은 요것도~");
  >       }
  >     }
  >   }
  >   ```

  - 그 외 Exception
  > 사용자의 실수와 같은 외적인 요인에 의해 발생하는 예외<br/>
  > Exception 클래스에 속하는 자식 클래스들은 치명적인 예외 상황을 발생시키므로, 반드시<br/>
  > try/catch문을 사용하여 예외 처리를 해야한다.<br/>
  > *여기서 예외처리를 반드시 해야하는 경우는 checked Exception이라 부른다.*

  - checked Exception 부가 설명
    > 명시적인 예외 처리를 강제하기 때문에 Checked Exception이라 한다.<br/>
    > 반드시 try ~ catch로 예외를 잡거나 throw로 호출한 메소드에게 예외를 던져야 한다.
  
  - 그 외 Exception의 예제
  >   - ClassNotFoundException : 프로그램 실행 중 객체를 생성할 때 클래스를 찾지 못하면 발생하는 예외<br/> 
  >   ▶ 예시 <br/>
  >       - IDE의 컴파일 문제로 개발자가 추가한 **클래스가 JAR에 추가되지 않은 상태로 실행된 경우**<br/>
  >       ▶ 해결 방법<br/>
  >         1. 설정한 ClassPath 경로에서 클래스 확인하기
  >       - 라이브러리에서 **호환성 문제로 클래스를 찾지 못하는 경우**<br/>
  >       ▶  해결 방법<br/>
  >         1. 설정한 ClassPath 경로에서 클래스 확인하기
  >         2. 라이브러리의 호환성 확인하기 <br/>
  > **!Tip2.** [ClassNotFoundException을 자세히 알아보기](https://mkil.tistory.com/392)<br/> <br/> 
  >   - DataFormatException : 데이터 형식 오류가 발생 했음을 알려주는 예외<br/> 
  >   ▶ 예시 : [DataFormatException 예제](http://www.javased.com/?api=java.util.zip.DataFormatException) <br/><br/> 
  >   - FileNotFoundException : 파일을 찾을수 없어서 발생 했음을 알려주는 예외 혹은 파일이 있어도 파일 읽기, 쓰기 권한이 없어서 발생<br/>
  >   ▶ 예시 <br/>
  >       - 파일의 경로를 확인하기<br/>
  >       ▶ 해결 방법<br/>
  >         1. 해당 경로와 파일명을 체크  
  >       - 파일의 대한 권한이 있는지 확인<br/>
  >       ▶ 해결 방법<br/>
  >         1. 파일 읽기, 쓰기 권한이 있는지 체크
  
  ##### 예외 발생시키기 / 메서드에 예외 선언하기
  
  - **Checked Exception과 Unchecked Exception 차이점**
  <table>
  <tr>
    <th>구분</th>
    <th>Checked Exception</th>
    <th>UnChecked Exception</th>
  </tr>
  <tr>
    <td>확인 시점</td>
    <td>컴파일(Compile)</td>
    <td>런타임(RunTime)</td>
  </tr>
  <tr>
    <td>처리 여부</td>
    <td>반드시 예외 처리해야한다.</td>
    <td>명시적으로 하지 않아도 된다.</td>
  </tr>
  <tr>
    <td>트랜잭션 처리</td>
    <td>예외 발생시 롤백하지 않음</td>
    <td>예외 발생시 롤백 해야함</td>
  </tr>
  <tr>
    <td>종류</td>
    <td>IOException<br/>, ClassNotFoundException등</td>
    <td>NullPointException<br/>, ClassCastException</td>
  </tr>
  </table>
  
  <br/>🌟 중요 : [Checked Exception과 Unchecked Exception 차이점](https://steady-coding.tistory.com/583) <br/>

   <br/>☑️ throw와 throws의 차이점? <br/> 
   >  - throw : 예외를 일부러 발생 시키기 위해 사용 - 본인이 예외를 발생시킴
   >    - 느낌 🤔 : *내가 어떻게든 해결해야해!*<br/>
   >    - 문법 
   >    ```java
   >     throw new 예외 처리 클래스명("예외 메세지");
   >    ```
   >  - throws: 예외객체를 호출한 쪽에 전달하기 위해 사용 - 제3자가 처리하도록 던짐 <br/>
   >    - 느낌 🤔 : *일단 던져 누군가 해주겠지?* 
   >    - 문법   
   >    ```java
   >      접근제어자 반환형 메소드명() throws 예외 처리 클래스명 {
   >        // 작성 내용
   >      }
   >    ```

   - 예외 방식1 (throw Exception)
   ```java
   public class TestException {
        static void handlingException() {
            try {
                throw new Exception();
            } catch (Exception e) {
                System.out.println("호출된 메소드 -> 예외가 처리");
            }
        }

        public static void main(String[] args) {
            try {
                handlingException();
            } catch (Exception e) {
                System.out.println("두둠! 메소드 등장! 메소드가 예외가 처리해버렸다구");
            }
        }
   }
   ```
   - 출력 결과
   ```text
   호출된 메소드 -> 예외가 처리
   ```
   
   - 예외 방식2 (throws Exception)
   ```java
    public class TestException {
        static void handlingException() throws Exception { 
          throw new Exception(); 
        }
        
        public static void main(String[] args) {
          try {
              handlingException();
          } catch (Exception e) {
              System.out.println("두둠! 메소드 등장! 메소드가 예외가 처리해버렸다구");
          }
      }
    }
   ```
  - 출력 결과
  ```text
  두둠! 메소드 등장! 메소드가 예외가 처리해버렸다구
  ```
  
  ##### finally블럭
  
  - finally
  >   - try/catch문으로 진입을 하게되면 마지막에 코드가 실행된다.
  >   - try/catch문 중간에 return으로 해당 try/catch문을 빠져 나가게 되어도 실행된 후 빠져나간다.
  >   - 예외가 발생하든 발생하지 않든 무조건 수행하는 부분
  >   - **DataBase처리 혹은 File처리를 할 때 꼭 필요한 부분이다.** <br/>
  >   이유는 해당 부분을 열면 꼭 닫아주어야 프로그램이 종료가 되기때문에 finally 부분에서 수행하기 때문이다.
  
  - try/catch/finally 문법
  > ```java
  > try {
  >   // 예외발생할 가능성이 있는 문장 
  >   
  > }catch(Exception1 e1) {
  >   // Exception1이 발생했을 경우, 이를 처리하지 위한 문장적는다.
  >   // 보통 이곳에 예외메세지를 출력하고 로그로 남김.
  >   
  > }catch(Exception2 e2) {
  >   // Exception2이 발생했을 경우, 이를 처리하지 위한 문장적는다.
  >   
  > }catch(ExceptionN eN) {
  >   // ExceptionN이 발생했을 경우, 이를 처리하지 위한 문장적는다.
  >   
  > }finally{
  >   // 예외발생여부에 관계없이 상항 수행되어야 하는 문장적는다.
  > }
  
  - finally 블럭
  >   - finally블럭은 예외가 발생하건 발생하지 않건간에 항상 수행되어져야 할 코드를 명시
  >   - 객체의 소멸은 프로그래머가 컨트롤 할 수 없지만 finally블럭에서 IO와<br/>
  >   DB, File등을 사용한 후 관계를 끊는 용도로 사용한다.
  
  ##### 자동 자원 반환 try-with-resources문
  
  - try-with-resources문
  > Java1.7부터 추가된 try-with-resources문을 사용하면 간결하게 문제를 해결 할 수 있다.<br/>
  > 입출력에 사용되는 클래스 중에서는 사용한 후에 꼭 닫아줘야하는 File, DB등이 있다.<br/>
  > 자원(resources)들이 반환 되기 때문이다.
  ```java
  // Java 1.7 이전 try/catch/finally문
  import java.io.BufferedOutputStream;
  import java.io.FileInputStream;
  import java.io.FileOutputStream;
  import java.io.IOException;
  import java.io.OutputStream;
  
  public class TestException {
    public static void Main(String[] args) {

      try {
	        fis = new FileInputStream("scroe.dat");
          dis = new DataInputStream(fis);
      } catch(IOException e) {
          e.printStackTrace();
      } finally {
        dis.close();
      }
    }
  }  
  
  // ================================================== //
  
  // Java 1.7부터 나온 try/catch/resources문
  import java.io.BufferedOutputStream;
  import java.io.FileInputStream;
  import java.io.FileOutputStream;
  import java.io.IOException;
  import java.io.OutputStream;
  
  public class TestException {
    public static void Main(String[] args) {

      try(
        fis = new FileInputStream("score.dat");
        dis = new DataInputStream(fis)
      ) {
        while (true) {
          score = dis.readInt();
          system.out.println(score);
          
          sum += score;
        }
      } catch(lOException e) {
          e.printStackTrace();
      }
    }
  }
  ```
  
  ##### 사용자정의 예외 만들기
  
   - 커스텀 예외(Custom Exception)
   > ```text
   > 일반 예외로 선언할 경우 Exception을 상속받아 구현
   > 실행 예외로 선언할 경우 RuntimeException을 상속받아 구현
   > ```
   > 	- 사용자 정의 예외 클래스는 컴파일러가 체크하는 일반 예외로 선언할 수도 있고,<br/>
   >    컴파일러가 체크하지 않는 실행 예외로 선언할 수도 있다.
   >    - 일반 예외로 선언할 경우 Exception을 상속하면 되고, 실행 예외로 선언할 경우에는 RuntimeException을 상속
   >    - 사용자 정의 예외 클래스 이름을 Exception으로 끝나는 것을 권장
   >    - 사용자 정의 예외 클래스 작성 시 생성자는 두 개를 선언하는 것이 일반적
   >    	- 매개 변수가 없는 기본 생성자
   >    	- 예외 발생원인(예외 메시지)을 전달하기 위해 String 타입의 매개변수를 갖는 생성자
   >    - 예외 메시지의 용도는 catch{} 블록의 예외처리 코드에서 이용하기 위해서

   - 사용자 정의 예외 객체
   > 	- 기본 라이브러리(API)에서 제공하는 예외 객체 외 개발자가 선언해서 사용하는 예외 객체
   > 	- Exception클래스 또는 Exception의 자식클래스를 반드시 상속받아야함
   > 	- 일반적으로 Exception에서 선언된 형태의 생성자 외에는 다른 멤버를 가지지 않음

   - 커스텀 예외 예시
   ```java
	public class ReservedException extends RuntimeException {     
	 public ReservedException(String msg) {        
	    super(msg);    
	 }     
	}

	public class JoinMember {         
	   String[] reserved = {"admin", "tester", "member"};         

	   public void regId(String userId) {        
		// userId가 reserved에 있는 값과 일치 하면 안됨        
		for(String name : reserved) {            
		    if(name.equals(userId)) {
			// System.out.println("예약어 입니다.");
			// 예외 발생이 목적이므로 변경
			// throw new XXXException("msg");                
			// throw new RuntimeException("실행 예외");
			// throw new Exception("일반 예외"); 
			// java에서 잡아주는 예외이므로 빨간줄                
			throw new ReservedException(userId + "는 예약어 입니다.");            
		    }        
		 }    
	   }
	}

	public class Main { // 임의의 예외처리 만들기     
	   public static void main(String[] args) {        
		JoinMember join = new JoinMember();        
		join.regId("admin");    
	   }  
	}
   ```
  
  ##### 예외 되던지기(exception re-throwing)
  
  ##### 연결된 예외(chained exception)
  
## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [블로그] [codepark_kr님의 java-이론편](https://velog.io/@codepark_kr/%EC%9E%90%EB%B0%94-%EC%9D%B4%EB%A1%A0-%EC%98%88%EC%99%B8-%EC%B2%98%EB%A6%AC ) 
3. [블로그] [damiing님의 자바의정석 8. 예외처리(Exception handling)](https://jungdami-ing.tistory.com/entry/%EC%9E%90%EB%B0%94%EC%9D%98-%EC%A0%95%EC%84%9D-8-%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%ACException-Handling)
4. [블로그] [cheershennah님의 try-catch문이란?](https://cheershennah.tistory.com/147)
5. [블로그] [coding captain님의 예외강제 발생시키기 & 사용자 정의 예외](https://makecodework.tistory.com/entry/Java-%EC%98%88%EC%99%B8%EC%B2%98%EB%A6%AC104-%EB%8B%A4%EC%A4%91-catch-%EB%A9%80%ED%8B%B0-catch)
6. [블로그] [국브님의 throw throws(예외발생 및 예외처리)](https://bvc12.tistory.com/196)
7. [블로그] [고코딩님의 throw, throws와 Exception Handle(예외처리) 개념 및 설명](https://go-coding.tistory.com/10)
8. [블로그] [Libi님의 try-with-resources:자원을 할당하는 방법](https://sorjfkrh5078.tistory.com/103)
9. [블로그] [Yskin's님의 Throw 예외처리, 커스텀 예외처](https://qdgbjsdnb.tistory.com/33)

