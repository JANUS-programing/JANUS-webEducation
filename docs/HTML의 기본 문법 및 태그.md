# HTML의 기본 문법 및 태그

HTML 페이지는 태그를 이용해서 각 부분을 구분하고, 그 기능에 맞는 형식을 가지게 됩니다. 아래의 예시와 같이 기본적인 태그들을 살펴보겠습니다.

```html
<!DOCTYPE html>
<html lang="ko">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>기본 HTML 예제</title>
</head>

<body>
    <h1>기본 HTML 예제</h1>

    <!-- 테이블 예시 -->
    <h2>테이블 예시</h2>
    <table border="1">
        <tr>
            <th>항목</th>
            <th>설명</th>
        </tr>
        <tr>
            <td>태그</td>
            <td>HTML의 기본 요소입니다.</td>
        </tr>
        <tr>
            <td>속성</td>
            <td>태그의 추가 정보를 제공합니다.</td>
        </tr>
    </table>

    <!-- 목록 예시 -->
    <h2>목록 예시</h2>
    <ul>
        <li>항목 1</li>
        <li>항목 2</li>
        <li>항목 3</li>
    </ul>

    <!-- 폼 예시 -->
    <h2>로그인 폼 예시</h2>
    <form action="#" method="post">
        <label for="username">아이디:</label>
        <input type="text" id="username" name="username"><br><br>
        
        <label for="password">비밀번호:</label>
        <input type="password" id="password" name="password"><br><br>
        
        <button type="submit">로그인</button>
    </form>

    <hr>
    <p>본 페이지는 기본 HTML 태그를 설명하기 위한 예제 페이지입니다.</p>

</body>

</html>
```