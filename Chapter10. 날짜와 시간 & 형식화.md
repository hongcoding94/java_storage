# Chapter10. 날짜와 시간 & 형식화

## 목차 
1. [날짜와 시간](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#%EB%82%A0%EC%A7%9C%EC%99%80-%EC%8B%9C%EA%B0%84 "날짜와 시간")
    - [1-1. Calendar와 Date](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#calendar%EC%99%80-date "Calendar와 Date")
2. [형식화 클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#%ED%98%95%EC%8B%9D%ED%99%94-%ED%81%B4%EB%9E%98%EC%8A%A4 "형식화 클래스")
    - [2-1. DecimalFormat](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#decimalformat "DecimalFormat")
    - [2-2. SimpleDateFormat](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#simpledateformat "SimpleDateFormat")
    - [2-3. ChoiceFormat](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#choiceformat "ChoiceFormat")
    - [2-4. MessageFormat](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#messageformat "MessageFormat")
3. [java.time패키지](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#javatime%ED%8C%A8%ED%82%A4%EC%A7%80 "java.time패키지")
    - [3-1. java.time패키지의 핵심 클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#javatime%ED%8C%A8%ED%82%A4%EC%A7%80%EC%9D%98-%ED%95%B5%EC%8B%AC-%ED%81%B4%EB%9E%98%EC%8A%A4 "java.time패키지의 핵심 클래스")
    - [3-2. LocalDate와 LocalTime](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#localdate%EC%99%80-localtime "LocalDate와 LocalTime")
    - [3-3. Instant](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#instant "Instant")
    - [3-4. LocalDateTime과 ZonedDateTime](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20%26%20%ED%98%95%EC%8B%9D%ED%99%94.md#localdatetime%EA%B3%BC-zoneddatetime "LocalDateTime과 ZonedDateTime")
    - [3-5. TemporalAdjusters](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#temporaladjusters "TemporalAdjusters")
    - [3-6. Period와 Duration](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#period%EC%99%80-duration "Period와 Duration")
    - [3-7. 파싱과 포맷](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#%ED%8C%8C%EC%8B%B1%EA%B3%BC-%ED%8F%AC%EB%A7%B7 "파싱과 포맷")
4. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter10.%20%EB%82%A0%EC%A7%9C%EC%99%80%20%EC%8B%9C%EA%B0%84%20&%20%ED%98%95%EC%8B%9D%ED%99%94.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")


## 날짜와 시간

##### calendar와 date



## 형식화 클래스

##### DecimalFormat

 - DecimalFormat이란? 
 > 10진수의 값을 원하는 포멧으로 변경해주는 numberFormat의 구상 서브 클래스 

 **!Tip1.** [DecimalFormat의 자세한 설명](http://cris.joongbu.ac.kr/course/2019-1/jcp/api/java/text/DecimalFormat.html)

 - DecimalFormat의 사용 방법
 >  - DecimalFormat을 이용하면 숫자 데이터를 정수, 부동소수점, 금액 등의 다양한 형식으로 표현
 >  - 반대로 일정한 형식의 텍스트 데이터를 숫자로 쉽게 변환
 >  - 형식화 클래스는 패턴을 정의하는 것이 전부

 - Decimalformat의 코드 문법
 ```java
 // 선언 - 문법 선언
 DecimalFormat testDF1 = new DecimalFormat();
 // 선언 - 특정 format방식으로 지원
 DecimalFormat testDF2 = new DecimalFormat("0000,0000.00"); // 만자리
 
 double num = testDF1.parse("123,456.78");
 double num2 = testDF2.parse("123,456.78");
 
 System.out.println("출력 값_1 : " + num.format(num));
 System.out.println("출력 값_2 : " + num2.format(num2));
 ```
 
 - 출력 결과
 ```text
 출력 값_1 : 123,456.78
 출력 값_2 : 123,456.78
 ```
 
##### SimpleDateFormat

 - SimpleDateFormat이란?
 > Java7버전에서 제공하는 클래스이며 역할은 아래와 같다.
 >  - String을 파싱하여 Date 객체를 생성한다.
 >  - Date 객체를 formatting하여. String 한다.
 
 
 - SimpleDateFormat을 쓰지 말아야하는 이유
 > 

##### ChoiceFormat

##### MessageFormat

## java.time패키지

##### java.time패키지의 핵심 클래스
 
 - java.time 패키지의 핵심 클래스
 > 날짜와 시간이 별도로 분리되어 있어 따로 사용할 수 있고, 합쳐진 클래스로 사용할 수 있다.
 >  - LocalDate : 날짜
 >  - LocalTime : 시간
 >  - Instant : 날짜 시간 초단위로 나타냄(타임스탬프)
 >  - LocalDateTime : 날짜 시간
 >  - ZonedDateTime : 날짜 시간 시간대
 
##### LocalDate와 LocalTime

##### Instant

##### LocalDateTime과 ZonedDateTime

##### TemporalAdjusters

##### Period와 Duration

##### 파싱과 포맷

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
