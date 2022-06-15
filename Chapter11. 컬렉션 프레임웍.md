## Chapter11. 컬렉션 프레임웍

1. [컬렉션 프레임웍(Collection Framework)](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%BB%AC%EB%A0%89%EC%85%98-%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8Dcollection-framework '컬렉션 프레임웍(Collection Framework)')
   - [1-1. 컬렉션 프레임웍의 핵심 인터페이스](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%BB%AC%EB%A0%89%EC%85%98-%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D%EC%9D%98-%ED%95%B5%EC%8B%AC-%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4 '컬렉션 프레임웍의 핵심 인터페이스')
   - [1-2. ArrayList](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#arraylist 'ArrayList')
   - [1-3. LinkedList](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#linkedlist 'LinkedList')
   - [1-4. Stack과 Queue](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#stack%EA%B3%BC-queue 'Stack과 Queue')
   - [1-5. Iterator, ListIterator, Enumeration](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#iterator-listiterator-enumeration 'Iterator, ListIterator, Enumeration')
   - [1-6. Arrays](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#arrays 'Arrays')
   - [1-7. Comparator와 Comparable](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#comparator%EC%99%80-comparable 'Comparator와 Comparable')
   - [1-8. HashSet](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#hashset 'HashSet')
   - [1-9. TreeSet](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#treeset 'TreeSet')
   - [1-10. HashMap과 Hashtable](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#hashmap%EA%B3%BC-hashtable 'HashMap과 Hashtable')
   - [1-11. TreeMap](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#treemap 'TreeMap')
   - [1-12. Properties](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#properties 'Properties')
   - [1-13. Collections](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#collections 'Collections')
   - [1-14. 컬렉션 클래스 정리 & 요약](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%BB%AC%EB%A0%89%EC%85%98-%ED%81%B4%EB%9E%98%EC%8A%A4-%EC%A0%95%EB%A6%AC--%EC%9A%94%EC%95%BD '컬렉션 클래스 정리 & 요약')
2. [참고 문서 / 블로그](https://github.com/hongcoding94/java_storage/blob/main/Chapter11.%20%EC%BB%AC%EB%A0%89%EC%85%98%20%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8D.md#%EC%B0%B8%EA%B3%A0-%EB%AC%B8%EC%84%9C--%EB%B8%94%EB%A1%9C%EA%B7%B8 '참고 문서 / 블로그')

## 컬렉션 프레임웍(Collection Framework)

- 컬렉션이란?

  > 사전적 의미 : 요소를 수집해서 저장하는 것
  > 다수의 데이터를 쉽고 효과적으로 처리할 수 있고 표준화된 방법을 제공하는 클래스의 집합
  > 즉, 데이터를 저장하는 자료구조와 데이터를 처리하는 알고리즘을 구조화하여 클래스로 구현해 놓은 것.
  >
  > - 자료구조 유형의 종류
  >
  >   - List : 순서가 있는 목록
  >   - Set : 순서가 중요하지 않은 목록
  >   - Queue : 먼저 들어온 순으로 나가는 목록
  >   - Map : Key | Value의 형태로 저장
  >
  > - 인터페이스로 가능한 컬렉션 클래스를 나타내는 자료
  >   ![image](https://user-images.githubusercontent.com/66407386/173496159-c6f3935f-6ef5-4109-9e04-7898888c9364.png)

- 컬렉션(Collection) 인터페이스의 메서드
<table>
    <tr>
        <th>메서드</th>
        <th>설명</th>
    </tr>
    <tr>
        <td>
            boolean add(object o)<br />
            boolean addAll(Collection c)
        </td>
        <td>
         지정된 객체(o)를 Collection에 추가<br />
        지정된 Collection(c)의 객체들을 Collection에 추가
        </td>
    </tr>
    <tr>
        <td>
        boolean contains(Object o)<br />
        boolean containsAll(Collection c)
        </td>
        <td>
        지정된 객체(o)가 Collection에 포함 되어 있는지 확인<br />
        지정된 Collection(c)의 객체들이 Collection에 포함 되어 있는지 확인
        </td>
    </tr>
    <tr>
        <td>
        void clear()
        </td>
        <td>
        Collection의 모든 객체를 삭제한다.
        </td>
    </tr>
    <tr>
        <td>
        boolean isEmpty()
        </td>
        <td>
        Collection이 비어있는지 확인
        </td>
    </tr>
    <tr>
        <td>
        int size()
        </td>
        <td>
        Collection에 저장된 객체의 개수를 반환
        </td>
    </tr>
</table>

- 컬렉션 프레임워크
  > 사전적 의미 : 표준화, 정형화된 프로그래밍 방식
  > 컬렉션을 다루기 위한 표준화된 프로그래밍 방식이며 컬렉션을 쉽고 편리하게 다룰 수 있는 다양한 클래스를 제공
  > 데이터 군집의 형태를 크게 3가지로 나눠서 각각의 데이터 군집 형태를 인터페이스로 정의
  >
  > - 컬렉션프레임워크 핵심 인터페이스
  >
  > 1. List
  > 2. Set
  > 3. Map
  >
  > ※ 이중에서 List와 set은 공통부분들이 있어서 Collection 인터페이스로 정의하였다.
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

- List 인터페이스
>  저장 순서가 유지되고 중복을 허용하는 컬렉션을 구현하는데 사용 <br />
>  ![image](https://user-images.githubusercontent.com/66407386/173521625-b04b3ae5-a385-4229-8f5e-10dc1bd459f9.png)
>   - java.util.List의 메소드 종류
>   <table>
>   <tr>
>       <th>메소드</th>
>       <th>내용</th>
>   </tr>    
>   <tr>
>       <td>ArrayList</td>
>       <td>
>   	List 컬렉션 인터페이스를 구현하는 클래스<br/>
>   	일반 배열과 ArrayList는 인덱스로 객체를 관리한다는 점은 동일하지만,<br/>
>   	<B>크기를 동적</B>으로 늘릴 수 있다는 점에서 차이가 있다.
>       </td>
>   </tr>
>   <tr>
>       <td>Verctor</td>
>       <td>
>   	ArrayLsit와 동일한 구조를 가지며 배열의 크기가 동적으로 작동하며<br/>
>   	항상 동기화 되어 있어 Collection 프레임워크 없이 메서드를 사용 가능<br/>
>   	<b>단, 동기화 특징상 스레드가 아닌 환경에서는 거의 사용 하지 않는다.</b> 
>       </td>
>   </tr>  
>   <tr>
>       <td>LinkedList</td>
>       <td>
>   	각 노드가 데이터와 포인터를 가지고 한줄로 연결되어 있는 방식의 자료구조<br/>
>   	쉽게 설명을 하자면 해당 건물(공간) 안에 직원(값)의 배분을 한층한칸씩 차례대로<br/>
>   	배분하는 것이 아닌 건물(공간) 안의 방을 빈 공간을 찾아 배분한다.<br/>
>   	만약 이해가 되지 않는다면 <b>"참고 문서 / 블로그 2번을 참조하자"</b> <br/>
>   	단, 추가 혹은 삭제는 용이하나 탐색하는 속도가 많이 느리다는 단점을 가지고있다.
>       </td>
>   </tr>
>   </table>
> 
>   - List 인터페이스에 정의된 메서드
>   <table>
>      <tr>
>           <th>메서드</th>
>           <th>설명</th>
>      </tr>
>      <tr>
>           <td>
>               void add(int index, Object e)<br />
>               boolean addAll(int idnex, Collection c)
>           </td>
>           <td>
>               지정된 위치(index)에 객체(e - element) 또는 컬렉션에 포함된 객체들을 추가
>           </td>
>      </tr>
>      <tr>
>           <td>
>               Object get(int index)
>           </td>
>           <td>
>               지정된 위치(index)에 있는 객체를 반환
>          </td>
>      </tr>
>      <tr>
>           <td>
>               int indexOf(Object o)
>           </td>
>           <td>
>               지정된 객체의 위치(index)를 반환<br />
>               (List의 마지막 요소부터 순방향으로 찾음)
>           </td>
>      </tr>
>      <tr>
>           <td>
>               int lastIndexOf(Object o)
>           </td>
>           <td>
>               지정된 객체의 위치(index)를 반환<br />
>               (List의 마지막 요소부터 역방향으로 찾음)
>           </td>
>      </tr>
>      <tr>
>           <td>
>               Object remove(int index)
>           </td>
>           <td>
>               지정된 위치(index)에 있는 객체를 삭제하고 삭제된 객체를 반환
>           </td>
>      </tr>
>      <tr>
>           <td>
>               Object set(int index, Object e)
>           </td>
>           <td>
>               지정된 위치(index)에 객체(e - element) 저장 
>           </td>
>      </tr>
>      <tr>
>           <td>
>               void sort(Comparator c)
>           </td>
>           <td>
>               지정된 비교자(comparator)로 List를 정렬
>           </td>
>      </tr>
>      <tr>
>           <td>
>               List SubList(int fromIndex, int tolndex)
>           </td>
>           <td>
>               지정된 범위(fromIndex부터 toIndex)에 있는 객체를 반환<br />
>               (일부만 뽑아내어 새로운 List 생성)
>           </td>
>      </tr>
>   </table>

- Set 인터페이스
> 저장 순서가 유지되지 않고 중복을 허용하지 않는 컬렉션을 구현하는데 사용
> ![image](https://user-images.githubusercontent.com/66407386/173524353-da2476d6-7571-4069-94e0-31080bc667bd.png)
> - java.util.Set의 메소드 종류
> <table>
>  <tr>
>     <th>메소드</th>
>     <th>내용</th>
>  </tr>
>  <tr>
>     <td>HashSet</td>
>     <td>
>     순서대로 입력되지 않고, 일정하게 유지되지 않으며 HashSet은 null 요소도<br/>
>     허용하지만 중복을 허용하지 않는다.<br />
>     <br />
>     ❓ Why - 중복을 어떻게 걸러내는거지?<br />
>     객체를 저장 하기 전 hashCode메소드를 호출하여 해시코드를 얻어 저장되어<br />
>     있는 객체들의 해시코드와 비교한 뒤 같은 해시 코드가 있다면<br />
>     두객체를 비교하여 동일한 객체로 판단시 중복 저장을 하지 않는다.
>     </td>
>  </tr>
>  <tr>
>     <td>TreeSet</td>
>     <td>
> 	HashSet과 비슷하게 구조를 가져와서 중복 데이터를 저장하지 않고 <br />
> 	저장 순서를 유지하지 않는다는 성질을 가진다.<br />
>      단, TreeSet은 이진 탐색 트리(BinarySearchTree) 구조로 되어 있다.<br />
> 	이진 탐색 트리 이해하기 ➡️ [클릭](https://yoongrammer.tistory.com/71)
>     </td>
>  </tr>
> </table>
>
>  - Set 인터페이스에 정의된 메서드
>   <table>
>      <tr>
>           <th>메서드</th>
>           <th>설명</th>
>      </tr>
>      <tr>
>           <td>
>               boolean addAll(Collection c)
>           </td>
>           <td>
>               지정된 Collection(c)의 객체들을 Collection에 추가 - [합집합]
>           </td>
>      </tr>
>      <tr>
>           <td>
>               boolean containsAll(Collectiokn c)
>           </td>
>           <td>
>               지정된 Collection의 객체들이 Collection에 포함되어 있는지 확인 - [부분집합]
>           </td>
>      </tr>
>      <tr>
>           <td>
>               boolean removeAll(Collection c)
>           </td>
>           <td>
>               지정된 Collectiokn에 포함된 객체들을 삭제 - [차집합]
>           </td>
>      </tr>
>      <tr>
>           <td>
>               boolean retainAll(Collection c)
>           </td>
>           <td>
>               지정된 Collection에 포함된 객체만을 남기고 나머지 Collection에서 삭제 - [교집합]
>           </td>
>      </tr>
>   </table>


- Map 인터페이스
> 저장 순서가 유지되지 않고 키는 중복을 허용하지 않고 값은 중복을 허용하는 컬렉션을 구현하는데 사용<br />
> ※ 저장 순서를 유지 해야하는 경우, Map 인터페이스의 구현체 중에 LinkedHashMap을 사용
>
> - java.util.Map의 메소드 종류
> <table>
>  <tr>
>     <th>메소드</th>
>     <th>내용</th>
>  </tr>
>  <tr>
>     <td>HashMap</td>
>     <td>
> 	Hashing(키 값에 직접 산술적인 연산을 적용하여 테이블의 주소를 게산하여 항목에 접근) / Map 의 조합<br />
>      즉, 키와 값 한쌍으로 데이터를 보관하는 자료 구조이다.<br />
>      키는 맵에 오직 유일해야하며 값은 중복된 값이여도 문제가 없다.
> 	</td>
>  </tr>
>  <tr>
>     <td>HashTable</td>
>     <td>
>      키와 값을 데이터를 저장하는 자료구조이며 자료구조 중 하나로 빠르게 데이터를 검색할 수 있는 자료구조<br />
> 	즉, 내부적으로 배열을 사용하여 데이터를 저장 하기 때문이다.<br /> 
> 	<b>(각각의 Key에 해시 함수를 적용해 배열의 고유한 index를 생성)</b>
>     </td>
>  </tr>
>  <tr>
>     <td>TreeMap</td>
>     <td>
>     이진트리를 기반으로 한 Map 컬렉션<br />
>     TreeSet과의 차이점은 TreeSet은 그냥 값만 저장한다면 TreeMap은 키와 값이 저장된 Map, Etnry를 저장한다<br />
>     또한 TreeMap에 객체를 저장하면 자동으로 정렬되는데, 키는 저장과 동시에 자동 오름차순으로 정렬되고<br />
>     숫자 타입일 경우에는 값으로, 문자열 타입일 경우에는 유니코드로 정렬
>     </td>
>  </tr>
>  <tr>
>     <td>Properties</td>
>     <td>
>     HashTbles의 하위 클래스이며 HashTables를 상속을 받았기 떄문에 Map의 속성 키와 값을 갖는다.<br />
>     HashMap과 큰 차이는 없지만 파일 입출력을 지원한다.
>     </td>
>  </tr>
> </table>
>
> - Map 인터페이스에 정의된 메서드
> <table>
>    <tr>
>         <th>메서드</th>
>         <th>설명</th>
>    </tr>
>    <tr>
>         <td>
>               Object put(Object key, object value)
>         </td>
>         <td>
>               Key 객체에 Value 객체를 연결하여 Map에 저장
>         </td>
>    </tr>
>    <tr>
>         <td>
>               void putAll(Map t)
>         </td>
>         <td>
>               지정된 Map의 모든 Key-Value 한쌍을 추가
>         </td>
>    </tr>
>    <tr>
>         <td>
>               boolean containsKey(Object key)
>         </td>
>         <td>
>               지정된 Key 객체와 일치하는 Map의 Key객체가 있는지 확인
>         </td>
>    </tr>
>    <tr>
>         <td>
>               boolean containsValue(Object value)
>         </td>
>         <td>
>               지정된 Value 객체와 일치하는 Map의 Value 객체가 있는지 확인
>         </td>
>    </tr>
>    <tr>
>         <td>
>               Object get(Object key)
>         </td>
>         <td>
>               지정된 Key 객체와 일치하는 Value 객체를 찾아서 반환
>         </td>
>    </tr>
>    <tr>
>         <td>
>               Object remove(Object key)
>         </td>
>         <td>
>               지정된 Key객체와 일치하는 key-Value 객체를 삭제
>         </td>
>    </tr>
>    <tr>
>         <td>
>               Set entrySet()
>         </td>
>         <td>
>               Map에 저장되어 있는 Key-Value 한쌍을<br />
>               Map.Entry타입의 객체로 저장한 Set으로 반환
>         </td>
>    </tr>
>    <tr>
>         <td>
>               Set keySet()
>         </td>
>         <td>
>               Map에 저장된 모든 key 객체를 반환
>         </td>
>
>    </tr>
>    <tr>
>         <td>
>               Collection values()
>         </td>
>         <td>
>               Map에 저장된 모든 Value 객체를 반환
>         </td>
>
>    </tr>
> </table>

##### ArrayList
  - ArrayList이란?
  > List 인터페이스를 상속받은 클래스이며 크기가 가변적으로 변하는 선형리스트<br/>
  > 일반적인 배열과 같은 순차리스트이며 인덱스로 내부의 객체를 관리한다는 점이 비슷하지만<br/>
  > 한번 생성하면 크기가 변하지 않은 배열과 달리 ArrayList는 객체들이 추가되어 저장 용량이<br/>
  > 초과한다면 자동으로 부족한 크기만큼 저장요량이 늘어난다는 특징

  <br/>
  <img src="https://user-images.githubusercontent.com/66407386/173502482-24de70f2-ac3f-46c9-a8df-a4cd8a846637.png">

   - ArrayList 선언
   > ```java
   > // ArrayList 선언
   > ArrayList isList = new ArrayList();
   > 
   > // ArrayList 타입 설정
   > ArrayList<Type> isListType = new ArrayList<Type>(용량); 
   >
   > // ArrayList 추가
   > isList.add(데이터 입력);
   >
   > // ArrayList 부분삭제
   > isList.remove(index);
   >
   > // ArrayList 전체 삭제
   > isList.clear();
   >
   > // ArrayList 사이즈 크기 구하기
   > System.out.println(isList.size());
   >
   > // ArrayList 값 출력 - for문
   > for(Integer i : isList) {
   >     System.out.println(i);
   > }
   >
   > // ArrayList 값 출력 - while
   > Iterator iter = isList.iterator();
   > while(iter.hasNext()){//다음값이 있는지 체크
   >     System.out.println(iter.next());
   > }
   > ```
   
##### LinkedList

  <br/>
  <img src="https://user-images.githubusercontent.com/66407386/173503205-5b5f501e-5e4b-4443-abbb-69e44a047bda.png">

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
2. [블로그] [opentutorials님의 Data Structure(자료구조)](https://opentutorials.org/module/1335/8821)
3. [블로그] [yoongrammer님의 [자료구조] 이진 탐색 트리 (BST, Binary Search Tree)](https://yoongrammer.tistory.com/71)
4. [블로그] [망나니개발자님의 [자료구조] 해시테이블(HashTable)이란?](https://mangkyu.tistory.com/102)
