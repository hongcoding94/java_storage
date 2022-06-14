## Chapter11. 컬렉션 프레임웍

1. [컬렉션 프레임웍(Collection Framework)](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%BB%AC%EB%A0%89%EC%85%98-%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8Dcollection-framework "컬렉션 프레임웍(Collection Framework)")
	- [1-1. 컬렉션 프레임웍의 핵심 인터페이스](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%BB%AC%EB%A0%89%EC%85%98-%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D%EC%9D%98-%ED%95%B5%EC%8B%AC-%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4 "컬렉션 프레임웍의 핵심 인터페이스")
	- [1-2. ArrayList](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#arraylist "ArrayList")
	- [1-3. LinkedList](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#linkedlist "LinkedList")
	- [1-4. Stack과 Queue](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#stack%EA%B3%BC-queue "Stack과 Queue")
	- [1-5. Iterator, ListIterator, Enumeration](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#iterator-listiterator-enumeration "Iterator, ListIterator, Enumeration")
	- [1-6. Arrays](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#arrays "Arrays")
	- [1-7. Comparator와 Comparable](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#comparator%EC%99%80-comparable "Comparator와 Comparable")
	- [1-8. HashSet](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#hashset "HashSet")
	- [1-9. TreeSet](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#treeset "TreeSet")
	- [1-10. HashMap과 Hashtable](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#hashmap%EA%B3%BC-hashtable "HashMap과 Hashtable")
	- [1-11. TreeMap](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#treemap "TreeMap")
	- [1-12. Properties](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#properties "Properties")
	- [1-13. Collections](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#collections "Collections")
	- [1-14. 컬렉션 클래스 정리 & 요약](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%BB%AC%EB%A0%89%EC%85%98-%ED%81%B4%EB%9E%98%EC%8A%A4-%EC%A0%95%EB%A6%AC--%EC%9A%94%EC%95%BD "컬렉션 클래스 정리 & 요약")
2. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 "참고 문서 / 블로그")


## 컬렉션 프레임웍(Collection Framework)

- 컬렉션이란?
> 사전적 의미 : 요소를 수집해서 저장하는 것
> 다수의 데이터를 쉽고 효과적으로 처리할 수 있고 표준화된 방법을 제공하는 클래스의 집합
> 즉, 데이터를 저장하는 자료구조와 데이터를 처리하는 알고리즘을 구조화하여 클래스로 구현해 놓은 것.
>
> - 자료구조 유형의 종류
>   - List : 순서가 있는 목록
>   - Set : 순서가 중요하지 않은 목록
>   - Queue : 먼저 들어온 순으로 나가는 목록
>   - Map : Key | Value의 형태로 저장
>
> - 인터페이스로 가능한 컬렉션 클래스를 나타내는 자료
>   ![image](https://user-images.githubusercontent.com/66407386/173496159-c6f3935f-6ef5-4109-9e04-7898888c9364.png)

- 컬렉션 프레임워크
> 사전적 의미 : 표준화, 정형화된 프로그래밍 방식
> 컬렉션을 다루기 위한 표준화된 프로그래밍 방식이며 컬렉션을 쉽고 편리하게 다룰 수 있는 다양한 클래스를 제공
> 데이터 군집의 형태를 크게 3가지로 나눠서 각각의 데이터 군집 형태를 인터페이스로 정의
>
>   - 컬렉션프레임워크 핵심 인터페이스
>   1. List
>   2. Set
>   3. Map
>
>   ※ 이중에서 List와 set은 공통부분들이 있어서 Collection 인터페이스로 정의하였다.

- 컬렉션 클래스 
> 여러 객체를 저잘할 수 있으며 저장 공간이 부족할 시 스스로 공간을 증가 시킨다.

##### 컬렉션 프레임웍의 핵심 인터페이스

   ![image](https://user-images.githubusercontent.com/66407386/173496095-dbe2e783-ddb6-4ead-b0da-60c64da2f1ab.png)

   - 컬렉션의 프레임워크 핵심 인터페이스 
   <table>
    <tr>
        <th>인터페이스</th>
        <th>설명</th>
    </tr>
    <tr>
        <td>List</td>
        <td>
        순서가 있는 데이터의 집합, 데이터의 중복을 허용<br/><br/>
        구현 클래스 : ArrayList, LinkedList, Stack, Vector 등
        </td>
    </tr>
    <tr>
        <td>Set</td>
        <td>
        순서를 유지하지 않는 데이터의 집합, 데이터의 중복을 허용하지 않는다.<br/><br/>
        구현 클래스 : HashSet, TreeSet 등
        </td>
    </tr>
    <tr>
        <td>Map</td>
        <td>
        키와 값의 쌍으로 이루어진 데이터의 집합<br/>
        순서는 유지되지 않으며, 키는 중복을 허용하지 않고, 값은 중복을 허용<br/><br/>
        구현 클래스 : HashMap, TreeMap, Hashtavle, Properties 등
        </td>
    </tr>
   </table>

##### ArrayList

##### LinkedList

##### Stack과 Queue

##### Iterator, ListIterator, Enumeration

##### Arrays

##### Comparator와 Comparable

##### HashSet

##### TreeSet

##### HashMap과 Hashtable

##### TreeMap

##### Properties

##### Collections

##### 컬렉션 클래스 정리 & 요약


## 참고 문서 / 블로그
1. [서적] 남궁성님의 Java의 정석 3rd Edition
