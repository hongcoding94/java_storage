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
 > - Date 클래스 : 컴퓨터의 현재 날짜와 시간을 가진 객체를 생성<br/>
 > 하지만, 공식문서를 참조하면 **더 이상 사용하지 않으며 언제 지원을<br/>안 하는 메소드이므로 사용을 지양하라는 내용이 있다.**
 >      - 공식문서 참조 내용 
 >      ![image](https://user-images.githubusercontent.com/66407386/173265363-8ce6e0cd-9d18-4bcf-aef6-d355898d4579.png)
 
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

 - DecimalFormat 문법 정의
    <table>
        <tr>
            <th>문법</th>
            <th>문법 내용</th>
            <th>적용 문법</th>
            <th>반응 문법</th>
        </tr>
        <tr>
            <td>0</td>
            <td>10진수(빈자리는 0)</td>
            <td>0<br>0.0<br>00000.000</td>
            <td>123<br>123.4<br>00123.400</td>
        </tr>
        <tr>
            <td>#</td>
            <td>10진수(빈자리 비워둠)</td>
            <td>#<br>#.#<br>#####.###</td>
            <td>123<br>123.4<br>123.4</td>
        </tr>
        <tr>
            <td>.</td>
            <td>소수점</td>
            <td>#.0</td>
            <td>123.4</td>
        </tr>
        <tr>
            <td>-</td>
            <td>음수 기호</td>
            <td>+#.0<br>-#.0</td>
            <td>+123.4<br>-123.4</td>
        </tr>
        <tr>
            <td>,</td>
            <td>단위 구분</td>
            <td>#,###.0</td>
            <td>1,234,567.8</td>
        </tr>
        <tr>
            <td>E</td>
            <td>지수 문자</td>
            <td>0.0E0</td>
            <td>1.2E6</td>
        </tr>
        <tr>
            <td>;</td>
            <td>양수와 음수의 패턴을 모두 기술할 경우, 패턴 구분자</td>
            <td>+#,###;-#,###</td>
            <td>+1,234(양수일 때)<br>-1,234(음수일 때)</td>
        </tr>
        <tr>
            <td>%</td>
            <td>% 문자</td>
            <td>#.# %</td>
            <td>123.4 %</td>
        </tr>
        <tr>
            <td>\u00A4</td>
            <td>통화 기호</td>
            <td>\u00A4 #,###</td>
            <td>\(돈 모양) 1,234,567</td>
        </tr>
    </table>

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
 
 - SimpleDateFormat 문법 정의
    <table>
        <tr>
            <th>문법</th>
            <th>문법 내용</th>
            <th>문법</th>
            <th>문법 내용</th>
        </tr>
        <tr>
            <td>y</td>
            <td>년</td>
            <td>H</td>
            <td>시(0~23)</td>
        </tr>
        <tr>
            <td>M</td>
            <td>월</td>
            <td>h</td>
            <td>시(1~12)</td>
        </tr>
        <tr>
            <td>d</td>
            <td>일</td>
            <td>K</td>
            <td>시(0~11)</td>
        </tr>
        <tr>
            <td>D</td>
            <td>월 구분이 없는 일(1~365)</td>
            <td>k</td>
            <td>시(0~24)</td>
        </tr>
        <tr>
            <td>E</td>
            <td>요일</td>
            <td>m</td>
            <td>분</td>
        </tr>
        <tr>
            <td>a</td>
            <td>오전/오후</td>
            <td>s</td>
            <td>초</td>
        </tr>
        <tr>
            <td>w</td>
            <td>년의 몇 번째 주</td>
            <td>S</td>
            <td>밀리세컨드(1/1000초)</td>
        </tr>
        <tr>
            <td>W</td>
            <td>월의 몇 번째 주</td>
            <td></td>
            <td></td>
        </tr>
    </table>
 
 - SimpleDateFormat을 쓰지 말아야하는 이유
 > Referemce 문서 내에 " SimpleDateFormat은 Multi-Thread 환경에서 Safe하지 않는다"라는 내용이 있다.<br/>
 > 즉, 의도치 않은 오류로 인한 결과값이 저장된다면 크게 문제가 발생할 수 있다. ➡️ *해결 방법은 아래 Tip2를 참조*

 **!Tip2.** [pranne1224님의 Java-SimpleDateFormat-위험성과 해결방법](https://velog.io/@pranne1224/Java-SimpleDateFormat-%EC%9C%84%ED%97%98%EC%84%B1)

 - SimpleDateFormat 문법
 > ```java
 > SimpleDateFormat df = new SimpleDateFormat("yyyy-MM-dd");
 > Date d = new Date();
 > System.out.println(df.format(d)); // SimpleDateFormat은 Date 클래스만 사용가능
 > // Calendar class를 사용하려면, Date class로 변환해주어야한다
 > ```

##### ChoiceFormat

 - ChoiceFormat이란?
 > 특정 범위에 속하는 값을 문자열로 변환

 - ChoiceFormat 문법
 > - 두 배열로 치환하기
 > ```java
 > double[] limits = {60, 70, 80, 90}; //오름차순으로
 > String[] grades = {"D", "C", "B", "A"};
 > int[] scores = {100, 95, 88, 70, 52, 60, 70};
 > ChoiceFormat form = new ChoiceFormat(limits, grades); // 범위배열, 결과값 배열
 > for(int i=0; i<scores.length; i++) {
 >     System.out.println(scores[i] + " : "+ form.format(scores[i])); // 결과값: A,A,B,C,D,D,C
 > ```
 > 
 > - 패턴으로 치환하기
 > ```java
 > String pattern = "60#D|70#C|80<B|90#A"; // #는 경계값을 범위에 포함, <포함시키지 않음
 > int[] scores = {91, 90, 80, 88, 70, 52, 60};
 > ChoiceFormat form = new ChoiceFormat(pattern);
 > for(int i=0; i < scores.length; i++) {
 >     System.out.println(scores[i] + " : " + form.format(scores[i])); // 결과값: A,A,C,B,C,D,D
 > ```

##### MessageFormat

 - MessageFormat이란?
 > 데이터를 정해진 양식에 맞게 메시지를 출력

 - MessageFormat 문법
 > - print
 > ```java
 > String pattern ="VALUES ({0}',''{1}'',{2},''{3}'')";
 > Object[] argument = {22.02221, "29세", "경기도", "학생"};
 > System.out.println(MessageFormat.format(pattern, argument)); //{숫자 부분에 데이터가 출력된다.}
 > ```
 > 
 > - parse
 > ```java
 > pattern = "{0},{1},{2},{3}"
 > MessageFormat mf = new MessageFormat(pattern);
 > Object[] objs = mf.parse(String 객체); //패턴을 따라 {}안에 있는 데이터값을 obj 객체 배열로 변환
 > ```

## java.time패키지

##### java.time패키지의 핵심 클래스
 
 - java.time 패키지의 핵심 클래스
 > 날짜와 시간이 별도로 분리되어 있어 따로 사용할 수 있고, 합쳐진 클래스로 사용할 수 있다.
 >  - LocalDate : 날짜
 >  - LocalTime : 시간
 >  - Instant : 날짜 시간 초단위로 나타냄(타임스탬프)
 >  - LocalDateTime : 로컬 날짜 및 시간(날짜 + 시간)
 >  - ZonedDateTime : 특정 타임존의 날짜 및 시간(날짜 + 시간 + 시간대)
 
##### LocalDate와 LocalTime


- LocalDate와 LocalTime 클래스 메소드 정의
<table>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;"><b>클래스</b></td>
        <td style="width: 33.3333%; height: 20px;"><b>메소드</b></td>
        <td style="width: 33.3333%; height: 20px;"><b>설명</b></td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;"><b>LocalDate</b></td>
        <td style="width: 33.3333%; height: 20px;">inr getYear()</td>
        <td style="width: 33.3333%; height: 20px;">년</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">Month getMonth()</td>
        <td style="width: 33.3333%; height: 20px;">Month 열거값</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">int getMonthValue()</td>
        <td style="width: 33.3333%; height: 20px;">월</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">int getDayOfYear</td>
        <td style="width: 33.3333%; height: 20px;">일년의 몇 번째 일</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">int getDayOfMonth()</td>
        <td style="width: 33.3333%; height: 20px;">월의 몇 번째 일</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">DayOfWeek getDayOfWeek()</td>
        <td style="width: 33.3333%; height: 20px;">요일</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">boolean isLeapYear()</td>
        <td style="width: 33.3333%; height: 20px;">윤년 여부</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;"><b>LocalTime</b></td>
        <td style="width: 33.3333%; height: 20px;">int getHour()</td>
        <td style="width: 33.3333%; height: 20px;">시간</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">int getMinute()</td>
        <td style="width: 33.3333%; height: 20px;">분</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">int getSecond()</td>
        <td style="width: 33.3333%; height: 20px;">초</td>
    </tr>
    <tr style="height: 20px;">
        <td style="width: 33.3333%; height: 20px;">&nbsp;</td>
        <td style="width: 33.3333%; height: 20px;">int getNano()</td>
        <td style="width: 33.3333%; height: 20px;">나노초 리턴</td>
    </tr>
</table>

##### Instant

##### LocalDateTime과 ZonedDateTime

##### TemporalAdjusters

##### Period와 Duration

##### 파싱과 포맷

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [홈페이지] [delftstack 변수 유형 확인하기](https://www.delftstack.com/ko/howto/java/how-to-check-type-of-a-variable-in-java/)
3. [블로그] [devkuma님의 Date 클래스](https://www.devkuma.com/docs/java/date-class/)
