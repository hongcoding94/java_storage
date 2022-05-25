# Chapter 2 변수(Variable)

## 목차
1. [변수와 상수](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EC%99%80-%EC%83%81%EC%88%98 "변수와상수")
   - [?]( "")
   - [?]( "")
2. [변수의 타입](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EB%B3%80%EC%88%98%EC%9D%98-%ED%83%80%EC%9E%85 "변수의타입")
   - [2-1. 기본 변수들의 설명](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#1-1-%EA%B8%B0%EB%B3%B8-%EB%B3%80%EC%88%98%EB%93%A4%EC%9D%98-%EC%84%A4%EB%AA%85 "2-1. 기본 변수들의 설명")
   - [2-2. 변수들의 선언 방법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#1-2-%EB%B3%80%EC%88%98%EB%93%A4%EC%9D%98-%EC%84%A0%EC%96%B8-%EB%B0%A9%EB%B2%95- "2-2. 변수들의 선언 방법")
3. [진법](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EC%A7%84%EB%B2%95 "진법")
   - [3-1]( "")
4. [기본형](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EA%B8%B0%EB%B3%B8%ED%98%95 "기본형")
   - [4-1]( "")
5. [형변환](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%ED%98%95%EB%B3%80%ED%99%98 "형변환")
   - [5-1]( "")     
6. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter%202%20%EB%B3%80%EC%88%98(Variable).md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "")

---
### 변수와 상수
#### ?



### 변수의 타입

   ##### 2-1. 기본 변수들의 설명<br/>
      <table>
      <tr>
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
             <td>	문자(character)를 저장하기 위한 타입</td>
           </tr>
           <tr>
             <td>여러문자</td>
             <td>String</td>
             <td>여러 문자(문자열, string)를 저장하기 위한 타입</td>
           </tr>
        </tr> 
      </table>
   
  ##### 2-2. 변수들의 선언 방법 <br/>
   
   ```java
      public Class object extends * () {
       // Vo 선언 방식 현재 많이 쓰는 방식 기준으로 정렬해봤습니다.
       /* 문자열 */
       private String   str;
      
       /* 정수 */
       private int      cnt;
       private integer  cnt2;
       private long     cnt3;
      
       /* 문자 */
       private char     strYn;
       
       /* 논리형 */
       private Boolean  trueOrFalse;
      }
   //
   ```
   
  **! Tip0.** [private와 public의 차이 - 접근 지정자](https://luyin.tistory.com/232 "private와 public의 차이")

2. 기본 변수들의 크기<br/>
   |종류/크기|1Byte|2Byte|3Byte|4Byte|
   |:---:|:---:|:---:|:---:|:---:|
   |논리형|boolean|    | | 	| 	 
   |문자형|       |char| |    |	 	 	 	 
   |정수형|byte|short|int|long| 	 	 	 
   |실수형|     ||float|double|	 	 	 


### 진법
#### ?


### 기본형
#### ?


### 형변환
#### ?


### 참고 문서 / 블로그
#### ?
