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
 > 

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

 - 박싱과 언박싱
 > 


## 유용한 클래스

##### java.util.Objects클래스 

##### java.util.Random클래스

##### 정규식(Regular Expression) - java.util.regex패키지

##### java.util.Scanner클래스

##### java.util.StringTokenizer클래스

##### java.math.BigInteger클래스

##### java.math.BigDecimal클래스

## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
2. [블로그] [donglee99님의 JavaStringClass정리](https://velog.io/@donglee99/JAVA-String-%ED%81%B4%EB%9E%98%EC%8A%A4-%EC%A0%95%EB%A6%AC)
3. [블로그] [_JSPark님의 래퍼 클래스](https://jusungpark.tistory.com/17)
4. 

https://rebeccacho.gitbooks.io/java-study-group/content/chapter9.html
