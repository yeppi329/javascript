<h3>Javascript</h3><br>
  1995년 넷스케이프 개발<br>
  Netscape Navigator 2.0 브라우저에 최초 탑재<br>
  웹 프로그래밍 개념 창시<br>
<h3>특징</h3><br>
  HTML 문서에 내장<br>
   - 조각 소스 코드<br>
  스크립트 언어<br>
   - 인터프리터 실행<br>
   - 컴파일 필요 없음<br>
  단순<br>
   - C언어 구조 차용<br>
   - 배우기 쉬움<br>
<h3>자바스크립트 코드 작성이 가능한 위치</h3><br>
  1. HTML 태그의 이벤트 리스너 속성에 작성<br>
  2. <script></script> 태그에 작성<br>
  3. 자바스크립트 파일에 작성<br>
  4. URL 부분에 작성<br>
<br>

[예제 6-1 HTML 태그의 이벤트 리스너 속성에 자바스크립트 코드 작성](https://github.com/yeppi329/javascript/blob/main/ex6_1)
<br>
<h3><script></script> 태그에 자바스크립트 작성</h3><br>
  특징<br>
   - <head></head>나 <body></body> 내 어디든 가능<br>
   - 웹 페이지 내에 여러 번 삽입 가능<br>
   <br>

[예제 6-2 <script>태그에 자바스크립트코드작성](https://github.com/yeppi329/javascript/blob/main/ex6_2)
<br>
<h3>자바스크립트 코드를 별도 파일에 작성</h3>
  자바스크립트 코드 파일 저장<br>
   - 확장자 .js 파일에 저장<br>
   - <script> 태그 없이 자바스크립트 코드만 저장<br>
  여러 웹 페이지에서 불러 사용<br>
   - 웹 페이지마다 자바스크립트 코드 작성 중복 불필요<br>
   - <script> 태그의 src 속성으로 파일을 불러 사용<br>
```
<script src=“파일이름.js”>
    // HTML5부터 이곳에 자바스크립트 코드 추가 작성하면 안 됨
</script>
```
	<br>
[예제 6–3 자바스크립트 파일 작성 및 불러오기](https://github.com/yeppi329/javascript/blob/main/ex6_3)<br>
예제 6–2의 <script> 태그에 들어 있는 자바스크립트 코드를 lib.js 파일에 저장하고 불러와서 사용하도록 수정하라.  <br>
```  
/* 자바스크립트 파일 lib.js */
function over(obj) {
	obj.src="media/banana.png";
}
function out(obj) {
	obj.src="media/apple.png";
}
```
```
<!DOCTYPE html>
<html>
<head><title>외부 파일에 자바스크립트 작성</title>
<script src="lib.js">
</script>
</head>
<body>
<h3>마우스 올려 보세요</h3>
<hr>
<img src="media/apple.png" alt="이미지" 
		onmouseover="over(this)"
		onmouseout="out(this)">
</body>
</html>
```
