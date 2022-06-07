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

##### Object클래스

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
