<h1># JavaUntitle</h1>
<p>자바 , 이것저것 ... </p>

<h2>equals() 에 대해서 </h2>
<pre>
equals() 메소드의 목적은 값 비교 이다.
equals() 는 앞에 null.equals("{data}") 이렇게 하게 되면 null point error 가 발생한다.
"{data}".equals(null) 은 비교 가능하며 false를 return
</pre>
<h2>HashCode 란 무엇인가?</h2>
<pre>
해시코드는 해시 알고리즘에 의해 생성된 정수 값.
같은 객체라면 반드시 같은 해시코드 값을 반환해야 하고
다른 객체임에도 같은 해시코드 값을 가질수 있다.

.... 더 알아보기!
</pre>
<h2>String 과 Char의 차이</h2>
<pre>
String 클래스는 Char배열을 할당 받는다.

char a1 = 'a' 는 a1 변수안에 'a' 라는 값을 가진다.
String a1 = 'a1' 는 'a1'라는 값이 위치한 좌표값을 가진다.

String number = "12345";
String number2 = "12345";
String number3 = new String("12345");
String number4 = new String("12345");

System.out.println(number.equals(number2));  // 내용물을 비교한다.
System.out.println(number == number2);       // 주소값을 비교한다.
System.out.println(number3.equals(number4)); // 내용물을 비교한다.
System.out.println(number3 == number4);      // 주소값을 비교한다.

출력값
true 
true
true
false

</pre>

<h2>엑셀 다운로드 하면서 삽질...</h2>
<pre>
계속 기존에 ExcelView 라이브러리에서 캐스팅을 못하길래 삽질 하던 와중....
HSSFWorkbook workbook = (HSSFWorkbook) transformer.transformXLS(inputStream, beans);  // 2003년 버전 엑셀
XSSFWorkbook workbook = (XSSFWorkbook) transformer.transformXLS(inputStream, beans); // 2003년 이후 버전 엑셀….

휴...
</pre>
