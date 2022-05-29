# Chapter5. 배열(Array)

## 목차

1. [배열(array)](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4array "배열(array)")
    - [1-1. 배열(array)이란?](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4array%EC%9D%B4%EB%9E%80 "배열(array)이란?")
    - [1-2. 배열의 선언과 생성](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%84%A0%EC%96%B8%EA%B3%BC-%EC%83%9D%EC%84%B1 "배열의 선언과 생성")
    - [1-3. 배열의 길이와 인덱스](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4%EC%9D%98-%EA%B8%B8%EC%9D%B4%EC%99%80-%EC%9D%B8%EB%8D%B1%EC%8A%A4 "배열의 길이와 인덱스")
    - [1-4. 배열의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94 "배열의 초기화")
    - [1-5. 배열의 복사](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4%EC%9D%98-%EB%B3%B5%EC%82%AC "배열의 복사")
    - [1-6. 배열의 활용](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%B0%B0%EC%97%B4%EC%9D%98-%ED%99%9C%EC%9A%A9 "배열의 활용")
2. [String배열](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#string%EB%B0%B0%EC%97%B4 "String배열")
    - [2-1. String배열의 선언과 생성](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#string%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%84%A0%EC%96%B8%EA%B3%BC-%EC%83%9D%EC%84%B1 "String배열의 선언과 생성")
    - [2-2. String배열의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#string%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94 "String배열의 초기화")
    - [2-3. char배열과 String클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#char%EB%B0%B0%EC%97%B4%EA%B3%BC-string%ED%81%B4%EB%9E%98%EC%8A%A4 "char배열과 String클래스")
    - [2-4. 커맨드 라인을 통해 입력받기](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EC%BB%A4%EB%A7%A8%EB%93%9C-%EB%9D%BC%EC%9D%B8%EC%9D%84-%ED%86%B5%ED%95%B4-%EC%9E%85%EB%A0%A5%EB%B0%9B%EA%B8%B0 "커맨드 라인을 통해 입력받기")
3. [다차원 배열](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%8B%A4%EC%B0%A8%EC%9B%90-%EB%B0%B0%EC%97%B4 "다차원 배열")
    - [3-1. 2차원 배열의 선언과 인덱스](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#2%EC%B0%A8%EC%9B%90-%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%84%A0%EC%96%B8%EA%B3%BC-%EC%9D%B8%EB%8D%B1%EC%8A%A4 "2차원 배열의 선언과 인덱스")
    - [3-2. 2차원 배열의 초기화](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#2%EC%B0%A8%EC%9B%90-%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%B4%88%EA%B8%B0%ED%99%94 "2차원 배열의 초기화")
    - [3-3. 가변 배열](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EA%B0%80%EB%B3%80-%EB%B0%B0%EC%97%B4 "가변 배열")
    - [3-4. 다차원 배열의 활용](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EB%8B%A4%EC%B0%A8%EC%9B%90-%EB%B0%B0%EC%97%B4%EC%9D%98-%ED%99%9C%EC%9A%A9 "다차원 배열의 활용")
4. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter5.%20%EB%B0%B0%EC%97%B4(Array).md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")

---

## 배열(array)

  ##### 배열(array)이란?
  
  - 배열이란?
  > 연관된 데이터를 모아서 관리하기 위해서 사용되는 데이터 타입 <br/>
  > 단일의 데이터를 변수로 저장한다면 배열은 여러 개의 데이터를 저장하는 것.
  
  ##### 배열의 선언과 생성
 
  - 배열 선언 방식
  > 타입[] 변수이름;              &nbsp; : 배열 선언 (배열을 다루기 위한 참조변수) <br/>
  > 변수이름 = new 타입[길이];     &nbsp; :  생성(실제 저장 공간 생성)
  
  ```java
  public class main {
    public static main(String[] args) {
        String[] arr = new String[4];
    }
  }
  ```
  
  - 배열 생성하면 컴퓨터에 메모리에 크기 4 만큼의 임의의 공간을 할당해서 사용자가 사용할 수 있도록 할당한다.
  <table>
    <tr>
        <th>1001</th>
        <th>1002</th>
        <th>1003</th>
        <th>1004</th>
        <th>1005</th>
        <th>1006</th>
        <th>1007</th>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>null [0]</td>
        <td>null [1]</td>
        <td>null [2]</td>
        <td>null [3]</td>
        <td></td>
    </tr>
    <tr>
        <td> </td>
        <td> </td>
        <td> - </td>
        <td> - </td>
        <td> - </td>
        <td> - </td>
        <td> </td>
    </tr>
  </table>
  
  - 예시
  ```java
  public class main {
    public static void main(String[] args) {
        String arr = new String[5];
        
        for(int i=0; i<6; i++) {
            // 잘못된 방식 : error : java.lang.NumberFormatException
            // arr[i] = i;
            
            // 정식 방식 : 배열에 담을때 int를 String으로 형변환
            arr[i] = Integer.toString(i);
            System.out.println(Arrays.toString(arr));
        }
    }
  }
  ```
  -  출력 결과
  <table>
    <tr>
        <th>1007</th>
        <th>1008</th>
        <th>1009</th>
        <th>1010</th>
        <th>1011</th>
    </tr>
    <tr>
        <td>[0]</td>
        <td>[1]</td>
        <td>[2]</td>
        <td>[3]</td>
        <td>[4]</td>
    </tr>
    <tr>
        <td> 1 </td>
        <td> 2 </td>
        <td> 3 </td>
        <td> 4 </td>
        <td> 5 </td>
    </tr>
  </table>
  
  ##### 배열의 길이와 인덱스
  
  - 배열의 인덱스(index)
  > 배열의 각 저장공간을 '배열의 요소'라고 한다. <br/>
  > '배열이름[index]'의 형식으로 배열의 요소에 접근한다. <br/>
  > index는 배열의 공간의 일련번호이며 각 요소를 구별하는데 사용한다. index의 범위는 0부터 지정한 배열의 길이-1까지이다.
  
  - 배열의 길이 (배열이름.length)
  > 배열은 한번 생성하면 길이를 변경할 수 없기 때문에 배열이름.legth는 상수이며 값을 읽을 수만 있고 변경 할 수 없다.
  ```java
  public class main {
    public static void main(String[] args) {
        int[] array = new int[4];
        
        int len = array.length;
        
        System.out.println("결과 출력 : " + len);
        // 결과 출력 : 4
    }
  }
  ```
  
  ##### 배열의 초기화
  
  > 배열은 생성과 동시에 자동적으로 기본값(0)으로 초기화되기 때문에 배열을 <br/>
  > 사용하기 전에 따로 초기화를 해주지 않아도 되지만 원하는 값을 저장하려면 각 요소마다 값을 지정해 주어야 한다.

  - 배열의 생성과 초기화
  ```java
  public class main {
    public static void main(String[] args) {
        // 방법 1
        int[] arr1 = new int[4];
        
        arr1[0] = 10;
        arr1[1] = 20;
        arr1[2] = 30;
        arr1[3] = 40;
        
        // 방법 2
        int[] arr2 = new int[]{10, 20, 30, 40};
        // 혹은
        int[] arr2 = {10, 20, 30, 40};  // arr2 int[]를 생략할 수 있다.
    }
  }
  ``` 

  - for문을 이용한 배열 초기화
  ```java
  public class main {
    public static void main(String[] args) {
        int[] arr = new int[4];
        
        for(int i=0; i<arr.length; i++) {
            arr[i] = i * 10;
        }
    }
  }
  ```
  
  ##### 배열의 복사
  
  - 배열의 복사 arraycopy
  > System.arraycopy(**원본 배열, 복사를 시작할 위치, 새로운 배열, 복사를 붙여넣을 위치, 복사할 요소의 개수**); <br/>
  > 만약, 배열의 공간이 **복사하려는 내용보다 작으면 에러(ArrayIndexOutOfBoundsException)를 발생**한다.
  
  ##### 배열의 활용
  
- Lotto
```java
public class Lotto {
    public static void main(String[] args) {
        // 섞기(Shuffle)  배열의 요소의 순서를 반복해서 바꾼다. (숫자 섞기, 로또번호 생성) 
        int[] ball = new int[45];

        for(int i =0; i<ball.length; i++)
            ball[i] = i+1;            //ball[0] = 1이 저장 

        int tmp = 0; 
        int j = 0; 

        for(int i =0; i<6; i++) {
            j=(int)(Math.random()*45); //0~44까지의 범위 
            tmp = ball[i];
            ball[i] = ball[j];
            ball[j] = tmp;
        }

        for(int i =0; i<6;i++) {
            System.out.printf("ball[%d]=%d%n",i,ball[i]);
        }

        for(int i =0; i<6; i++) {
            System.out.print(ball[i]+" ");
        }
    }
}
```

  - 가위바위보
  ```java
  import java.util.Arrays;
 
    public class rock_Paper_Scissors {
        public static void main(String[] args) {
            // TODO Auto-generated method stub
            String[] strArr = {"가위","바위","보"};

            System.out.println(Arrays.toString(strArr));
            for(int i =0; i<3; i++) {
                int tmp = (int)(Math.random()*3);
                System.out.println(strArr[tmp]);
            }
        }
    }
  ```
  
  - 배열 순서 섞기
  ```java
  import java.util.Arrays;
 
    public class arrRandom {

        public static void main(String[] args) {
            // 섞기(Shuffle)  배열의 요소의 순서를 반복해서 바꾼다. (숫자 섞기, 로또번호 생성) 
            int[] numArr = {0,1,2,3,4,5,6,7,8,9};
            System.out.println(Arrays.toString(numArr));

            for(int i = 0; i<numArr.length; i++) {
                int n = (int)(Math.random() *10);      // 0~9 임의의 수 
                int tmp = numArr[i];
                numArr[i] = numArr[n];
                numArr[n] = tmp;

            }
            System.out.println(Arrays.toString(numArr));
        }
    }
  ```
  
## String배열

  ##### String배열의 선언과 생성
  
  - String 배열
  > 기본 배열과 선언 방법과 생성 방법은 다르지 않다.
  ```java
  public class main {
    public static void main(String[] args) {
        String[] country = new String[3];
    }
  }
  ```
   <table>
    <tr>
        <th>1011</th>
        <th>1012</th>
        <th>1013</th>
    </tr>
    <tr>
        <td>[0]</td>
        <td>[1]</td>
        <td>[2]</td>
    </tr>
    <tr>
        <td> null </td>
        <td> null </td>
        <td> null </td>
    </tr>
  </table>
  
  - String클래스의 주요 메서드
  <table>
     <tr>
        <th>메서드</th>
        <th>설명</th>
    </tr>
    <tr>
        <td> char charAt(int index) </td>
        <td> 문자열에서 해당 위치(index)에 있는 문자를 반환  </td>
    </tr>
    <tr>
        <td> int length() </td>
        <td> 문자열의 길이를 반환한다. </td>
    </tr>
    <tr>
        <td> String substring(int from, int to) </td>
        <td> 문자열에서 해당 범위(from ~ to)에 있는 문자열을 반환 to는 범위에 포함되지 않는다. </td>
    </tr>
    <tr>
        <td> boolean equals(String str) </td>
        <td> 문자열의 내용이 같은지 확인한다. 같으면 결과는 true, 다르면 false이 된다. </td>
    </tr>
    <tr>
        <td> char[] toCharArray() </td>
        <td> 문자열을 문자배열(char[])로 변환하여  </td>
    </tr>
  </table>
  
  ##### String배열의 초기화

  - String 배열의 초기화 생성
  ```java
  public class main {
    public static void main(String[] args) {
        // 방법 1
        String[] country = new String[3];
        
        company[0] = 'KOR';
        company[1] = 'USA';
        company[2] = 'JPN';
        
        // 방법 2
        String[] country = new String[]{'KOR', 'USA', 'JPN'};
        // 혹은
        String[] country = {'KOR', 'USA', 'JPN'};  // new String[]를 생략할 수 있다.
    }
  }
  ```  
  
  
  ##### char배열과 String클래스
  
  > String클래스는 char배열에 기능(메서드)을 추가한 것 <br/>
  > 단, char배열과 String클래스의 한 가지 중요한 차이가 있다. <br/>
  > String객체(문자열)는 읽을 수만 있을 뿐 내용을 변경할 수 없다.

  ```java
  public class main {
    public static void main(String[] args) {
        String[] ch = new String[10]; 
        String str = 'helloJava';  

        for(int i=0; i< str.legnth; i++) {
            ch[i] = str.charAt(i);
        }
    }
  }
  ```
  <table>
    <tr>
        <th>1017</th>
        <th>1018</th>
        <th>1019</th>
        <th>1020</th>
        <th>1021</th>
        <th>1022</th>
        <th>1023</th>
        <th>1024</th>
        <th>1025</th>
        <th>1026</th>
    </tr>
    <tr>
        <td>[0]</td>
        <td>[1]</td>
        <td>[2]</td>
        <td>[3]</td>
        <td>[4]</td>
        <td>[5]</td>
        <td>[6]</td>
        <td>[7]</td>
        <td>[8]</td>
        <td>[9]</td>
    </tr>
    <tr>
        <td>h</td>
        <td>e</td>
        <td>l</td>
        <td>l</td>
        <td>o</td>
        <td>J</td>
        <td>a</td>
        <td>v</td>
        <td>a</td>
        <td> null </td>
    </tr>  
  </table>
  
  ##### 커맨드 라인을 통해 입력받기
  
  

## 다차원 배열

  ##### 2차원 배열의 선언과 인덱스
  
  - 2차원 선언 방식과 인덱스 
  > 1. 타입[][] 변수이름;
  > 2. 타입 변수이름[][];
  > 3. 타입[] 변수이름[];
  > 행 index의 범위는 0~행의 길이-1 이며, 열 index의 범위는 0~열의 길이-1
  
  ```java
  public class main {
    public static void main(String[] argd) {
        int[][] arr = new int[3][2];
    }
  }
  ```
  <table>
    <tr>
       <th>1000</th>
       <th>1001</th>
       <th>1002</th>
    </tr>
    <tr>
       <td>1004</td>
       <td>-</td>
       <td>-</td>
    </tr>
    <tr>
       <td>1005</td>
       <td>-</td>
       <td>-</td>
    </tr>
    <tr>
       <td>1006</td>
       <td>-</td>
       <td>-</td>
    </tr>
  </table>
  
  ##### 2차원 배열의 초기화
  ```java
  public class main {
    public static void main(String[] args) {
        // 방법 1
        // 2차원 배열의 선언
        int[][] arr1;
        
        // 2차원 배열의 초기화
        arr1 = new int[2][3];
        
        // 방법 2
        // 선언 및 동시에 초기화 하는방법
        int[] [] arr2 = new int[2][3];
        
        // 방법 3
        int[][] arr3 = {{1,2}, {1,2,3}};
    }
  }
  ```
  
  ##### 가변 배열
  
  
  ##### 다차원 배열의 활용
  
  - 좌표에 X표 구하기
 ```java
 import java.util.Scanner;
 import java.util.concurrent.CountDownLatch;

  public class main {
    public static void main(String[] args) {
        final int SIZE = 10;
		int x=0, y=0;
		
		char[][] board = new char [SIZE][SIZE];
		byte[][] shipBoard = {
			   //1,2,3,4,5,6,7,8,9
				{0,0,0,0,0,0,1,0,0},
				{1,1,1,1,0,0,1,0,0},
				{0,0,0,0,0,0,1,0,0},
				{0,0,0,0,0,0,1,0,0},
				{0,0,0,0,0,0,0,0,0},
				{1,1,0,1,0,0,0,0,0},
				{0,0,0,1,0,0,0,0,0},
				{0,0,0,1,0,0,0,0,0},
				{0,0,0,0,0,1,1,1,0}
		};
		
		for(int i=1; i<SIZE; i++)
			board[0][i] = board[i][0] = (char)(i+'0');
		
		Scanner scanner = new Scanner(System.in);
		
		while(true) {
			System.out.printf("좌표를 입력하세요 (종료 00) : ");
			String input = scanner.nextLine();
			
			if(input.length()==2) {
				x = input.charAt(0) - '0'; //문자를 숫자로 변환
				y = input.charAt(1) - '0';
				
				if(x==0 && y==0)
					break;
			}
			
			if(input.length() != 2 || x<=0 || x>=SIZE || y<=0 || y>=SIZE) {
				System.out.println("잘못된 입력입니다. 다시 입력해주세요.");
				continue;
			}
			
			board[x][y] = shipBoard[x-1][y-1]==1 ? '0' : 'x';
			
			for(int i=0; i<SIZE; i++) {
				System.out.println(board[i]);
			}
			System.out.println();
		}
    }
  }
  ```
  
  - 단어 맞추기
  ```java
  import java.util.Scanner;

  public class main {
    public static void main(String[] args) {
        String[][] words = {
				{"chair", "의자"},
				{"computer", "컴퓨터"},
				{"integer", "정수"}
		};
		
		Scanner scanner = new Scanner(System.in);
		
		for(int i=0; i<words.length; i++) {
			System.out.printf("Q%d. %s의 뜻은?", i+1, words[i][0]);
			
			String tmp = scanner.nextLine();
			
			if(tmp.equals(words[i][1])) {
				System.out.printf("정답입니다. %n%n");
			}else {
				System.out.printf("틀렸습니다. 정답은 %s입니다. %n%n", words[i][1]);
			}
		}
    }
  }
  ```
  
  **Tip0.** [다차원 배열의 이해](https://better-tomorrow.tistory.com/entry/%EB%8B%A4%EC%B0%A8%EC%9B%90-%EB%B0%B0%EC%97%B416-1-%EB%8B%A4%EC%B0%A8%EC%9B%90-%EB%B0%B0%EC%97%B4%EC%9D%98-%EC%9D%B4%ED%95%B4%EC%99%80-%ED%99%9C%EC%9A%A9 "다차원 배열의 이해")

## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition
  2. [블로그] 무니의 개발 로그님의 배열내용 - https://devmoony.tistory.com/20 
  3. [블로그] hi.anna님의 가변 길이 배열 - https://hianna.tistory.com/518
  4. [서적] 윤성우님의 열혈 java 프로그래밍
  5. [블로그] 심플심플심플심플님의 2차 배열에 대한 내용 - https://simplex3510.tistory.com/214


