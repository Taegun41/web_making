<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>대학 다이어리</title>
    <link rel="stylesheet" href="/css/main_style.css" />
  </head>
  <body>
    <!-- 왼쪽 영역 -->
    <div class="sidebar">
      <div class="login-box" id="loginBox">
        <input type="text" id="userId" placeholder="아이디" />
        <input type="password" id="password" placeholder="비밀번호" />
        <button onclick="login()">로그인</button>
        <button onclick="register()">회원가입</button>
      </div>

      <div class="profile-box" id="profileBox">
        <img src="profile.jpg" alt="프로필" />
        <p id="profileName"></p>
        <button onclick="logout()">로그아웃</button>
      </div>

      <ul class="nav-menu">
        <li onclick="changePage('home.html')">홈</li>
        <li onclick="changePage('index.html')">게시판</li>
        <li onclick="changePage('schedule.html')">내 일정</li>
      </ul>
    </div>

    <!-- 오른쪽 영역 -->
    <div class="content">
      <iframe id="contentFrame" src="home.html"></iframe>
    </div>

    <script src="/js/main_script.js"></script>
  </body>
</html>
