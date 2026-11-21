<!DOCTYPE html>
<html lang="zh-Hant">

<head>
  <meta charset="UTF-8">
  <title>荒野亂鬥介紹網頁</title>
  
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />

  <style>
    body {
      background-color: rgb(166, 182, 184);
      margin: 0;
      padding: 0;
      font-size: 28px;
      font-family: "PingFang TC", "Microsoft JhengHei", sans-serif;
    }
    p.one {
      background-color: grey; 
      font-size: 50%
    }
    #p_1 {
      color: blueviolet;
      text-align: center;
    }

    p.go {
      text-align: center;
      margin: 40px 10px 10px 10px;
      font-size: 200%;
      font-weight: bold;
    }

    p.center {
      text-align: center;
    }

    p.small {
      text-align: center;
      font-size: 75%;
    }

    .simple-center {
      text-align: center;
    }

    h2 {
      margin: 10px;
    }
    aside{
      width:40%;
      padding: 15px;
      margin-left: 20px;
      float:right;
      background-color:rgb(214, 214, 34);
      border-radius: 10px;
    }
    
    ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      overflow: hidden;
      background-color: #333333;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    ul li {
      float: left;
    }

    ul li a {
      display: block;
      color: white;
      text-align: center;
      padding: 20px 16px;
      text-decoration: none;
    }

    ul li.word a:hover {
      background-color: blueviolet;
    }

    p.small2 {
      color: blue;
    }

    
    .hero-slider-section {
      width: 100%;
      height: 500px;
      position: relative;
      overflow: hidden;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
      background-color: #1a1a1a;
      will-change: opacity; opacity: 1;
    }

    .hero-swiper {
      width: 100%;
      height: 50%;
    }

    .hero-slide {
      position: relative;
      width: 100%;
      height: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    
    .hero-slide img {
      width: 100%;
      height: 100%;
      object-fit: contain; 
    }

   
    .hero-caption {
      position: absolute;
      bottom: 150px; 
      left: 0;
      width: 100%;
      background: linear-gradient(transparent, rgba(0, 0, 0, 0.75), transparent); 
      color: white;
      padding: 20px 40px;
      box-sizing: border-box;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.6);
    }

    .hero-caption h3 {
      margin: 0 0 10px 0;
      font-size: 36px;
    }

    .hero-caption p {
      margin: 0;
      font-size: 20px;
      color: #e0e0e0;
    }

   
    .hero-swiper .swiper-button-next, 
    .hero-swiper .swiper-button-prev {
      color: #fff;
      background: rgba(138, 43, 226, 0.6);
      width: 60px;
      height: 60px; 
      border-radius: 50%;
    }
    .hero-swiper .swiper-button-next:hover{
      background: rgba(138, 43, 226, 0.9);
    } 
    .hero-swiper .swiper-button-prev:hover {
      background: rgba(138, 43, 226, 0.9);
    }
    .hero-swiper .swiper-pagination-bullet-active {
      background: #fff !important;
      width: 25px; 
      border-radius: 5px;
    }

    
    div.mycontainer {
      overflow: auto;
      display: flex;
      flex-wrap: wrap;
    }

    div.mycontainer div {
      margin: 10px;
    }

    div.carl, div.penny, div.shelly {
      width:100%;
      overflow:auto;
      margin-bottom: 30px;
    }
    div.carl div, div.penny div, div.shelly div {
      width:50%;
      float:left;
      box-sizing: border-box;
      padding: 10px;
    }

    
    .chat-section {
      background: rgba(255, 255, 255, 0.8);
      padding: 20px;
      margin: 20px;
      border-radius: 15px;
      text-align: center;
    }

    #display {
      margin-bottom: 15px;
      font-weight: bold;
      color: #333;
    }

    input[type="text"] {
      font-size: 20px;
      padding: 10px;
      width: 60%;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    button {
      font-size: 20px;
      padding: 10px 20px;
      cursor: pointer;
      background-color: blueviolet;
      color: white;
      border: none;
      border-radius: 5px;
    }

    button:hover {
      background-color: #7a2edb;
    }
    
    div.first {
      background-color:rgb(75, 33, 33);
    }
    
    footer {
      background-color: #777;
      padding: 10px;
      text-align: center;
      color: white;
      clear: both;
    }
      div.shellyb {
        width:100%;
        overflow:auto;                    
      }
      div.shellyb div {
        width:14%;
        float:left;
        border-radius:30px;
      }
      div.shellyb h1 {
        margin-top: 0;          
        text-align: auto;     
      }
      div.ultra{
        background-image: url("srdmhkerhaxe1.gif");
        height:600px;
      }
      .video-overlay {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 60%;
        z-index: 2;
        background: rgba(0, 0, 0, 0);
        pointer-events: none;
        will-change: background;
      }
      .zoom-img {
          width: 100%;
          height: auto;
          display: block; 
          border-radius: 8px; 
          transition: transform 0.3s ease, box-shadow 0.3s ease; 
      }
      .zoom-img:hover {
          transform: scale(1.05); 
          box-shadow: 0 10px 20px rgb(0, 255, 55);
      }
      .zoom-img-99 {
          width: 100%;
          height: auto;
          display: block; 
          border-radius: 8px; 
          transition: transform 0.3s ease, box-shadow 0.3s ease; 
      }
      .zoom-img-99:hover {
          transform: scale(1.05); 
          box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
      }
    </style>
</head>

<body>
  <ul>
    <li><a href="file:///Q:/%E6%88%91%E7%9A%84%E9%9B%B2%E7%AB%AF%E7%A1%AC%E7%A2%9F/Students/ryderwang/brawlstarsweb.html"><img src="Brawl Stars Logo.png" alt="Logo" style="width:70px;height:50px;"></a></li>
    <li class="word"><a class="active" href="#home">首頁</a></li>
    <li class="word"><a href="#introduction">簡介</a></li>
    <li class="word"><a href="#skills">戰鬥技巧</a></li>
    <li class="word"><a href="#brawlers">英雄介紹</a></li>
    <li class="word"><a href="#new">全新角色</a></li>
    <li class="word"><a href="#nb">全新更新</a></li>
    <li class="word"><a href="#search">搜尋問答</a></li>
  </ul>
  
  <div class="video-overlay" id="overlay"></div>
  
  <div class="hero-slider-section" id="home">
    <div class="swiper heroSwiper" id="heroContent"> 
      <div class="swiper-wrapper">
        
        <div class="swiper-slide hero-slide">
          <img src="fast 3v3 battels.webp" alt="荒野亂鬥" style="width:100%; height:500px;">
          <div class="hero-caption">
            <h3>進入荒野，開始亂鬥！</h3>
            <p>在三分鐘內完成快節奏對戰，與好友並肩作戰！</p>
          </div>
        </div>

        <div class="swiper-slide hero-slide">
          <img src="rank up.webp" alt="排位賽" style="width:100%; height:500px;">
          <div class="hero-caption">
            <h3>刺激的排位賽!</h3>
            <p>測試出你真正的實力!!!</p>
          </div>
        </div>
        
        <div class="swiper-slide hero-slide">
          <img src="Thunderfrogs.webp" alt="更新" style="width:100%; height:500px;">
          <div class="hero-caption">
            <h3>2026全新英雄</h3>
            <p>等待更精彩的活動!</p>
          </div>
        </div>
        
        <div class="swiper-slide hero-slide">
          <img src="royle.webp" alt="史詩" style="width:100%; height:480px;">
          <div class="hero-caption">
            <h3>皇家活動</h3>
            <p>等待更刺激的皇家戰鬥!</p>
          </div>
        </div>

      </div>
      <div class="swiper-pagination"></div>
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>
      
    </div>
  </div>

<script>
    const overlay = document.getElementById('overlay');
    const heroContent = document.getElementById('heroContent');
    
    const heroHeight = window.innerHeight * 0.8; 

    window.addEventListener('scroll', () => {
      const scrollTop = window.scrollY;
      
      let progress = scrollTop / heroHeight;
      if (progress > 1) progress = 1;
      if (progress < 0) progress = 0;

      const alpha1 = progress * 0.85; 
      const alpha2 = progress * 0.95; 

      overlay.style.background = `linear-gradient(135deg, 
        rgba(0, 0, 0, ${alpha1}) 0%, 
        rgba(0, 0, 0, ${alpha2}) 100%)`;

      if (heroContent) {
        heroContent.style.opacity = Math.max(0, 1 - progress * 2);
        
        heroContent.style.transform = `translateY(${-progress * 150}px) scale(${1 - progress * 0.1})`;
      }
    });
  </script>
</body>
    <p class="go">歡迎來到荒野的世界!</p>
  <p class="small">目前在這個「荒野」裡，已經有 111 位強大英雄等著你解鎖！</p>
  
  <p class="go" id="introduction">簡介<img src="emoji_pierce_gg.png" style="width:50px;"></p>
  <p style="padding-left: 20px;">在這個荒野裡，有多種模式：荒野死鬥，寶石爭霸，亂鬥足球，淘汰賽...</p>
  <p style="padding-left: 20px;">這些模式都可以與好朋友並肩作戰!</p>
  <p style="padding-left: 20px;">不但可以增進與好朋友的關係還可以練習許多戰鬥技巧!</p>
  <p class="small2" style="padding-left: 20px;">荒野死鬥：有分三人，二人與一人</p>
  
  <aside> 
      <a href="https://www.youtube.com/c/kairostimegaming">
          <img class="zoom-img" src="k-a-i-r-o-s-code-kairos-in-the-brawl-stars-shop-art-by-me-v0-lycuwax4v9z41.webp" alt="kairos youtube">
      </a> 
      <p style="font-size: 20px;">如果想來觀看kairos的頻道，快來點擊圖片!另外，並在brawl stars支持他！</p> 
  </aside>

  <div class="mycontainer">
    <div>
      <p>單人模式：</p>
      <img class="zoom-img" src="solo showdown.jpg" style="width: 100%; max-width: 300px; height:183px;">
    </div>
    <div>
      <p>雙人模式：</p>
      <img class="zoom-img"  src='duo showdown.jpg' style="width: 100%; max-width: 300px; height:183px;">
    </div>
    <div>
      <p>三人模式：</p>
      <img class="zoom-img"  src='trio showdown.webp' style="width: 100%; max-width: 400px;">
    </div>
  </div>

  <p class="go" id="skills">戰鬥技巧</p>
  <h1>carl(卡爾)的戰鬥技巧!</h1>
  <div class="carl">
    <div>
      <p>卡爾的最推薦配件是!飛天鉤爪!(flying hook)</p>
      <p>這是它的介紹!</p>
      <img class="zoom-img-99" src="flying hook.png" style="max-width:100%; height:50%;">
    </div>
    <div>
      <p>這是它的使用方式:</p>
      <img class="zoom-img-99" src="carl.gif" style="max-width: 50%; height:50%;">
    </div>
  </div>

  <h1>penny(佩妮)的戰鬥技巧!</h1>
  <div class="penny">
    <div>
      <p>當佩妮的子彈打到人時，子彈會散開並對周圍的人造成傷害。</p>
      <p>這是它的使用方式:</p>
      <img class="zoom-img-99" src="penny.webp" style="width:100%; max-height:600px; object-fit: cover;">
    </div>
  </div>

  <h1>shelly(雪莉)的戰鬥技巧!</h1>
  <div class="shelly">
    <div>
      <p>雪莉的超級緒能不但可以造成極大傷害，也能將對手擊退。</p>
      <p>這是它的使用方式:</p>
      <img class="zoom-img-99" src="shelly.gif" style="width:100%; max-height:600px; object-fit: cover;">
    </div>
  </div>
  <p class="go" id="brawlers">英雄性能與介紹(常見角色)</p>
  <div class="shellyb">
    <div style="background-color:lightblue; height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Shelly">雪莉</a></h1>
      <p>
      稀有度：<br>
      初始英雄<br>
      職業:<br>
      輸出<br>
      移動速度：<br>
      770（快）<br>
      924（使用極限威能）<br>
      2400（使用配件）</p>
    </div>
    <div style="background-color:rgb(50, 193, 44); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Colt">柯爾特</a></h1>
      <p>
      稀有度：<br>
      稀有<br>
      職業：<br>
      輸出<br>
      移動速度：<br>
      720（普通）<br>
      814（裝備星之能量）<br>
      864（裝備極限威能）<br>
      958（裝備星之能量和極限威能）</p>
    </div>
    <div style="background-color:rgb(37, 130, 192); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Dynamike">爆破麥克</a></h1>
      <p>
      稀有度：<br>
      超稀有<br>
      職業：<br>
      壓制<br>
      移動速度：<br>
      770（快）<br>
      814（裝備星之能量）<br>
      864（裝備極限威能）<br>
      958（裝備星之能量和極限威能）</p>
    </div>
    <div style="background-color:rgb(37, 130, 192); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Gus">格斯</a></h1>
      <p>
      稀有度：<br>
      超稀有<br>
      職業：<br>
      支援<br>
      移動速度：<br>
      750（普通）</p>
    </div>
    <div style="background-color:rgb(127, 79, 201); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Edgar">艾德加</a></h1>
      <p>
      稀有度：<br>
      史詩<br>
      職業：<br>
      刺客<br>
      移動速度：<br>
      820（極快）<br>
      1020（使用超級續能後）<br>
      984（裝備極限威能）<br>
      958（裝備極限威能且使用超級續能後）</p>
    </div>
    <div style="background-color:rgb(212, 12, 0); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Fang">范</a></h1>
      <p>
      稀有度：<br>
      神話<br>
      職業：<br>
      刺客<br>
      移動速度：<br>
      770（快）<br>
      924（裝備極限威能）<br>
      4000(裝備超級續能)</p>
    </div>
    <div style="background-color:rgb(212, 12, 0); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Vince">文斯</a></h1>
      <p>
      稀有度：<br>
      神話<br>
      職業：<br>
      輸出<br>
      移動速度：<br>
      750（普通）</p>
    </div>
    <div style="background-color:rgb(255, 239, 0); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Chester">查斯特</a></h1>
      <p>
      稀有度：<br>
      傳奇<br>
      職業：<br>
      輸出<br>
      移動速度：<br>
      770（快）<br>
      920（裝備武裝配件）<br>
      955（裝備極限威能）<br>
      1105（裝備武裝配件和極限威能）</p>
    </div>
    <div style="background-color:rgb(255, 239, 0); height:600px; width: 300px;" class="zoom-img">
      <h1><a href="https://brawlstars.fandom.com/wiki/Nori">憲</a></h1>
      <p>
      稀有度：<br>
      傳奇<br>
      職業：<br>
      刺客<br>
      移動速度：<br>
      855（超快）<br>
      1026（裝備星之能量）</p>
    </div>
    <div class="ultra" class="zoom-img" width: 300px;>
      <h1><a href="https://brawlstars.fandom.com/wiki/Sirius">西里烏斯</a></h1>
      <p>
      稀有度：<br>
      超凡<br>
      職業：<br>
      控場<br>
      移動速度：<br>
      720（普通）<br>
      864（裝備極限威能）</p>
    </div>
  </div>
  <p class="go" id="new">全新角色!</p>
  <p style="padding-left: 20px;">英雄種類：輸出者、坦克、刺客、狙擊手、控場者、輔助、投擲者。</p>
  <p style="padding-left: 20px;">我們現在2026年11月~2027年1月的最新英雄有3個!:thunderfrogs (雷蛙)，雷 (Rey)與露比 (Ruby)</p>
  <div style="text-align: center;">
    <img class="zoom-img" src="Thunderfrogs.webp" style="width:50%; height:50%;">
  </div>
  <p class="go" id="nb">全新更新!</p>
  <p style="padding-left: 20px;">每個賽季都有特別的遊戲主畫面與活動!2026的更新如下:</p>
  <h1>全新排位賽!</h1>
  <p style="padding-left: 20px;">最近荒野亂鬥更新了排位賽，讓排位賽變得更刺激!</p>
  <img class="zoom-img-99" src="new-brawler-selection-screen-v0-7po01kme2cmh1.webp" style="width:50%; height:50%;">  
  <p style="padding-left: 20px;">大家一起來下載brawlstars吧!</p>
  <p style="padding-left: 20px;">下載網址: <a href="https://play.google.com/store/apps/details?id=com.supercell.brawlstars&hl=zh_TW">點我前往 Google Play 下載</a></p>
  <p id="more" style="padding-left: 20px;"><b>Pictures from:</b> frantkit.com, google</p>

  <div class="first">
    <div id="search" class="chat-section">
      <div id="display">在這裡輸入問題，我會回答你...</div>
      <input type="text" id="userInput" placeholder="例如：你好 / 這個網站在介紹什麼？">
      <button onclick="respond()">送出</button>
    </div>

    <form action="" style="text-align: center; margin-bottom: 20px;">
      <label for="lan" style="color: white;">choose a language:</label>
      <select id="lan" name="lan" style="font-size: 20px; padding: 5px;">
        <option value="chinese">chinese</option>
        <option value="english">english</option>
        <option value="japanese">japanese</option>
        <option value="chinese(china)">chinese(china)</option>
      </select>
    </form>
  </div>

  <script>
    document.getElementById('userInput').addEventListener('keypress', function (e) {
      if (e.key === 'Enter') {
        respond();
      }
    });

    function respond() {
      const input = document.getElementById('userInput').value;
      const display = document.getElementById('display');
      const language = document.getElementById('lan').value;

      if (input.trim() ==="") return; 
      if (language === "chinese")
        if (input.includes("你好")) {
          display.innerText = "你好！很高興見到你。";
        } 
        else if (input.includes("這些圖片從哪裡來")) {
          display.innerText = "從 google 和 frant.kit 網站來。";
        } 
        else if (input.includes("這個網站在介紹什麼")) {
          display.innerText = "本站正在介紹：荒野亂鬥 (Brawl Stars)";
        }
        else {
          display.innerText = '我不知道您在說些什麼？？？？？？';
        }
      if (language === "english")
        if (input.includes("hello")) {
          display.innerText = "hello!very nice to meet you!";
        } 
        else if (input.includes("were are those pictures from")) {
         display.innerText = "they are from google and frant.kit";
        } 
        else if (input.includes("what is this website talking about")) {
          display.innerText = "this website is talking about brawl stars.";
        }
        else {
          display.innerText = 'I dont no what are you saying？？？？？？';
        }
      if (language === "japanese")
        if (input.includes("こんにちは")) {
         display.innerText = "こんにちは！お会いできて光栄です。";
        } 
        else if (input.includes("これらの写真はどこから来たのですか？")) {
          display.innerText = "Googleとfrant.kitのウェブサイトより。";
        } 
        else if (input.includes("このウェブサイトは何を紹介しているのですか？")) {
          display.innerText = "このサイトではブロスタを紹介しています。";
        }
        else {
          display.innerText = "何の話をしているのか分かりません??????";
        }
      if(language === "chinese(china)")
        if (input.includes("你好")) {
          display.innerText = "你好！很高寻见到你。";
        }
        else if (input.includes("these图片从哪里来")) {
          display.innerText = "从 google 和 frant.kit 网站来。";
        }
        else if (input.includes("这个网站在介绍什么")) {
          display.innerText = "本站正在介绍：荒野乱斗 (Brawl Stars)";
        }
        else {
          display.innerText = "我不明白你在说什么??????";
        }
      document.getElementById('userInput').value = "";
      document.getElementById('userInput').focus();
    }
  </script>

  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>

  <script>
    var heroSwiper = new Swiper(".heroSwiper", {
      loop: true,             
      speed: 800,             
      autoplay: {
        delay: 3500,          
        disableOnInteraction: false,
      },
      pagination: {
        el: ".swiper-pagination",
        clickable: true,
      },
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
      },
    });
  </script>

  <footer>
    <p class="one">本版本有著作權；請勿冒仿!!!</p>
    <p class="one">本版本網址:file:///Q:/%E6%88%91%E7%9A%84%E9%9B%B2%E7%AB%AF%E7%A1%AC%E7%A2%9F/Students/ryderwang/brawlstarsweb.html</p>
    <p class="one">本網站適用於教學</p>
    <p class="one">網站製作人:王懷謙</p>
  </footer>
</body>
</html>
