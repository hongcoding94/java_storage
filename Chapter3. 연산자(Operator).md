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

  - 연산자의 종류
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

  ##### 1-1. 연산자와 피연산자
  
  - 연산자와 피연산자
  > 연산을 수행하려면 반드시 연산의 대상이 있어야 하는데, 이를 피연산자라고 한다. <br/>
  > A &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; + &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; B <br/>
  > ▲ 피연산자 ▲ 연산자 ▲ 피연산자
  
  ##### 1-2. 식(式)과 대입연산자
  
  
  ##### 1-3. 연산자의 종류
  
  
  ##### 1-4. 연산자의 우선순위와 결합규칙


  ##### 1-5. 산술 변환(usual arithmetic conversion)
  
  
## 단항 연산자

  ##### 2-1. 증감 연산자 - ++, --
  
  ##### 2-2. 부호 연산자 - +, -
  
## 산술 연산자

  ##### 3-1. 사칙 연산자 - +, -, *, /
  
  ##### 3-2. 나머지 연산자 - %
  
## 비교 연산자

  ##### 4-1. 대소비교 연산자 - 〈, 〉, 〈=, 〉=
  
  ##### 4-2. 등가비교 연산자 - ==, !=
  
## 논리 연산자

  ##### 5-1. 논리 연산자 - &&, ||, !
  
  ##### 5-2. 비트 연산자 - &, |, ^, ~, 〈〈, 〉〉
  
## 그 외의 연산자

  ##### 6-1. 조건 연산자 - ? :
  
  ##### 6-2. 대입 연산자 - =, op=
  
## 참고 문서 / 블로그
  1. [서적] 남궁성님의 Java의 정석 3rd Edition

