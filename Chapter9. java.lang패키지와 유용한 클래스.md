# Chapter9. java.lang패키지와 유용한 클래스

## 목차
  1. [java.lang패키지](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javalang%ED%8C%A8%ED%82%A4%EC%A7%80 "java.lang패키지")
	 - [1-1. Object클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#object%ED%81%B4%EB%9E%98%EC%8A%A4 "Object클래스")
	 - [1-2. String클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#string%ED%81%B4%EB%9E%98%EC%8A%A4 "String클래스")
	 - [1-3. StringBuffer클래스와 StringBuilder클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#stringbuffer%ED%81%B4%EB%9E%98%EC%8A%A4%EC%99%80-stringbuilder%ED%81%B4%EB%9E%98%EC%8A%A4 "StringBuffer클래스와 StringBuilder클래스")
	 - [1-4. Math클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#math%ED%81%B4%EB%9E%98%EC%8A%A4 "Math클래스")
	 - [1-5. 래퍼(wrapper) 클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#%EB%9E%98%ED%8D%BCwrapper-%ED%81%B4%EB%9E%98%EC%8A%A4 "래퍼(wrapper) 클래스")
  2. [유용한 클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#%EC%9C%A0%EC%9A%A9%ED%95%9C-%ED%81%B4%EB%9E%98%EC%8A%A4 "유용한 클래스")
	 - [2-1. java.util.Objects클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javautilobjects%ED%81%B4%EB%9E%98%EC%8A%A4 "java.util.Objects클래스")
	 - [2-2. java.util.Random클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javautilrandom%ED%81%B4%EB%9E%98%EC%8A%A4 "java.util.Random클래스")
	 - [2-3. 정규식(Regular Expression) - java.util.regex패키지](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#%EC%A0%95%EA%B7%9C%EC%8B%9Dregular-expression---javautilregex%ED%8C%A8%ED%82%A4%EC%A7%80 "정규식(Regular Expression) - java.util.regex패키지")
	 - [2-4. java.util.Scanner클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javautilscanner%ED%81%B4%EB%9E%98%EC%8A%A4 "java.util.Scanner클래스")
	 - [2-5. java.util.StringTokenizer클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javautilstringtokenizer%ED%81%B4%EB%9E%98%EC%8A%A4 "java.util.StringTokenizer클래스")
	 - [2-6. java.math.BigInteger클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javamathbiginteger%ED%81%B4%EB%9E%98%EC%8A%A4 "java.math.BigInteger클래스")
	 - [2-7. java.math.BigDecimal클래스](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#javamathbigdecimal%ED%81%B4%EB%9E%98%EC%8A%A4 "java.math.BigDecimal클래스")
  3. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter9.%20java.lang%ED%8C%A8%ED%82%A4%EC%A7%80%EC%99%80%20%EC%9C%A0%EC%9A%A9%ED%95%9C%20%ED%81%B4%EB%9E%98%EC%8A%A4.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")
## java.lang패키지
  
  - java.lang 패키지란?
  > 자바프로그래밍에 가장 기본이 되는 클래스들을 포함하며 import문 없이도 사용 가능한 패키지

##### Object클래스

 - Object 클래스란?
 > 모든클래스(API or Class등)는 Object클래스의 자식클래스이다. <br/>
 > 즉, Object클래스가 자바에서 '최상의 클래스'이다.
 > Object클래스에는 다양한 메소드가 존재하는데, 어떤 클래스에서도 이 메소드를 호출할수 있다.

 - Object클래스 대표 메소드 종류
 > 	- equals() 메소드 : 문자열을 비교하는 비교문, 두 객체가 동일한 객체라면 true를 리턴하고 아니라면 false를 리턴한다.<br/>
 > 	▶ 예시
 > 	```java
 >	public class EqString {
 >	  public static void main(String[] args) {
 >	   String a = "hello";
 >	   String b = "hello";
 >	   
 >	   if(a.equals(b)) {
 >	   	System.out.println("동일O");
 >	   } else {
 >	   	System.out.println("동일X");	   
 >	   }
 >	  }
 >	}
 > 	```
 > 	✍️ 출력결과
 > 	```text
 > 	동일O
 > 	```
 > 	
 > 	- hashCode() 메소드 : 객체의 메모리 번지를 이용해서 해시코드를 만들어 리턴하며 객체마다 다른값을 가지고 있따.<br/>
 > 	▶ 예시 : 예시로 들만한게 없다.
 > 
 > 	- toString() 메소드 : 객체의 문자 정보를 리턴하며 객체를 문자열로 표현해준다.<br/>
 > 	▶ 예시
 > 	```java
 >	class Car{
 >		private String model;
 >		private String year;
 >
 >		public Car(String model, String year) {
 >			this.model = model;
 >			this.year = year;
 >		}
 >
 >		public String toString() {
 >			return model + " , " + year;
 >		}
 >	}
 >
 >	public class Test {
 >
 >		public static void main(String[] args) {
 >			Car car1 = new Car("first", "2001");
 >			Car car2 = new Car("second", "2018");
 >			System.out.println(car1.toString());
 >			System.out.println(car2.toString());
 >		}
 >	}
 > 	``` 
 > 	
 > 	✍️ 출력결과
 > 	```text
 > 	first, 2001
 > 	second, 2018
 > 	```

 - Object 클래스의 메서드
  <table>
   <tr>
     <th>Object 클래스의 메서드</th>
     <th>설명</th>
   </tr>
   <tr>
     <td>public boolean equals(Object obj)</td>
     <td>객체 자신과 객체 obj가 같은 객체 인지 여부를 반환 (같으면 true)</td>
   </tr>
   <tr>
     <td>public int hashCode()</td>
     <td>객체 자신의 해시코드를 반환</td>
   </tr>
   <tr>
     <td>public String toString()</td>
     <td>객체 자신의 정보를 문자열로 반환</td>
   </tr>
   <tr>
     <td>protected Object clone()</td>
     <td>객체 자신의 복사본을 반환</td>
   </tr>
   <tr>
     <td>public Class getClass()</td>
     <td>객체 자신의 클래스 정보를 담고 있는 Class인스턴스를 반환</td>
   </tr>
   <tr>
     <td>public void notify()</td>
     <td>객체 자신을 사용하려고 기다리는 쓰레드를 하나만 깨움</td>
   </tr>
   <tr>
     <td>public void notifyAll()</td>
     <td>객체 자신을 사용하려고 기다리는 모든 쓰레드를 깨움</td>
   </tr>
   <tr>
     <td>publid void wait() <br/> public void wait(long timeout) <br/> public void wait(long timeout, int nanos)</td>
     <td>다른 쓰레드가 notify()나 notifyAll()을 호출할 때까지 현재 쓰레드를 무한히 또는 지정된 시간(timeout, nanos)동안 기다리게 한다.<br/>
(timeout은 천 분의 1초, nanos는 10^9분의 1초)</td>
   </tr>
   <tr>
     <td>protected void finalize()</td>
     <td>객체가 소멸될 때 가비지 컬렉터에 의해 자동적으로 호출<br/>
이 때 수행되어야하는 코드가 있을 때 오버라이딩 (거의 사용안함)</td>
   </tr>
  </table>	
  
**!Tip0.** [java.lang패키지와 유용한(util) 클래스](https://rebeccacho.gitbooks.io/java-study-group/content/chapter9.html)

##### String클래스

 - String 클래스
 > Char()타입의 불편함을 해소 시켜주는 매우 편리한 존재<br/>
 > 스트링 클래스 내부를 까보면 결국 Char배열로 생성된 불변 객체 값

 - String 클래스 선언
 > 	- 원시 타입처럼 보여서 원시타입으로 착각은 근물!<br/>
 > 	즉, 원시 타입이 아닌 참조형 객체 클래스이며 불변 객체로 동일한 객체가 공유되면서 사용

 ![제목 없음](https://user-images.githubusercontent.com/66407386/172546584-ae84fb4e-d6d9-4ef4-b188-5c61d2400501.png)
 <br/> **!Tip1.** [스트링의 내부구현](https://pjh3749.tistory.com/255) <br/>

 **!Tip2.** [자바 데이터 타입, 변수 그리고 배열 - 프리미티브 타입](https://minikuma-laboratory.tistory.com/26)

 - 스트링 클래스는 2가지 선언 방법
 > 	- 리터럴
 > 	▶ 예시
 > 	```java
 > 	String str1 = "String1";
 > 	```
 > 		
 > 	- new를 사용한 선언
 > 	▶ 예시
 > 	```java
 > 	String str2 = new String("String2");
 > 	```
 > 	
 > 	☑️ 둘다 똑같은 값이 나오긴 하지만 차이가 있음!!
 > 	- 리터럴 선언은 String 클래스는 선언언시 객체가 *String constant pool*에 저장
 > 	- new는 *Heap영역*에 저장되어 사용됨 <br/>
 
 ![image](https://user-images.githubusercontent.com/66407386/172543739-4b434666-1d6d-4f79-9a4b-80a02347eed3.png)
 
 ❓ 그렇다면 다른 이유는 뭘까?
 > "="은 왜 다른 걸까? 리터럴과 new의 선언 후 저장되는 **객체의 위치**가 다르기 때문 [이유는 위 내용 참조] <br/>
 > "=="은 왜 같다고 하는 걸까? 불면 객체이기 때문에 미리 ***intern()메서드***에서 탐색되어 객체가 공유되어 비교하기 때문

 **!Tip3.** [String.intern() 이란? 언제 사용하는가?](https://simple-ing.tistory.com/3)

##### StringBuffer클래스와 StringBuilder클래스

 - Buffer & Builder의 어원
 > 	- Buffer의 어원
 > 	  데이터를 한 곳에서 다른 한곳으로 전송하는 동안 일시적으로 그 데이터를 보관하는 메모리 영역<br/>
 > 	  ✋ 보통 속도가 바뀔 수 있기 때문에 데이터 수신, 처리속도에 차이가 있다.
 > 	- Builder의 어원 - *정리의 필요성이 있다.*
 > 	  건축 업자 혹은 건축 회사라 표현한다. 즉, 복합 객체의 생성 과정과 표현 방법을 분리하여<br/>
 > 	  절차에 따라 다른 표현 결과를 만드는 것이라 생각한다.<br/>
 > 	  때문에 String과 문자열을 더할 때 새로운 객체를 생성하는 것이 아니라 기존의 데이터를 더하는 방식이다.<br/>
 > 	  ✋ 속도는 빠르며 상대적으로 부하가 적다. 특히 긴 문자열을 더하는 상황이라면 StringBuilder를 사용하는 것이 좋다.

 - String과 StringBuffer & StringBuilder
 > 	- String
 > 	String은 너무 직관적이며 객체 생성 후 문자열을 더하면 객체가 변경된 것으로 착각 할 수 있다.<br/>
 > 	새로운 메모리 영역을 가르키며 변경되고 기존에 있는 값으로 할당된 메모리 영역은 GC에 의해 살아진다.<br/>
 > 	따라서 String은 불변성이기 때문에 **변하지 않는 문자열을 읽어들이는 경우에만 사용하는 것이 좋다.**
 > 	
 > 	- StringBuffer & StringBuilder
 >      문자열이 추가, 수정, 삭제 등등 연산이 많이 일어나는 경우 알고리즘에서<br/>
 >      String를 쓰는 것은 Heap 또는 GC를 계속 사용하면 Heap 메모리 부족으로 성능에 크게 영향을 미칠 수도 있다.<br/>
 >      따라서 동일 객체 내에서 변경 편한 **가변성을 지닌 StringBuffer 혹은 StringBuilder를 사용하는 것이 좋다.**

 - String & StringBuffer & StringBuilder의 차이점
 > 
 <table>
  <tr>
    <th></th>
    <th>String</th>
    <th>StringBuffer</th>
    <th>StringBuilder</th>
  </tr>
  <tr>
    <td>저장소</td>
    <td>String ppol</td>
    <td>Heap Memory</td>
    <td>Heap Memory</td>
  </tr>
  <tr>
    <td>수정 여부</td>
    <td>불가능(불변성)</td>
    <td>가능(가변성)</td>
    <td>가능(가변성)</td>
  </tr>
  <tr>
    <td>스레드 지원</td>
    <td>가능</td>
    <td>가능</td>
    <td>불가능</td>
  </tr>
  <tr>
    <td>동기화 여부</td>
    <td>가능</td>
    <td>가능</td>
    <td>불가능</td>
  </tr>
  <tr>
    <td>성능</td>
    <td>빠름</td>
    <td>느림</td>
    <td>빠름</td>
  </tr>
 </table>

 - StringBuffer & StringBuilder가 적정한 경우
 > StringBuffer : 멀티 쓰레드 환경의 경우<br/>
 > StringBuilder: 싱글 쓰레드 환경 혹은 멀티 쓰레드에서 동기화가 필요없는 경우

##### Math클래스
 - Math 클래스
 > 수학에 자주 사용하는 상수들과 함수들을 미리 구현해 놓은 클래스<br/>
 > 객체를 생성하지 않고도 바로 사용 가능하다.

- 대표적인 Math 메소드
 <table>
  <tr>
    <th>메소드</th>
    <th>설명</th>
  </tr>
  <tr>
    <td>static double random()</td>
    <td>0.0 이상 1.0 미만의 범위에서 임의의 double형 값을 하나 생성하여 반환함.</td>
  </tr>
  <tr>
    <td>
	static double abs(double a)<br/>
	static double abs(float a)<br/>
	static double abs(int a)<br/>
	static double abs(long a)
    </td>
    <td>전달된 값이 음수이면 그 값의 절댓값을 반환하며, 전달된 값이 양수이면 인수를 그대로 반환함.</td>
  </tr>
  <tr>
    <td>static double ceil(double a)</td>
    <td>전달된 double형 값의 소수 부분이 존재하면 소수 부분을 무조건 올리고 반환함.</td>
  </tr>
  <tr>
    <td>static double floor(double a)</td>
    <td>전달된 double형 값의 소수 부분이 존재하면 소수 부분을 무조건 버리고 반환함.</td>
  </tr>
  <tr>
    <td>
	static long round(double a)<br/>
	static int round(float a)
    </td>
    <td>전달된 값을 소수점 첫째 자리에서 반올림한 정수를 반환함.</td>
  </tr>
  <tr>
    <td>static double rint(double a)</td>
    <td>전달된 double형 값과 가장 가까운 정수값을 double형으로 반환함.</td>
  </tr>
  <tr>
    <td>
	static double max(double a, double b)<br/>
	static float max(float a, float b)<br/>
	static long max(long a, long b)<br/>
	static int max(int a, int b)
    </td>
    <td>전달된 두 값을 비교하여 큰 값을 반환함.</td>
  </tr>
  <tr>
    <td>
	static double min(double a, double b)<br/>
	static float min(float a, float b)<br/>
	static long min(long a, long b)<br/>
	static int min(int a, int b)
    </td>
    <td>전달된 두 값을 비교하여 작은 값을 반환함.</td>
  </tr>
  <tr>
    <td>static double pow(double a, double b)</td>
    <td>전달된 두 개의 double형 값을 가지고 제곱 연산을 수행하여, ab을 반환함.</td>
  </tr>
  <tr>
    <td>static double sqrt(double a)</td>
    <td>전달된 double형 값의 제곱근 값을 반환함.</td>
  </tr>
  <tr>
    <td>
	static double sin(double a)<br/>
	static double cos(double a)<br/>
	static double tan(double a)
    </td>
    <td>전달된 double형 값에 해당하는 각각의 삼각 함숫값을 반환함.</td>
  </tr>
  <tr>
    <td>static double toDegrees(double angrad)</td>
    <td>호도법의 라디안 값을 대략적인 육십분법의 각도 값으로 변환함.</td>
  </tr>
  <tr>
    <td>static double toRaidans(double angdeg)</td>
    <td>육십분법의 각도 값을 대략적인 호도법의 라디안 값으로 변환함.</td>
  </tr>
 </table>

**!Tip4.** [Math클래스 예제](https://yang-droid.tistory.com/33)

##### 래퍼(wrapper) 클래스

 - 래퍼란?
 > 래핑의 어원으로 **"감싼다"** 혹은 **"포장한다"** 라는 의미를 내포하고 있다.<br/>
 > 기본 타입의 데이터를 객체로 표현해야하는 경우가 있는데 이때 기본 자료타입을<br/>
 > 객체로 다루기 위해서 사용하는 것이 래퍼 클래스이다.<br/>
 > 단, 래퍼 클래스로 감싸고 있는 기본 타입 값은 외부에서 변경할 수 없다.<br/>
 > 변경을 하고 싶다면 새로운 객체를 생성해야한다.

 - 래퍼의 종류 
 <table>
  <tr>
    <th>원어(Primitive)</th>
    <th>Boxing<br/>&<br/>Unboxing</th>
    <th>래퍼 클래스(Wrapper Class)</th>
  </tr>
  <tr>
    <td>byte</td>
    <td></td>
    <td>Byte</td>
  </tr>
  <tr>
    <td>short</td>
    <td></td>
    <td>Shrot</td>
  </tr>
  <tr>
    <td>int</td>
    <td>Boxing(박싱)<br/>→</td>
    <td>Interger</td>
  </tr>
  <tr>
    <td>long</td>
    <td></td>
    <td>Long</td>
  </tr>
  <tr>
    <td>float</td>
    <td>UnBoxing(언박싱)<br/>←</td>
    <td>Float</td>
  </tr>
  <tr>
    <td>double</td>
    <td></td>
    <td>Double</td>
  </tr>
  <tr>
    <td>char</td>
    <td></td>
    <td>Character</td>
  </tr>
  <tr>
    <td>bollean</td>
    <td></td>
    <td>Boolean</td>
  </tr>
 </table>

 - 래퍼 클래스 구조<br/>
 ![image](https://user-images.githubusercontent.com/66407386/172748457-07033e9f-cace-4bb0-9331-b2a42f9bcb9f.png)
 > 최초 부모는 Object로 내부적으로 숫자를 다루는 래퍼 클래스는 Number로 지칭한다.

 - 박싱과 언박싱<br/>

 ![image](https://user-images.githubusercontent.com/66407386/172787084-df02cf8b-d61c-4453-b868-5901959e07db.png)

 > 박싱 : 기본 타입의 값을 포장 객체로 만드는 과정<br/>
 > 언박싱 : 포장 객체에서 기본타입의 값을 받아오는 과정<br/>
 > ▶ 예제
 > ```java
 > public class Wrapper_Ex {
 >    public static void main(String[] args)  {
 >       Integer num = new Integer(17); // 박싱
 >       int n = num.intValue(); //언박싱
 >       System.out.println(n);
 >    }
 > }
 > ```

 - 자동박싱(AutoBoxing)과 자동언박싱(AutoUnBoxing)
 > 자동 박싱과 자동 언박싱읜 Java 1.5버전부터 지원하고 있다.
 > - 자동박싱 : 원시 타입의 값을 해당하는 래퍼 클래스의 객체로 바꾸는 과정 
 > 	- 원시 타입이 래퍼 클래스 타입의 파라미터를 받는 메서드를 통과할때
 > 	- 원시 타입이 래퍼 클래스의 변수호 할당 될때<br/>
 >      ▶ 예제
 > 	```java
 >	public class Test {
 >	  // 변수 초기화
 >	  private int inte;
 >	  
 >	  public Integer getInte() {
 >	  	return inte;
 >	  }
 >	}
 >	// 숨은 과정 보여주기
 >	public class Test {
 >	  // 변수 초기화
 >	  private int inte;
 >	  
 >	  public Integer getInte() {
 >	  	return Integer.valueOf(inte);
 >	  }
 >	}
 > 	```
 > - ~~자동언박싱 : 래퍼 클래스 타입을 원시 타입으로 변환하는 과정~~
 > 		- ~~래퍼 클래스 타입이 원시 타입의 파라미터를 받는 메서드를 통과할 때~~
 > 		- ~~래퍼 클래스 타입이 원시 타입의 변수로 할당 될때~~

**!Tip5.** [오토박싱 및 언박싱 그리고 JVM내 캐시에 대하여](https://www.charlezz.com/?p=46017)

## 유용한 클래스

##### java.util.Objects클래스 

 - Objects 클래스
 > 객체 비교, null 여부등을 조사할 때 사용
 
 - Objects 클래스의 정적 메소드
 <table>
  <tr>
    <th>리턴 타입</th>
    <th>메소드(매개변수)</th>
    <th>설명</th>
  </tr>
  <tr>
    <td>int</td>
    <td>compare(T a, T b, Comparator<T> c)</td>
    <td>두 객체 a, b를 Comparator를 사용해서 비교</td>
  </tr>
  <tr>
    <td>boolean</td>
    <td>deepEquals(Object a, Object b)</td>
    <td>두 객체의 깊은 비교(배열의 항목까지 비교)</td>
  </tr>
  <tr>
    <td>boolean</td>
    <td>equals(Object a, Object b)</td>
    <td>두 객체의 얕은 비교(번지 값만 비교)</td>
  </tr>
  <tr>
    <td>int</td>
    <td>hash(Object ... values)</td>
    <td>매개 값이 저장된 배열의 해시코드 생성</td>
  </tr>
  <tr>
    <td>int</td>
    <td>hashCode(Object o)</td>
    <td>객체의 해시코드 생성</td>
  </tr>
  <tr>
    <td>boolean</td>
    <td>isNull(Object obj)</td>
    <td>객체가 null인지 조사</td>
  </tr>
  <tr>
    <td>boolean</td>
    <td>nonNull(Object obj)</td>
    <td>객체가 null이 아닌지 조사</td>
  </tr>
  <tr>
    <td>T</td>
    <td>requireNonNull(T obj)</td>
    <td>객체가 null인경우 예외 발생</td>
  </tr>
  <tr>
    <tdT>T</td>
    <td>requireNonNull(T obj, String message)</td>
    <td>객체가 null 인경우 에외 발생<br/>(주어진 예외 메시지 포함)</td>
  </tr>
  <tr>
    <td>T</td>
    <td>requireNonNull(T obj, Supplier<String> messageSupplier)</td>
    <td>객체가 null인 경우 예외 발생<br/>(람다식이 만든 예외 메시지 포함)</td>
  </tr>
  <tr>
    <td>String</td>
    <td>toString(Object o)</td>
    <td>객체의 toString()리턴 값 리턴</td>
  </tr>
  <tr>
    <td>String</td>
    <td>toString(Object o, String nullDefault)</td>
    <td>객체의 toString() 리턴 값 리턴,<br/>첫 번째 매개 값이 null인 경우 두번째 매개 값 리턴</td>
  </tr>
</table>

<br/>❓. T로 받는 다는 의미는 무엇일까? - 타입

- equlas() & deepEquals()
> - equlas()
> 문자열을 비교할 때 가장 많이 쓰는 Objects 클래스 중 하나로 <br/>
> 반환 형태는 true & false로 반환하며 java.util.Object의 내용 속 equals는 아래와 같다.
> ```java
> public static boolean equals(Object a, Object b) {
>   return (a == b) || (a != null && a.equals(b));
> }
>   /*
>    * 반환을 할 때 두가지를 체크 한다.
>    * 1. (a == b) : a와 b의 타입이 같니?
>    * 또한(둘중 하나가 맞다면)
>    * 2. (a != null && a.equals(b)) : a가 null 아니라면 a와 b를 비교해봐
>    */
> ```
> 
> - deepEquals()
> equls에서는 단순 문자열을 비교 했다면 deepEquals에서는 객체까지도 비교하며<br/>
> 반환 형태는 equals와 동일하게 true & false로 반환하며 java.utile.Obacject의 내용 속 deepEquals는 아래와 같다.
> ```java
> public static boolean deepEquals(Object a, Object b) {
>   if (a == b)
>      return true;
>   else if (a == null || b == null)
>      return false;
>   else
>     return Arrays.deepEquals0(a, b);
> }
> 
>  /*
>   * 1. if 조건에서 a와 b가 동등하다면 true를 반환
>   * 2. if 조건이 아니라면 else if 조건으로 a 그리고 b 둘중 하나라도 null이라면 false를 반환
>   * 3. 위 두 조건다 아니라면 Arrays 클래스의 deepEquals() 메소드를 이용하여 반환하라
>   */
> ```

- hash() & hashCode()
> - hash()
> 주어진 매개값들로 이용하여 해시코드를 생성하는 역할이며<br/>
> 반환 형태는 int로 반환하며 java.util.Objects의 내용 속 hash는 아래와 같다.
> ```java
> public static int hash(Object... values) {
>    return Arrays.hashCode(values);
> }
> ```
> 
> - hashCode()
> 주어진 매개값들로 배열을 생성하고, Arrays.hashCode(Obhects[])를 호출해서 해시코드를 얻고, 값을 리턴한다.<br/>
> 반환 형태는 hash와 동일하게 int로 반환하며 java.util.Objects의 내용 속 hashCode는 아래와 같다.
> ```java
> public static int hashCode(Object o) {
>    return o != null ? o.hashCode() : 0;
> }
> ```

- isNull() & nonNull(), requireNonNull()
> - isNull()
> isNull()메소드는 매개 값이 null일 경우 체크한다.<br/>
> 반환 형태는 타입(Type)통해서 반환하며 boolean 형태로 반환하며 java.util.Objects의 내용 속 isNull은 아래와 같다.
> ```java
> public static boolean isNull(Object obj) {
>     return obj == null;
> }
> ```
> 
> - nonNull()
> nonNull()메소드는 isNull과 반대로 매개값이 null 아닌 경우를 체크한다.<br/>
> 반환형태는 isNull과 동일하게 boolean형태로 반환하며 java.util.Objects의 내용 속 nonNull은 아래와 같다.
> ```java
> public static boolean nonNull(Object obj) {
>     return obj != null;
> }
> ```
>  
> - requireNonNull()
> 개발자라면 못 본 사람이 없는 아주 친숙한 단어이자 제일 만나기 싫은 문제의 단어 NullPointerException의 원리가 여기 있다.<br/>
> 반환형태는 파라미터로 입력된 값이 null이라면 NullPointerException이 발생하고, 그렇지 않다면 입력값을 그대로 반환하며 java.util.Objects의 내용 속 requireNonNull은 아래와 같다.
> ```java
> public static <T> T requireNonNull(T obj, Supplier<String> messageSupplier) {
>     if (obj == null)
>         throw new NullPointerException(messageSupplier.get());
>     return obj;
> }
> ```

- toString()
> 객체의 문자 정보를 리턴한다.<br/>
> 반환 방식은 해당 객체의 문자를 반환하거나 혹은 데이터가 없을 경우 nullDefault를 리턴한다.
> ```java
> public static String toString(Object o) {
>     return String.valueOf(o);
> }
> ```


##### java.util.Random클래스

 - Random 클래스
 > 임의의 난수를 발생시킬 수 있는 객체이며 다양한 데이터 타입형 발생 시키거나 일정한 범위에 존재하는 난수를 발생되게 할 수도 있다.
 > - Random() : 디폴트 생성자. 현재 시간을 초기 값으로 하는 난수 발생기 객체를 생성
 > - Random(longseed) : long형의 seed값을 매개변수로 받아 난수 발생기 객체를 생성

 - Random 메소드
 <table>
  <tr>
    <th>메소드</th>
    <th>설명</th>
  </tr>
  <tr>
    <td>void nextBytes(byte[] bytes)</td>
    <td>buffer를 난수로 채운다.</td>
  </tr>
  <tr>
    <td>boolean nextBoolean()</td>
    <td>boolean 형태의 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>double nextDouble()</td>
    <td>double 형태의 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>float nextFloat()</td>
    <td>float 형태의 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>int nextInt()</td>
    <td>int 형태의 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>long nextLong()</td>
    <td>long 형태의 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>int nextInt(int bound)</td>
    <td>한계 값(bound)을 받아서 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>double nextGaussian()</td>
    <td>가우스의 형의 난수를 double 형태의 난수를 반환한다.</td>
  </tr>
  <tr>
    <td>void setSeed(long seed)</td>
    <td>난수 발생기의 seed 값을 새로 설정한다.</td>
  </tr>
</table>
	
##### 정규식(Regular Expression) - java.util.regex패키지

 - 정규식이란?
 >  - 정규 / 표현 / 패턴 어원
 > 	- 정규 : 정식으로 된 규정이나 규범
 > 	- 표현 : 생각이나 느낌 다위를 언어나 몸짓 따위의 형상
 > 	- 패턴 : 일정한 형태나 양식 또는 유형
 > 특정한 규칙을 가진 문자열의 집합을 표현하는 데 사용하는 형식 언어
 > 정규 표현식은 많은 텍스트 편집기와 프로그래밍 언어에서 문자열의 검색과 치환을 위해 지원

 - 정규표현식의 장점과 단점
 > - 장점
 >   1. 입력 문자열의 처리<br/>
 >     ▶ 사용자가 데이터를 입력할 때 어떤 구성의 문자열이 입력될지 예상 어렵다.<br/>
 >     &nbsp; &nbsp; &nbsp;   이런 경우 정규식을 통한 제한 범위를 주면서 sql인젝션 공격에 방어할 수 있다.
 >   2. 범용성<br/>
 >     ▶ 다양한 언어와 프로그램에서 지원하는 범용성이 매우 뛰어난 문법이다.<br/>
 >     &nbsp; &nbsp; &nbsp;   따라서 특정한 처리를 유사한 표현식으로 손쉽게 처리 가능하다.
 >   3. 생산성의 증대<br/>
 >     ▶ 문서의 이동이 편하다.<br/>
 >     &nbsp; &nbsp; &nbsp;   즉, 특정한 문자열을 그대로 코드에 적용해야하는 경우 반대로 문서로 <br/>
 >     &nbsp; &nbsp; &nbsp;   정규 표현식을 통해서 원하는 특정 문자를 변환하고 추출하기 편하다.
 >
 > - 단점
 >  1. 배우고 익히며 정확하게 사용하기 어렵다.<br/>
 >     ▶ 문법은 어렵지 않지만 문법에 오류를 찾기 쉽지 않으며 작성자와 유지보수자가 <br/>
 >     &nbsp; &nbsp; &nbsp;   유지보수성이 매우 떨어지며 실제로 정규 표현식을 잘 다루는 사람이 많이 없다.
 >  2. 난해한 코드성<br/>
 >     ▶ 정규 표현식을 모른다면 암호화된 코드로 밖에 안보인다.<br/>
 >     &nbsp; &nbsp; &nbsp;   지나치게 난해한 표현식의 사용은 가독성을 낮추고 유지보수와 협업이 매우 어렵다.
 >  3. 유용하지만 오차범위가 있다.<br/>
 >     ▶ 실제로 정규 표현식을 사용하다 보면 완벽이란 정규 표현식을 보기 어렵다.<br/>
 >     &nbsp; &nbsp; &nbsp;   작성자가 미쳐 생각하지 못한 예외 케이스가 있을 수 있으며 이는 해커에게 <br/>
 >     &nbsp; &nbsp; &nbsp;   공격 당할 수 있는 치명적인 문제로 자리 매김될 수 있기 때문에 충분한 테스트가 필요하다.
 >

 - 정규식은 어떻게 사용하는지?
	
 **!Tip6.** [정규식 테스트 사이트 중 가장 많이 사용되는 사이트](https://regexr.com/)<br/>
 **!Tip7.** [Java 정규식 공식 문서](https://docs.oracle.com/javase/7/docs/api/java/util/regex/Pattern.html)<br/>
 
 **!Tip8.** [SQL 인젝션 개념과 원리](https://m.blog.naver.com/lstarrlodyl/221837243294)<br/>
 **!Tip9.** [정규식을 통한 SQL인젝션 취약점 방어](https://m.mkexdev.net/427)
	
##### java.util.Scanner클래스

 - Scanner클래스
 > 입력되는 키 값을 공백으로 구분되는 토큰 단위로 읽으며 읽은 바이트를 문자, 정수, 실수, 불린, 문자열 등 타입으로 변환하여 리턴하는 

 - Scanner 선언
 > ```java
 > import java.util.Scanner; // 스캐너를 사용하기 위해서 사용하는 필요 import
 > 
 > Scanner sc = new Scanner(System.in); // Scanner 객체
 > ```

 - Scanner의 주요 메소드
 <table>
  <tr>
    <th>메소드</th>
    <th>설명</th>
  </tr>
  <tr>
    <td> String next() </td>
    <td> 다음 토큰을 문자열로 리턴 </td>
  </tr>
  <tr>
    <td> byte nextByte() </td>
    <td> 다음 토큰을 byte 타입으로 리턴 </td>
  </tr>
  <tr>
    <td> short nextShort() </td>
    <td> 다음 토큰을 short 타입으로 리턴 </td>
  </tr>
  <tr>
    <td> int nextInt() </td>
    <td> 다음 토큰을 int 타입으로 리턴 </td>
  </tr>
  <tr>
    <td> long nextLong() </td>
    <td> 다음 토큰을 long 타입으로 리턴 </td>
  </tr>
  <tr>
    <td> float nextFloat() </td>
    <td>다음 토큰을 float 타입으로 리턴 </td>
  </tr>
  <tr>
    <td> double nextDouble() </td>
    <td> 다음 토큰을 double 타입으로 리턴 </td>
  </tr>
  <tr>
    <td> String nextLine() </td>
    <td> ' \n '을 포함하는 한 라인을 읽고 ' \n '을 버린 나머지만 리턴 </td>
  </tr>
  <tr>
    <td> void close() </td>
    <td> Scanner의 사용 종료 </td>
  </tr>
  <tr>
    <td> boolean hasNext() </td>
    <td>
	 재 입력된 토큰이 있으면 true, 아니면 새로운 입력이 들어올 때까지 무한정 기다려서,<br/>
	 새로운 입력이 들어오면 그 때 true 리턴.<br/>
	 ctrl + z 키가 입력되면 입력 끝이므로 false 리턴 </td>
  </tr>
</table>

##### java.util.StringTokenizer클래스

 - StringTokenizer클래스
 > 특정 문자로 구분된 문자열을 뽑아낼 때
 > 

##### java.math.BigInteger클래스

 - BigInteger클래스
 > 큰 정수형 타입인 long은 10진수 19자리 정도이다. 만약 이보다 더 큰값을 사용할때는 BigInteger를 사용
 > long 보다는 큰값을 다룰 수 있지만 성능은 long타입보다 떨어진다.

##### java.math.BigDecimal클래스

 - BigDecimal클래스
 > double타입의 값은 범위가 넓지만 정밀도가 최대 13자리 빡에 되지 않기 떄문에 특성상 오차를 피할 수 없다.
 > 때문에 오차가 없는 2진 정수로 변환하여 다루면서 실수를 정수와 10의 제곱의 곱으로 표현한다.


## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [블로그] [donglee99님의 JavaStringClass정리](https://velog.io/@donglee99/JAVA-String-%ED%81%B4%EB%9E%98%EC%8A%A4-%EC%A0%95%EB%A6%AC)
3. [블로그] [_JSPark님의 래퍼 클래스](https://jusungpark.tistory.com/17)
4. [블로그] [coco3o님의 [java]Wrapper클래스란?](AutoUnBoxing)
5. [블로그] [code0xff님의 Autoboxing과 AutoUnboxing](https://code0xff.tistory.com/150)
6. [이클립스] 이클립스에서 java.util 中 (ObjectsClass) 참조

https://rebeccacho.gitbooks.io/java-study-group/content/chapter9.html
https://kyleyj.tistory.com/28
