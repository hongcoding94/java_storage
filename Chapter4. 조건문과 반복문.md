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
  > 조건의 참, 거짓을 구분지어 서로 다른 작업을 수행을 도와주는 구문 <br/>
  > - 조건문의 종류 <br/>
  >     - if문 / if-else <br/>
  >     - 중첩 if문 <br/>
  >     - swith문 <br/>
    
  <table>
    <tr>
        <th> for 문을 사용하는 경우 </th>
        <th>while 문을 사용하는 경우 </th>
    </tr>
    <tr>
        <td>
            1. 반복 횟수가 정해진 경우 <br/>
            2. 배열과 함께 주로 많이 사용
        </td>
        <td>
           1. 무한 루프나 특정 조건에 만족할 때까지 반복해야하는 경우 <br/>
           2. 주로 파일을 읽고 쓰기에 많이 사용 
        </td>
    </tr>
  </table>

  ##### 1-1. if문
  ```java
  public class main {
    public static void main(String[] args) {
        int i = 1;

        if(i >= 1) {
            System.out.println("출력결과 : 조건 (if)");
        }
        
        // 출력결과 : 조건 성공(if)
    }
  }
  ```

  ##### 1-2. if-else문
  ```java
  public class main {
    public static void main(String[] args) {
        int i = 1;

        if(i > 0) {
            System.out.println("출력결과 : 조건 (if)");
        } else {
            System.out.println("출력결과 : 다른 조건 (else)");
        }
        
        // 출력결과 : 조건 실패(else)
    }
  }
  ```
  
  ##### 1-3. if-else if문
  ```java
  public class main {
    public static void main(String[] args) {
        int i = 0;
        
        if(0 < 2002) {
            System.out.println("출력결과 : 조건 (if)");
        } else if(0 == 0) {
            System.out.println("출력결과 : 다른 조건 1(else-if)");
        } else {
            System.out.println("출력결과 : 다른 조건 2(else)");
        }
        
        // 출력결과 : 다른 조건 1(else-if)
    }
  }
  ```

  ##### 1-4. 중첩 if문
  ```java
  public class main {
    public static void main(String[] args) {
        int i = 2002;
        int j = 2022;
        
        if(i<2022) {
            System.out.println("출력결과 : " + i + "년 입니다.");
        }
        
        if(j == 2022) {
            System.out.println("출력결과 : " + j + "년 입니다.");
        }

        // 출력결과 : 2022년입니다.
    }  
  }
  ```
  
  ##### 1-5. switch문
  ```java
  public class main {
    public static void main(String[] args) {
        String string = "B";
        
        swith(string) {
            //만약 값이 A라면 다음 내용 출력
            case "A" :
                ...
                break;
                //만약 값이 B라면 다음 내용 출력
                case "B" :
                ...
                break;
                //만약 값이 C라면 다음 내용 출력
                case "C" :
                ...
                break;
                //그 외의 값이라면 다음 내용 출력
                default :
                ...
         }
    }
  }
  ```

## 반복문 - for, while, do-while

  - 반복문이란?
  > 어떤 코드들을 반복적으로 실행되도록 할때 사용한다.
  >  - 반복문의 종류
  >     - for문
  >     - while문 / do - while문

  ##### 2-1. for문
  
  - for문이란?
  > 반복 횟수를 알고 있을 때 사용한다.
  ```java
  public class main {
   public static void main(String[] args) {
     int testNum = 5;
     
     for(int i = 0; i<=testNum; i++) {
        System.out.println("출력 결과 : " + i);
     }
     
     // 출력결과 
     // 출력 결과 : 1
     // 출력 결과 : 2
     // 출력 결과 : 3
     // 출력 결과 : 4
     // 출력 결과 : 5
   }
  }
  ```
  
  ##### 2-2. while문
  
  - while문이란?
  >  조건식이 true일 경우에 계속해서 반복 <br/>
  >  비교 또는 논리 연산식이 주로 오는데, 조건식이 false가 되면 반복 행위를 멈추고 while문을 정지한다. <br/>
  >  단, 조건이 맞지 않으면 무한 루프가 돌 수 있기 때문에 조건을 잘 주어야한다.
  
  ```java
  public class main {
   public static void main(String[] args) {
        int treeHit = 0;
        
        while (treeHit < 3) {
            treeHit++;
            System.out.println("나무를  " + treeHit + "번 찍었습니다.");
            if (treeHit == 3) {
                System.out.println("나무 넘어갑니다.");
            }
        }
	
	// 출력 결과
	// 나무를 1번 찍었습니다.
	// 나무를 2번 찍었습니다.
	// 나무를 3번 찍었습니다.
	// 나무 넘어갑니다.
   }
  }
  ```
  **!Tip0.** [while문](https://wikidocs.net/212 "While문")

  ##### 2-3. do-while문

  ```java
  public class main {
   public static void main(String[] args) {
        int i = 1; 
        
	do {
		System.out.println("출력결과 : " + i); // 실행문
		i++; // 증감식
	} while (i <= 5); // 조건식
   
    // 출력결과
    // 출력결과 : 1 
    // 출력결과 : 2
    // 출력결과 : 3
    // 출력결과 : 4
   }
  }
  ```

  ##### 2-4. break문
  
  ```java
  public class main {
   public static void main(String[] args) {
        int i = 0;
	
	while(true){  // 특별한 제어가 없다면 이 while문은 무한으로 반복한다.
	    if(i == 3){  // i가 3이 되면 if문 실행
		break;      // 멈춘다
	    }
	    i++;
	}
   }
  }
  ```
  
  ##### 2-5. continue문
  
  ```java
  public class main {
   public static void main(String[] args) {
        int i = 0;
        
        while(i < 10) {
            i++;
            if(i % 2 == 0) {
                continue;
            }
            System.out.println("출력결과 : " + i);
        }
   }
  }
  
  // 출력 결과
  // 출력 결과 : 1
  // 출력 결과 : 3
  // 출력 결과 : 5
  // 출력 결과 : 7
  // 출력 결과 : 9
  ```
  
  ##### 2-6. 이름 붙은 반복문
  
  ```java
  public class main {
   public static void main(String[] args) {
    outer:
	while(true) {
	    ···
	    for(;;) {
		···
		if(num==0){    
		    break;   // for문을 벗어난다
		    continue // for문의 시작으로 돌아간다.
		}
		if(num==9){ 
		    break outer;    // for문과 while문 모두 벗어난다.
		    continue outer; // while문의 시작으로 돌아간다.
		}
	    }
	}
   }
  }
  ```
  
## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition
  2. 애송이의 코딩이야가님의 continue와 break - https://mjn5027.tistory.com/94
  3. 둔덩님의 자바 반복문 알고 쓰자 - https://tecoble.techcourse.co.kr/post/2020-08-31-java-loop/
