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
  
  <!DOCTYPE html>
<html>
<head>
<title>이벤트 리스너 속성에 자바스크립트 코드</title>
</head>
<body>
<h3>마우스 올려 보세요</h3>
<hr>
<img src="media/apple.png" alt="이미지" 
			onmouseover="this.src='media/banana.png'"
			onmouseout="this.src='media/apple.png'">
</body>
</html>
