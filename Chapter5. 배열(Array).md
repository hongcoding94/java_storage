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
            arr[i] = i;
            
            // 정식 방식 : 배열에 담을때 int를 String으로 형변환
            arr[i] = Integer.toString(i);
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
  
  
  
  ##### 배열의 초기화
  
  
  ##### 배열의 복사
  
  
  ##### 배열의 활용
  
  
  
## String배열

  ##### String배열의 선언과 생성
  
  
  ##### String배열의 초기화
  
  
  ##### char배열과 String클래스
  
  
  ##### 커맨드 라인을 통해 입력받기
  
  

## 다차원 배열

  ##### 2차원 배열의 선언과 인덱스
  
  
  ##### 2차원 배열의 초기화
  
  
  ##### 가변 배열
  
  
  ##### 다차원 배열의 활용
  
  

## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition
  2. 
