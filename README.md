:pushpin: 네이버 웹툰 데이터 분석
네이버 웹툰 데이터를 베이스로 데이터 분석을 해보았습니다.

1. 제작 기간 & 참여 인원
기간: 2019년 2월 4일 ~ 2월 6일

구성: 팀 프로젝트

2. 사용 기술
Python, Flask, HTML/CSS/JS

3. 화면구성[page0.html](https://github.com/user-attachments/files/25247410/page0.html)
 <!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
@font-face {
    font-family: 'Pretendard';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/pretendard@1.0/Pretendard-SemiBold.woff2') format('woff2');
    font-weight: 600;
    font-display: swap;
}

body{
    margin:0;
    /* background:#ddd; */
    background-color: whitesmoke;
    font-family:'Pretendard';
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background-image: url(../static/bge7.png);
        /* background-size: cover; */
}

/* 종이 겹침 효과 */

.paper-back{
    width:900px;
    height:520px;
    background:#cfcfcf;
    position:absolute;
    transform:rotate(-3deg);
    border:5px solid black;
}

.paper-back2{
    width:900px;
    height:520px;
    background:#bfbfbf;
    position:absolute;
    transform:rotate(2deg);
    border:5px solid black;
}

/* 메인 컷 */

.paper-main{
    width:900px;
    height:520px;
    background:white;
    border:6px solid black;
    position:relative;
    overflow:hidden;
}

/* 상단 영역 */

.top-area{
    height:65%;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:40px;
}

/* 캐릭터 */

.character{
    width:160px;
}

/* 제목 */

.title{
    font-size:48px;
    line-height:1.2;
}

.subtitle{
    font-size:14px;
    color:#666;
    letter-spacing:1px;
}

.highlight{
    background:#a8e6a3;
    padding:5px 10px;
}

/* 말풍선 */

.bubble{
    position:absolute;
    top:70px;
    right:180px;
    background:white;
    border:3px solid black;
    border-radius:20px;
    padding:8px 14px;
    font-size:14px;
}

/* 붓 오브젝트 */

.brush{
    position:absolute;
    bottom:-30px;
    right:-40px;
    width:180px;
    transform:rotate(-20deg);
}

/* ===== 하단 검정 컷 ===== */

.bottom{
    height:35%;
    background:black;
    color:white;
    padding:20px;
    font-size:13px;
}
.title-line{
    width:220px;
    height:4px;
    background:black;
    margin:15px 0 8px 0;
}

</style>
</head>

<body>

<div class="paper-back"></div>
<div class="paper-back2"></div>

<div class="paper-main">

    <div class="top-area">

        <img src="../static/WEBTOON_Logo.png" class="character">

        <div class="title">
            네이버 <span class="highlight">웹툰</span><br>
            데이터 분석
            
            <div class="title-line"></div>

            <div class="subtitle">
                Naver Webtoon Data Analysis
            </div>
        </div>

    </div>

    <!-- <div class="bubble">꿀잼각</div> -->

    <img src="./pen1.jpg" class="brush">

    <div class="bottom" onclick="location.href='/page1';" style="cursor: pointer;">
        Date - 2026.02.06 <br>
        Created by Team 일당백
    </div>

</div>

</body>
</html>

