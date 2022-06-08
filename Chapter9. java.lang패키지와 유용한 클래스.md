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
 > 	- hashCode() 메소드 : 객체의 메모리 번지를 이용해서 해시코드를 만들어 리턴하며 객체마다 다른값을 가지고 있따.<br/>
 > 	▶ 예시 : 예시로 들만한게 없다.
 > 	<br/>
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

##### String클래스

##### StringBuffer클래스와 StringBuilder클래스

##### Math클래스

##### 래퍼(wrapper) 클래스

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

https://rebeccacho.gitbooks.io/java-study-group/content/chapter9.html
