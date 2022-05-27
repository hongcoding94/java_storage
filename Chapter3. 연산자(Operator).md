# Chapter3. 연산자(Operator)

## 목차
1. [연산자(operator)](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EC%97%B0%EC%82%B0%EC%9E%90operator "연산자(operator)")
    - [1-1. 연산자와 피연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#1-1-%EC%97%B0%EC%82%B0%EC%9E%90%EC%99%80-%ED%94%BC%EC%97%B0%EC%82%B0%EC%9E%90 "연산자와 피연산자")
    - [1-2. 식(式)과 대입연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#1-2-%EC%8B%9D%E5%BC%8F%EA%B3%BC-%EB%8C%80%EC%9E%85%EC%97%B0%EC%82%B0%EC%9E%90 "식(式)과 대입연산자")
    - [1-3. 연산자의 종류](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#1-3-%EC%97%B0%EC%82%B0%EC%9E%90%EC%9D%98-%EC%A2%85%EB%A5%98 "연산자의 종류")
    - [1-4. 연산자의 우선순위와 결합규칙](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#1-4-%EC%97%B0%EC%82%B0%EC%9E%90%EC%9D%98-%EC%9A%B0%EC%84%A0%EC%88%9C%EC%9C%84%EC%99%80-%EA%B2%B0%ED%95%A9%EA%B7%9C%EC%B9%99 "연산자의 우선순위와 결합규칙")
    - [1-5. 산술 변환(usual arithmetic conversion)](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#1-5-%EC%82%B0%EC%88%A0-%EB%B3%80%ED%99%98usual-arithmetic-conversion "산술 변환(usual arithmetic conversion)")
2. [단항 연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EB%8B%A8%ED%95%AD-%EC%97%B0%EC%82%B0%EC%9E%90 "단항 연산자")
    - [2-1. 증감 연산자 - ++, --](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#2-1-%EC%A6%9D%EA%B0%90-%EC%97%B0%EC%82%B0%EC%9E%90------ "증감 연산자 - ++, --")
    - [2-2. 부호 연산자 - +, -](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#2-2-%EB%B6%80%ED%98%B8-%EC%97%B0%EC%82%B0%EC%9E%90----- "부호 연산자 - +, -")
3. [산술 연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EC%82%B0%EC%88%A0-%EC%97%B0%EC%82%B0%EC%9E%90 "산술 연산자")
    - [3-1. 사칙 연산자 - +, -, *, /](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#3-1-%EC%82%AC%EC%B9%99-%EC%97%B0%EC%82%B0%EC%9E%90------- "사칙 연산자 - +, -, *, /")
    - [3-2. 나머지 연산자 - %](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#3-2-%EB%82%98%EB%A8%B8%EC%A7%80-%EC%97%B0%EC%82%B0%EC%9E%90--- "나머지 연산자 - %")
4. [비교 연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EB%B9%84%EA%B5%90-%EC%97%B0%EC%82%B0%EC%9E%90 "비교 연산자")
    - [4-1. 대소비교 연산자 - 〈, 〉, 〈=, 〉=](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#4-1-%EB%8C%80%EC%86%8C%EB%B9%84%EA%B5%90-%EC%97%B0%EC%82%B0%EC%9E%90------ "대소비교 연산자 - 〈, 〉, 〈=, 〉=")
    - [4-2. 등가비교 연산자 - ==, !=](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#4-2-%EB%93%B1%EA%B0%80%EB%B9%84%EA%B5%90-%EC%97%B0%EC%82%B0%EC%9E%90---- "등가비교 연산자 - ==, !=")
5. [논리 연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EB%85%BC%EB%A6%AC-%EC%97%B0%EC%82%B0%EC%9E%90 "논리 연산자")
    - [5-1. 논리 연산자 - &&, ||, !](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#5-1-%EB%85%BC%EB%A6%AC-%EC%97%B0%EC%82%B0%EC%9E%90----- "논리 연산자 - &&, ||, !")
    - [5-2. 비트 연산자 - &, |, ^, ~, 〈〈, 〉〉](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#5-2-%EB%B9%84%ED%8A%B8-%EC%97%B0%EC%82%B0%EC%9E%90-------- "비트 연산자 - &, |, ^, ~, 〈〈, 〉〉")
6. [그 외의 연산자](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EA%B7%B8-%EC%99%B8%EC%9D%98-%EC%97%B0%EC%82%B0%EC%9E%90 "그 외의 연산자")
    - [6-1. 조건 연산자 - ? :](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#6-1-%EC%A1%B0%EA%B1%B4-%EC%97%B0%EC%82%B0%EC%9E%90---- "조건 연산자 - ? :")
    - [6-2. 대입 연산자 - =, op=](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#6-2-%EB%8C%80%EC%9E%85-%EC%97%B0%EC%82%B0%EC%9E%90----op "대입 연산자 - =, op=")
7. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter3.%20%EC%97%B0%EC%82%B0%EC%9E%90(Operator).md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")

---

## 연산자(operator)
  
  - 연산자란?
  > 주어진 식을 계산하여 결과를 얻어내는 과정을 연산이라고 하며, 연산을 수행하는 기호를 연산자라고한다.

   **!Tip0.** [연산자 내용 정리](https://yunjungblog.tistory.com/29 "연산자 내용 정리")

  ##### 1-1. 연산자와 피연산자
  
  - 연산자와 피연산자
  > 연산을 수행하려면 반드시 연산의 대상이 있어야 하는데, 이를 피연산자라고 한다. <br/>
  > A &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; + &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; B <br/>
  > ▲ 피연산자 ▲ 연산자 ▲ 피연산자
  
  ##### 1-2. 식(式)과 대입연산자
  
  - 식
  > 연산자와 피연산자를 조합하여 계산을 하는 방식 <br/>
  > 즉. 하나의 식을 계산하면, 단 하나의 결과를 얻을 수 있다.
  >  - 대입연산자'='를 사용하면 변수와 같이 값을 저장 할 수 있음
  >  - 식을 저장하지 않고 출력만 할 경우, "System.out.println("2 * 2");"으로 식을 써도 무관
  
  ```java
  public static void operation() {
   int i = 0;
   int j = 7;
   int k = 7;
   
   i = j * k;
   System.out.println("i : " + i);
   // i : 49
  }
  ```
  
  ##### 1-3. 연산자의 종류
  <table>
    <tr>
        <th>종류</th>
        <th>연산자</th>
        <th>설명</th>
    </tr>
    <tr>
        <td>증감</td>
        <td> ++   -- </td>
        <td>피연산자에 저장된 값을 1증가 또는 감소</td>
    </tr>
    <tr>
        <td>산술</td>
        <td> +   -   *   /   % </td>
        <td>사칙 연산과 나머지 연산(%)</td>
    </tr>
    <tr>
        <td>시프트</td>
        <td> >>   <<  >>> </td>
        <td>피연산자의 각 비트들을 대상으로 연산</td>
    </tr>
    <tr>
        <td>비교</td>
        <td> >   <   >=   <=   ==   != </td>
        <td>크고 작음과 같고 다름을 비교</td>
    </tr>
    <tr>
        <td>비트</td>
        <td> &   |   ^   ~ </td>
        <td>비트단위 논리 연산</td>
    </tr>
    <tr>
        <td>논리</td>
        <td> &&   ||   !   ^ </td>
        <td>논리연산으로 결과값은 true 또는 false</td>
    </tr>
    <tr>
        <td>조건</td>
        <td> ? : </td>
        <td>조건문으로 참,거짓에 따라 작업을 수행</td>
    </tr>
    <tr>
        <td>대입</td>
        <td> =   *=   /=   +=   -=   &=   ^=   |= </td>
        <td>우변의 값을 좌변에 저장</td>
    </tr>
  </table>
  
  ##### 1-4. 연산자의 우선순위와 결합규칙
  1. 산술 > 비교 > 논리 > 대입 순
  2. 단항(1) > 이항(2) > 삼항(3)
  3. 단항 연산자와 대입 연산자를 제외한 모든 연산자의 진행 방향은 왼쪾에서 오른쪽 진행

  <table>
    <tr>
        <th>종류</th>
        <th>결합규칙</th>
        <th>연산자</th>
        <th>비교</th>
        <th>우선순위</th>
    </tr>
    <tr>
        <td>단항 연산자</td>
        <td> ← </td>
        <td> ++ – + - ~ ! (type) </td>
        <td> + -는 부호연산자임 </td>
        <td> 1 </td>
    </tr>
    <tr>
        <td>산술 연산자</td>
        <td> → </td>
        <td> * / % </td>
        <td></td>
        <td> 2 </td>
    </tr>
    <tr>
        <td>산술 연산자</td>
        <td> → </td>
        <td> + - </td>
        <td> 계산 연산자임 </td>
        <td> 3 </td>
    </tr>
    <tr>
        <td>산술 연산자</td>
        <td> → </td>
        <td> << >> </td>
        <td></td>
        <td> 4 </td>
    </tr>
    <tr>
        <td>비교 연산자</td>
        <td> → </td>
        <td> < > <= >= </td>
        <td> instance of </td>
        <td> 5 </td>
    </tr>
    <tr>
        <td>비교 연산자</td>
        <td> → </td>
        <td> == != </td>
        <td></td>
        <td> 6 </td>
    </tr>
    <tr>
        <td>논리 연산자</td>
        <td> → </td>
        <td> & </td>
        <td></td>
        <td> 7 </td>
    </tr>
    <tr>
        <td>논리 연산자</td>
        <td> → </td>
        <td> ^ </td>
        <td></td>
        <td> 8 </td>
    </tr>
    <tr>
        <td>논리 연산자</td>
        <td> → </td>
        <td> | </td>
        <td></td>
        <td> 9 </td>
    </tr>
    <tr>
        <td>논리 연산자</td>
        <td> → </td>
        <td> && </td>
        <td></td>
        <td> 10 </td>
    </tr>
    <tr>
        <td>논리 연산자</td>
        <td> → </td>
        <td> || </td>
        <td></td>
        <td> 11 </td>
    </tr>
    <tr>
        <td>삼항 연산자</td>
        <td> → </td>
        <td> ?: </td>
        <td></td>
        <td> 12 </td>
    </tr>
    <tr>
        <td>대입 연산자</td>
        <td> → </td>
        <td> = += -= *= /= %= </td>
        <td></td>
        <td> 13 </td>
    </tr>
    <tr>
        <td>대입 연산자</td>
        <td> ← </td>
        <td> «= >>= &= ^= |= </td>
        <td></td>
        <td> 14 </td>
    </tr>
  </table>  

  ##### 1-5. 산술 변환(usual arithmetic conversion)
  
  - 연산 전에 피연산자의 타입을 일치시키는 것 
  >  - 두 피연산자의 타입을 같게 일치시킨다. (보다 큰 타입으로 일치)
  >  - 피연산자의 타입이 int 보다 작은 타입이면 int로 변환 
  
## 단항 연산자

  ##### 2-1. 증감 연산자 - ++, --
  
  <table>
   <tr>
       <th>증감 종류</th>
       <th>설명</th>
   </tr>
   <tr>
       <td> ++ </td>
       <td>증가(increment) 연산자로 항의 값을 1씩 증가 시킨다.</td>
   </tr> 
   <tr>
       <td> -- </td>
       <td>감소(Decrement) 연산자로 항의 값을 1씩 감소 시킨다.</td>
   </tr> 
  </table>
  
  ```java
    public class Main {
      public static void main(String[] args) {
        int i = 2022;
        i++;
        System.out.println(i); // 출력 결과 : 2023
        ++i;
        System.out.println(i); // 출력 결과 : 2024 
        System.out.println(++i); // 출력 결과 : 2025 
        System.out.println(i++); // 출력 결과 : 2026 
        System.out.println(i); // 출력 결과 : 2027 
      }
    }
  ```
  
  
  ##### 2-2. 부호 연산자 - +, -
  
  <table>
   <tr>
       <th>부호 종류</th>
       <th>설명</th>
   </tr>
   <tr>
       <td> + </td>
       <td>양수를 표현한다</td>
   </tr> 
   <tr>
       <td> - </td>
       <td>음수를 표현한다</td>
   </tr> 
  </table>
  
 ```java
    public class Main {
      public static void main(String[] args) {
        int x = 0;
        int i = 2022;
        int j = 1994;
        
        x = i+j; // 출력 결과 : 4016
        x = 0; // 변수 초기화
        
        x = i-j; // 출력 결과 : 28 
        
        
      }
    }
  ```
  
## 산술 연산자

  ##### 3-1. 사칙 연산자 - +, -, *, /
  
  - 사칙연산자
  > 산수의 기본이 되는 덧셈, 뺄셈, 곱셈, 나눗셈의 4가지 연산을 일컫는다.
  
  ```java
  public calass main {
    public static void main(String[] args) {
        int x;   // 0으로 처리
        int i = 2022;
        int j = 94;
        
        // 덧셈(+)
        x = i + j; // 출력 결과 : 2116
        x = 0; // 변수 초기화
        
        // 뺄셈(-) 
        x = i - j; // 출력 결과 : 1928
        x = 0; // 변수 초기화
        
        // 곱셈(*)
        x = i x j; / 출력 결과 : 190068
        x = 0; // 변수 초기화
        
        // 나눗셈(/) - 방식1
        x = i / j; // 출력 결과 : 21.51063829787234
        x = 0; // 변수 초기화
        
        // 나눗셈(/) - 방식2
        x = ((double) i / j); // 출력 결과 : 21.51063829787234
        // 소수 둘째까지 처리
        String formattedResult = String.format("%.2f", x); 
        System.out.println("출력 결과 : " + formattedResult); // 출력 결과 : 21.51  
        x = 0; // 변수 초기화
        
    }
  }
  ```
  
  ##### 3-2. 나머지 연산자 - %
  
  - java에서 나머지 값을 구하는 산술연산자는 %로 표기한다.

  ```java
  public class main {
    public static void main(String[] args) {
        int x;
        int i = 1000;
        int j = 3;
        
        // 나머지 값(%)
        x = i % j; // 출력 결과 : 1
        x = 0; // 변수 초기화
    }
  }
  ```
  
## 비교 연산자

   - 비교 연산자
   > 비교란? 주어진 값들이 같은지, 다른지, 큰지, 작은지를 구분하는 것

   - 비교 연산자종류
   <table>
    <tr>
        <th>기호</th>
        <th>문법</th>
        <th>의미</th>
    </tr>
    <tr>
        <td> == </td>
        <td>i == x</td>
        <td>i와 x가 같은가?</td>
    </tr>
    <tr>
        <td> != </td>
        <td>i != x</td>
        <td>i와 x가 다른가?</td>
    </tr>
    <tr>
        <td> > / < </td>
        <td> i > x / i < x </td>
        <td> i가 x보다 큰가? / i가 x보다 작은가? </td>
    </tr>
    <tr>
        <td> >= / <= </td>
        <td> i >= x / i <= x </td>
        <td> i가 x보다 같거나 큰가? / i가 x보다 같거나 작은가? </td>
    </tr>
    </table>

  ##### 4-1. 대소비교 연산자 - 〈, 〉, 〈=, 〉=

 ```java
 public class main {
    public static void main(String[] args) {
        int i = 60;
        
        // 작다 / 크다 (< / >)
        System.out.println("결과 : " + i > 100); // 출력 결과 : false
        System.out.println("결과 : " + i < 100); // 출력 결과 : true
        
        int j = 1994;
        
        // 같거나 작다 / 같거나 크다 (<= / >=)
        System.out.println("결과 : " + j >= 100); // 출력 결과 : true
        System.out.println("결과 : " + j <= 100); // 출력 결과 : false  
        System.out.println("결과 : " + j <= 1994); // 출력 결과 : true   
        
    }
 }
 ```
  
  ##### 4-2. 등가비교 연산자 - ==, !=
  
  
  
## 논리 연산자

  ##### 5-1. 논리 연산자 - &&, ||, !
  
  ##### 5-2. 비트 연산자 - &, |, ^, ~, 〈〈, 〉〉
  
## 그 외의 연산자

  ##### 6-1. 조건 연산자 - ? :
  
  ##### 6-2. 대입 연산자 - =, op=
  
## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition
  2. [동영상] 생활코딩님의 자바(JAVA) 연산자 中 - [자바(JAVA) 연산자 中](https://edu.goorm.io/lecture/41/%25EB%25B0%2594%25EB%25A1%259C%25EC%258B%25A4%25EC%258A%25B5-%25EC%2583%259D%25ED%2599%259C%25EC%25BD%2594%25EB%2594%25A9-%25EC%259E%2590%25EB%25B0%2594-java "자바(JAVA) 연산자 中")
  3. 
