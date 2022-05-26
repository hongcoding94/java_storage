# Chapter 2 변수(Variable)

## 목차
1. [변수와 상수](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EC%99%80-%EC%83%81%EC%88%98 "변수와상수")
   - [변수란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EB%9E%80 "변수란?")
   - [변수를 선언 방법과 종류](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EB%A5%BC-%EC%84%A0%EC%96%B8-%EB%B0%A9%EB%B2%95%EA%B3%BC-%EC%A2%85%EB%A5%98 "변수를 선언 방법과 종류")
   - [변수의 규칙](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EC%9D%98-%EA%B7%9C%EC%B9%99 "변수의 규칙")
2. [변수의 타입](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EC%9D%98-%ED%83%80%EC%9E%85 "변수의타입")
   - [2-1. 기본 변수들의 설명](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#2-1-%EA%B8%B0%EB%B3%B8-%EB%B3%80%EC%88%98%EB%93%A4%EC%9D%98-%EC%84%A4%EB%AA%85 "2-1. 기본 변수들의 설명")
   - [2-2. 기본 변수들의 크기](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#2-2-%EA%B8%B0%EB%B3%B8-%EB%B3%80%EC%88%98%EB%93%A4%EC%9D%98-%ED%81%AC%EA%B8%B0 "2-2. 기본 변수들의 크기")
   - [2-3. 클래스 선언 하여 객체 담는 방법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#2-3-%ED%81%B4%EB%9E%98%EC%8A%A4-%EC%84%A0%EC%96%B8-%ED%95%98%EC%97%AC-%EA%B0%9D%EC%B2%B4-%EB%8B%B4%EB%8A%94-%EB%B0%A9%EB%B2%95--%EC%89%AC%EC%96%B4%EA%B0%80%EA%B8%B0- "2-3. 클래스 선언 하여 객 담는 방법")
   - [2-4. 상수와 리터럴](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#2-4-%EC%83%81%EC%88%98%EC%99%80-%EB%A6%AC%ED%84%B0%EB%9F%B4 "2-4. 상수와 리터럴")
   - [2-5. 형식화된 출력](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#2-5-%ED%98%95%EC%8B%9D%ED%99%94%EB%90%9C-%EC%B6%9C%EB%A0%A5 "2-5. 형식화된 출력")
   - [2-6. 화면에서 입력받기](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#2-6-%ED%99%94%EB%A9%B4%EC%97%90%EC%84%9C-%EC%9E%85%EB%A0%A5%EB%B0%9B%EA%B8%B0 "2-6. 화면에서 입력받기")
3. [진법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EC%A7%84%EB%B2%95 "진법")
   - [3-1. 10진법과 2진법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#3-1-10%EC%A7%84%EB%B2%95%EA%B3%BC-2%EC%A7%84%EB%B2%95 "3-1. 10진법과 2진법")
   - [3-2. 비트와 바이트 ](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#3-2-%EB%B9%84%ED%8A%B8%EC%99%80-%EB%B0%94%EC%9D%B4%ED%8A%B8 "3-2. 비트와 바이트")
   - [3-3. 8진법과 16진법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#3-3-8%EC%A7%84%EB%B2%95%EA%B3%BC-16%EC%A7%84%EB%B2%95 "3-3. 8진법과 16진법")
   - [3-4. 정수의 진법 변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#3-4-%EC%A0%95%EC%88%98%EC%9D%98-%EC%A7%84%EB%B2%95-%EB%B3%80%ED%99%98 "3-4. 정수의 진법 변환")
   - [3-5. 실수의 진법 변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#3-5-%EC%8B%A4%EC%88%98%EC%9D%98-%EC%A7%84%EB%B2%95-%EB%B3%80%ED%99%98 "3-5. 실수의 진법 변환")
   - [3-6. 6음수의 2진표현 -2의 보수법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#3-6-6%EC%9D%8C%EC%88%98%EC%9D%98-2%EC%A7%84%ED%91%9C%ED%98%84--2%EC%9D%98-%EB%B3%B4%EC%88%98%EB%B2%95 "3-6. 6음수의 2진표현 -2의 보수법")
4. [기본형](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EA%B8%B0%EB%B3%B8%ED%98%95 "기본형")
5. [형변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%ED%98%95%EB%B3%80%ED%99%98 "형변환")
   - [5-1. 형변환(캐스팅 Casting)이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#5-1-%ED%98%95%EB%B3%80%ED%99%98%EC%BA%90%EC%8A%A4%ED%8C%85-casting%EC%9D%B4%EB%9E%80 "5-1. 형변환(캐스팅 Casting)이란?")
   - [5-2. 형변환 방법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#5-2-%ED%98%95%EB%B3%80%ED%99%98-%EB%B0%A9%EB%B2%95 "5-2. 형변환 방법")
   - [5-3. 정수형과 실수형 간의 형 변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#5-3-%EC%A0%95%EC%88%98%ED%98%95%EA%B3%BC-%EC%8B%A4%EC%88%98%ED%98%95-%EA%B0%84%EC%9D%98-%ED%98%95-%EB%B3%80%ED%99%98 "5-3. 정수형과 실수형 간의 형 변환")
   - [5-4. 자동 형 변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#5-4-%EC%9E%90%EB%8F%99-%ED%98%95-%EB%B3%80%ED%99%98 "5-4. 자동 형 변환")     
6. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "")

---
## 변수와 상수

   ##### 변수란?
   > 값을 저장하는 공간(선언과 동시에 메모리 공간에 변수를 지정) <br/>
   > 즉. 큰 도화지 위에 하나의 공간을 배정하여 공간 안에 미지의 조건 데이터 입력하는 공간

   ##### 변수를 선언 방법과 종류
   ```java
      /* 방법1. 변수를 선언하는 동시에 데이터 부여 */
      int count = 0;
      String name = '자바의정석';
      
      System.out.println("count : " + count + ", name : " + name );
      // 출력 시 - count : 0, name : 자바의정석

      /* 방법2. 변수를 선언하고 후에 데이터 부여 */
      int count;           // 실질적으로 int는 조건 숫자 데이터가 없기 때문에 0으로 처리됨
      String name;         // 실질적으로 String는 조건 문자 데이터가 없기 때문에 null으로 처리됨
     
      System.out.println("count : " + count + ", name : " + name );
      // 출력 시 - count : 0, name : null
      
      count = 1;           // 해당 변수에 1을 선언함으로 변수 안에 1이라는 숫자가 들어감
      name = '자바의정석';  // 해당 변수에 '자바의정석'을 선언함으로 변수 안에는 "자바의정석"이라는 문자가 들어감
     
      System.out.println("count : " + count + ", name : " + name );
      // 출력 시 - count : 1, name : 자바의정석
      
      // 방법2의 변수만 선언 후 데이터를 출력하면 데이터가 없는 빈 변수로 출력이 된다.
      // 즉. 변수에 데이터를 담은 이후 데이터가 출력되는 것을 볼 수 있다.
   ```
   
   **! Tip0.** [변수 선언(Variable declare)과 초기화(Initialize)](https://7942yongdae.tistory.com/22 "변수 선언(Variable declare)과 초기화(Initialize)")
   
   ##### 변수의 규칙
   1. 예약어 혹은 규칙어를 사용하지 않는다.
   2. 특수문자는 __와 $를 제외한 나머지는 사용하면 안된다.
   3. 첫글자에 숫자를 사용하지 않으며 되도록이면 숫자를 사용하지 않는 것을 권장한다.
   4. 대소문자가 구분되며 길이제한이 없다.
   
## 변수의 타입

   ##### 2-1. 기본 변수들의 설명<br/>
   <table>
      <tr>
        <tr>
           <td rowspan="2">논리</td>
           <tr>
              <td>논리</td>
              <td>boolean</td>
              <td>논리의 참과 거짓을 의미하는 true, false 중 하나의 값을 저장</td>
           </tr>
        </tr>   
        <tr>
           <td rowspan="5">숫자</td>
           <tr>
             <td rowspan="2">정수</td>
             <td>int</td>
             <td rowspan="2">정수(Integer)를 저장하기 위한 타입</td>
           </tr>
           <tr>
             <td>long</td>
           </tr>
           <tr>
             <td rowspan="2">실수</td>
             <td>float</td>
             <td rowspan="2">실수(floating-point number)를 저장하기 위한 타입</td>
           </tr>
           <tr>
             <td>double</td> 
           </tr>
        </tr>        
        <tr>
           <td rowspan="3">문자</td>
           <tr>
             <td>문자</td>
             <td>char</td>
             <td>문자(character)를 저장하기 위한 타입</td>
           </tr>
           <tr>
             <td>여러 문자</td>
             <td>String</td>
             <td>여러 문자(문자열, string)를 저장하기 위한 타입</td>
           </tr>
        </tr> 
   </table>
  
  ##### 2-2. 기본 변수들의 크기<br/>
   |종류/크기|1Byte|2Byte|3Byte|4Byte|
   |:---:|:---:|:---:|:---:|:---:|
   |논리형|boolean|    | | 	| 	 
   |문자형|       |char| |    |	 	 	 	 
   |정수형|byte|short|int(default)|long| 	 	 	 
   |실수형|     ||float|double|	
   
   
  ##### 2-3. 클래스 선언 하여 객체 담는 방법  (쉬어가기) <br/>
   
   ```java
      package hello.helloWorld.veriable.java
   
      public Class veriable() {
          // Vo 선언 방식 현재 많이 쓰는 방식 기준으로 정렬해봤습니다.
          /* 문자열 / 문자 */
          private String   str;
          private char     strYn;
         
          /* 정수 */
          private int      cnt;
          private long     cnt2;

          /* 논리형 */
          private Boolean  trueOrFalse;
      }
   ```
   
  **! Tip1.** [private와 public의 차이 - 접근 지정자](https://luyin.tistory.com/232 "private와 public의 차이")

  ##### 2-4. 상수와 리터럴
  
  상수이란?
  > 변하지 않는 변수 <br/>
  > 즉. 상수에 넣는 데이터는 숫자나 클래스나 구조체 같이 기본형에서 파생된 객체나 유도형 같은 데이터를 넣을 수 있다.
  >   예시)
  >    ```java
  >       package hello.helloWorld.constant.java
  >       
  >       public class constant() {
  >         public void constantTest() {
  >            // 상수 선언 및 초기화
  >            final int con;
  >
  >            // 데이터 주입 
  >            final int con = 20220525;
  >
  >            // 변수에 다른 데이터 주입
  >            con = 20220524;
  >
  >            // 결과
  >            System.out.println("con : " + con);
  >        
  >            // con : 20220525
  >            // 상수는 처음 값을 초기화하면, 이후 상수의 값은 변경할 수 없다.
  >         }
  >      }
  >    ```
  
  - *중요*
      - JDK 1.6 이전에는 상수 선언과 동시에 초기화가 필수였으나, 1.6 이후부터는 선언과 동시에 초기화하지 않아도 자동으로 처리해준다. <br>
        하지만 상수는 선언과 동시에 초기화하는 것을 **권장**합니다.  
  
  리터럴이란?
  > 값이 변하지 않는 데이터 <br/>
  > 즉. 변수에 변하지 않은 값으로 돌려준다.
  >   예시)
  >   ```java
  >      package hello.helloWorld.literal.java
  >
  >      public class literal() {
  >         public void literalTest() {
  >           // 변수 선언
  >           int lit = 20220525;
  >
  >           /*
  >           *  이렇게 생각하자
  >           *  변수(variable)   -   하나의 값을 저장하기 위한 공간
  >           *  상수(constant)   -   값을 한번만 저장할 수 있는 공간
  >           *  리터럴(literal)  -   그 자체로 값을 의미하는 것
  >           */
  >         }
  >      }
  >   ```
      
  
  ##### 2-5. 형식화된 출력
  
  > 형식화된 출력
  > 화면에 값을 출력할 때 System.out.println("내용") 편리하지만
  > 단점으로는 변수의 값을 그대로  노출하고, 값을 변환하지 않고서는 다른 형식으로 출력할 수 없다.
  
  - printf( )는 '지시자(specifier)' 를 통해 변수의 값을 여러 가지 형식으로 변환하여 출력하는 기능을 갖고있다.
  - printf( )는 println( )과 달리 줄바꿈을 하지않는다. 줄바꿈을 할때는 큰따옴표("") 안에 \n 혹은 %n을 사용한다.
  
  <table>
   <tr>
      <th>지시자</th>
      <th>설명</th>
   </tr>
   <tr>
      <td>%d</td>
      <td>10진(decimal) 정수의 형식으로 출력</td>
   </tr>
   <tr>
      <td>%f</td>
      <td>부동 소수점(float -point)의 형식으로 출력</td>
   </tr>
   <tr>
      <td>%o</td>
      <td>8진(octal) 정수의 형식으로 출력</td>
   </tr>
   <tr>
      <td>%x, %X</td>
      <td>16진(hexa-decimal) 정수의 형식으로 출력</td>
   </tr>
   <tr>
      <td>%c</td>
      <td>문자(charactor)로 출력</td>
   </tr>
   <tr>
      <td>%s</td>
      <td>문자열(string)로 출력</td>
   </tr>   
   <tr>
      <td>%b</td>
      <td>불리언(boolean)로 출력</td>
   </tr>     
   <tr>
      <td>%e, %E</td>
      <td>지수(exponent) 표현식의 형식으로 출력</td>
   </tr>  
</table>
  
  ```java
  int num_i = 123;
  double num_d = 1.23456789;
  double num_d1 = 1.2345678987654321;
  String url = "https://hbeige.tistory.com";
 
  System.out.printf("[%d]%n", num_i);   // [123]
  System.out.printf("[%5d]%n", num_i);  // [  123]
  System.out.printf("[%05d]%n", num_i); // [00123]
  System.out.printf("[%-5d]%n", num_i); // [123  ]
 
  System.out.println("[123456789012345678901234567890]->30칸");
  System.out.printf("[%s]%n", url);
  System.out.printf("[%30s]%n", url);  // 30칸 중 오른쪽 정렬
  System.out.printf("[%-30s]%n", url); // 30칸 중 왼쪽정렬
  System.out.printf("[%.8s]%n", url);  // 왼쪽에서 8글자만 출력
 
  System.out.printf("[%f]%n", num_d); // 마지막 소수점 자리에서 반올림
  System.out.printf("[%14.10f]%n", num_d);  // 전체 14자리 중 소수점 10자리까지 출력
  System.out.printf("[%14.10f]%n", num_d1); // 전체 14자리 중 소수점 10자리까지 출력+마지막 소수점 자리에서 반올림
  System.out.printf("[%-14.10f]%n", num_d); // 전체 14자리 중 소수점 10자리까지 왼쪽정렬 출력
  ```
  
  - 출력 결과 <br/>
    ![출력 결과](https://user-images.githubusercontent.com/66407386/170272305-f07ac873-5db6-4e37-b3bd-75c9ba6c1967.png)

  
  ##### 2-6. 화면에서 입력받기
  
  Scanner 사용방법<br/>
  >  - import java.util.* ; : java util에 대한 모든 클래스의 객체를 생성<br/>
  >  - import java.Scanner; : java Scanner의 클래스의 객체를 생성

  ```java
  import java.util.*;

  public class scanner {
    public static voiud main(String[] args) {
      Scanner scanner = new Scanner(System.in);
     
      // Scanner에 데이터를 넣기 위한 변수 생성
      String inputData = scanner.nextLine();
      int number = Integer.parseInt(inputData);

      System.out.println("nember : " + nember);
      // nember : "스캐너에 넣은 데이터 출력"
      // 단. int로 출력하기 때문에 문자를 넣었을때 Error발생
    }
  }
  ```
  

## 진법

   ##### 3-1. 10진법과 2진법

   - 10진법
   > 우리가 실생활에 쓰는 수
   
   - 2진수
   > 0-1을 나타낼 수 있음
   > 가장 큰 수 1의 값은 : 1
   > 2진수는 1개의 비트만 있으면 모두 표현 가능

   2진수 <-> 10진수 <br/>
   ex) 10101(2) <br/>
      - 1*2^3 + 0*2^2 + 1*2^0 = 8 2 + 1 = 11(10)
   
   10진수 -> 2진수       <br/>
   ex) 11(10)           <br/>
      - 2 | 11          <br/>
      - 2 | 5  - 1      <br/>
      - 2 | 2  - 1      <br/>
      - &nbsp;&nbsp;&nbsp;&nbsp; 1  - 0      <br/>
      > 결과 : 1011(2)   <br/>
   
   

   **!Tip4.** [10진법과 2진법이 이해가 안될 때 영상](https://www.youtube.com/watch?v=ZMTYl8NHjTg "10진법과 2진법이 이해가 안될 때 영상") 
   
   ##### 3-2. 비트와 바이트
   
   <table>
   <tr>
      <th>단위</th>
      <th>바이트</th>
      <th>비트</th>
   </tr>
   <tr>
      <td>비트(bit)</td>
      <td>1/8 바이트</td>
      <td>1 비트</td>
   </tr>
   <tr>
      <td>바이트(Byte)</td>
      <td>1 바이트</td>
      <td>8 비트</td>
   </tr>
   </table>
   
   - 비트(bit) - 컴퓨터에서 사용하는 가장 작은 데이터 단위, 하나의 비트는 2진수 1 또는 0으로 표현되어데이터를 처리, 저장, 전송 할 때 사용된다.
   - 바이트(Byte) - 데이터 파일의 크기, 디스크 또는 그 외 저장 매체의 공간, 그리고 네트워크를 통하여 전송 되는 데이터의 양을 표현하는데 
                   사용 되는 측정 단위, 1바이트는 8비트 (1Byte = 8bit) 와 같다.
   
   **!Tip5.** [Bit와 Byte차이점](https://roxxy.tistory.com/entry/Bit-%EC%99%80-Byte-%EC%B0%A8%EC%9D%B4%EC%A0%90 "Bit와 Byte차이점")
   
   ##### 3-3. 8진법과 16진법
   
   - 8진법
   > 0-7을 나타낼 수 있음
   > 가장 큰 수 7의 이진수 값은  : 111
   > 8진수는 3개의 비트만 있으면 모두 표현 가능
   
   - 16진법
   > 0-15를 나타낼 수 있음
   > 가장 큰 수 15의 이진수 값은 1111
   > 16진수는 4개의 비트만 있으면 모두 표현 가능
   
   8진수 <-> 10진수
   ex) 17(8) <br/>
   1*8^1 + 7*8^0 = 8 + 7 = 15(10) <br/>
   
   10진수 -> 8진수 <br/>
   ex) 15(10) <br/>
    - 8 | 15 <br/>
    - &nbsp;&nbsp;&nbsp;&nbsp; 1 - 7 <br/>
    - 결과 : 17(8)
   
   ##### 3-4. 정수의 진법 변환
   
   
   ##### 3-5. 실수의 진법 변환
   
   
   ##### 3-6. 6음수의 2진표현 -2의 보수법


   **!Tip6.** [진법 총정리](https://itbeginner2020.tistory.com/17 "진법 총정리")

## 기본형

 - 논리형(True or False)
   - 논리형에는 'boolean' 한가지 밖에 없다. true, false 둘 중 한가지 값만을 허락한다. <br/> default 값은 'false'이다. 
 >  - boolean
 >  > ```java
 >  > public statice void main(String[] args) {
 >  >  boolean power = true;
 >  >  -- boolean check = False; // 에러발생. 대소문자가 구분됨
 >  >  
 >  >  System.out.println("power : " + power);
 >  >  // power : true
 >  > }
 >  > ```

 - 문자형
   - char, 한 가지 자료형 밖에 없다. 단. 하나의 문자만 저장할 수있다. <br/> 
     '문자'가 저장되는 것 같지만, 사실은 문자가 아닌 '문자의 유니코드(정수)'가 저장된다. <br/>
     컴퓨터는 숫자 밖에 모른다.
 > - char(character)
 >  > ```java
 >  > public statice void main(String[] args) {
 >  >  char ch = 'A'; // 문자 'A'를 char타입의 변수 ch에 저장
 >  >  -- char ch = 29;  // 문자의 코드를 직접 변수 ch에 저장
 >  > 
 >  >  System.out.println("ch : " + ch);
 >  >  // ch : A
 >  > }
 >  > ```
 
 - 참조형
   - 어떤 값이 저장되어 있는 주소를 값으로 가진다. 8개의 기본형을 제외한 나머지 모든 타입
 >  - String
 >  > ```java
 >  > public statice void main(String[] args) {
 >  >  String str = '자바의 정석';
 >  >  
 >  >  System.out.println("str : " + str);
 >  >  // str : 자바의 정석
 >  > }
 >  > ```

 - 정수형
   - 기본 자료형은 'int'이다. 어떤 진법의 리터럴을 변수에 저장해도 실제로는 2진수로 바뀌어 저장된다. <br/>
     ex) 정수나 실수 범위가 벗어나면 오버플로우 혹은 언더플로우 를 발생시킨다.
 >  - byte
 >  > 
 >  - short
 >  > 
 >  - int(integer)
 >  > 
 >  - long
 >  > 

 - 실수형
 > - float
 > > ```java
 > > public static void main(String[] args) {
 > >  float number = 0.1f;
 > >  
 > >  System.out.println("number : " + number);
 > >  // number : 0.1
 > > }
 > > ```
 > - double
 > > ```java
 > > public static void main(String[] args) {
 > >  double number = 0.01;       
 > >  
 > >  System.out.println("number : " +number);
 > >  // number: 0.01
 > > }
 > > ```

## 형변환

  ##### 5-1. 형변환(캐스팅 Casting)이란?
  - 형변환이란? 
  > 변수 도는 상수의 타입을 다른 타입으로 변환하는 것
  >  - 자동 형변환
  >      - 서로 다른 두타입을 일치시키기 위해서
  >  - 강제 형변환
  >      - 사용자가 강제로 변수의 자료형을 바꿔주는 것
  
  ##### 5-2. 형변환 방법
  - 자동 형변환
      - 기본형 포함범위 포함 관계에서 왼쪽에서 오른쪽으로 이동하는 것은 자동 형변환 

  - 강제 형변환
      - 강제 형변환의 경우는 사용자 바꿀 자료형을 명시적으로 적지 않으면 오류가 발생 
      - 강제 형변환을 한다면 **OverFlow** 형상이 발생할 수 있다.
      ```java
      char c = 'A';
      int a = 10;

      char c = (char)a;

      System.out.println("c : " + c);
      // c : 61
      ```
  **! Tip2.** [아스키코드](https://stepbystep1.tistory.com/10 "아스키코드") <br/>
  **! Tip3.** [오버라이딩과 오버로딩의 차이](https://gmlwjd9405.github.io/2018/08/09/java-overloading-vs-overriding.html "오버라이딩과 오버로딩의 차이") 
  
  ##### 5-3. 정수형과 실수형 간의 형 변환
  - 정수형 간의 형 변환
  > 큰 타입에서 작은 타입으로의 변환, 예를 들어 int타입(4byte)의 값을 byte타입(1byte)으로 변환하는 경우 <br/>
  > 아래와 같은 크기의 만큼 잘려나간다. 그래서 경우에 따라 '값 손실'이 발생한다.
  
   ```java
      System.out.println(300);
      System.out.println((byte)300);
   ```
  
  - 큰 타입(int)에서 작은 타입(byte)으로 변환 / 값 손실 발생 
  ![image](https://user-images.githubusercontent.com/66407386/170480169-b98d8697-987a-41d0-9f1e-ce2447f5ba36.png)

  - 작은 타입(btye)에서 큰 타입(int)으로 변환 / 빈 공간은 부호에 맞춰 0 또는 1로 채워진다.
  ![image](https://user-images.githubusercontent.com/66407386/170480297-10d31b77-3cc0-435b-be76-30d853ef6cdd.png)

  ##### 5-4. 자동 형 변환
  - 자동 형 변환
  > 일반적으로 서로 다른 두 타입간의 덧셈에서는 두 타입 중 표현범위가 더 넓은 타입으로 형변환하여
  > 타입을 일치시킨 다음에 연산을 수행하여 값 손실을 줄이기 위함.
  > 이처럼 연산과정에서 자동적으로 발생하는 형변환을 산술 변환이라고 한다.
  >  - boolean을 제외한 7개(char, String, btye, int, long, short, float)의 기본형은 서로 형 변환이 가능하다.
  >  - 기본형과 참조형은 서로 형 변환이 불가능하다.
  >  - 서로 다른 타입의 변수간의 연산은 형 변환을 하는 것이 원칙이지만, 값의 범위가 작은 타입에서 큰 타입으로의 형변환은 생략
  >    - char와 short는 서로 같은 byte 크기를 갖고 있지만, 부호가 있고 없고의 차이 때문에 서로 형변환이 될 수 없음
  >    - int보다 작은 타입은 자동으로 int로 형변환된다.


<br/>  

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition 
2. [블로그] 밥줄과 취미 사이님의 Java 객체 생성 가이드 - https://dejavuhyo.github.io/posts/java-initialization/
3. [블로그] 헤이베이지님의 형식화된 출력 - https://hbeige.tistory.com/m/16
4. [블고그] Jake, Seo님의 자바의 정석 -변수 (형변환) - https://placeforjake.tistory.com/14
