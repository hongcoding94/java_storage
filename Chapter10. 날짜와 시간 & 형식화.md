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

 - Calendar와 Date
 > - Calendar 클래스 : 추상클래스이기 떄문에 직접 객체를 생성할 수 없고,<br/>
 > 메서드를 통해서 완전히 구현된 클래스의 인스턴스를 얻어야한다.
 > - Date 클래스 : 디폴트 생성자 현재의 날짜와 시간을 가진 객체를 생성<br/>
 > 하지만, 공식문서를 참조하면 **더 이상 사용하지 않으며 언제 지원을 안하는 메소드이므로 사용을 지양하라는 내용이 있다.**

 - Date 🔄 Calendar
     - Date ➡️ Calendar
     > ```java
     > import java.util.Calendar;
     > import java.util.Date; 
     > 
     > public class DateToCalendar {    
     > 	public static void main(String[] args) {                
     > 
     > 	    // 1. 현재 날짜 Date 구하기        
     > 	    Date date = new Date();         
     > 
     > 	    // 2. Calendar 객체 생성        
     > 	    Calendar calendar = Calendar.getInstance();         
     > 
     > 	    // 3. Date 객체를 Calendar로 변환        
     > 	    calendar.setTime(date);         
     > 
     >  	    // 4. Date, Calendar 객체 출력        
     >  	    System.out.println("날짜 : " + date);     
     >  	    System.out.println("캘린더 : " + calendar.getTime());   
     > 	}
     > }
     > ```
     > - 출력결과
     > ```text
     > 날짜 : Sun Jun 20 20:17:48 KST 2021  
     > 캘린더 : Sun Jun 20 20:17:48 KST 2021   
     > ```

    - Calendar ➡️ Date
    >  ```java
    > import java.util.Calendar;
    > import java.util.Date;
    > import java.util.GregorianCalendar; 
    > public class CalendarToDate {   
    > 	public static void main(String[] args) {
    >       // 1. 2021년 6월 20일로 Calendar 생성        
    > 		Calendar calendar = new GregorianCalendar(2021, 6, 20);         
    > 
    > 		// 2. Calendar를 Date로 변경        
    > 		Date date = calendar.getTime();        
    > 
    > 		// 3. Date 출력       
    > 		System.out.println("날짜 : " + date);
    > 	}
    > }
    > ```
    > - 출력결과
    > ```text
    > 날짜 : Tue Jul 20 00:00:00 KST 2021
    > ```

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
 > Referemce 문서 내에 " SimpleDateFormat은 Multi-Thread 환경에서 Safe하지 않는다"라는 내용이 있다.<br/>
 > 즉, 의도치 않은 오류로 인한 결과값이 저장된다면 크게 문제가 발생할 수 있다. ➡️ *해결 방법은 아래 Tip2를 참조*

 **!Tip2.** [pranne1224님의 Java-SimpleDateFormat-위험성과 해결방법](https://velog.io/@pranne1224/Java-SimpleDateFormat-%EC%9C%84%ED%97%98%EC%84%B1)

##### ChoiceFormat

 - ChoiceFormat이란?
 > 특정 범위에 속하는 값을 문자열로 변환

 - ChoiceFormat 문법
 >

##### MessageFormat

 - MessageFormat이란?
 > 데이터를 정해진 양식에 맞게 메시지를 출력

 - MessageFormat 문법
 > 

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
2. [홈페이지] [delftstack 변수 유형 확인하기](https://www.delftstack.com/ko/howto/java/how-to-check-type-of-a-variable-in-java/)
3. [블로그] [devkuma님의 Date 클래스](https://www.devkuma.com/docs/java/date-class/)
