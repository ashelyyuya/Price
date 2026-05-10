<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>美業資訊頁</title>

<style>
body{
    margin:0;
    font-family:"Noto Sans TC",sans-serif;
    background:#f7f2ec;
    color:#6b5d52;
}

/* Header */

.header{
    text-align:center;
    padding:40px 20px 20px;
}

.header h1{
    font-size:34px;
    margin-bottom:10px;
    letter-spacing:2px;
    color:#8c7768;
}

.header p{
    color:#9d8d80;
}

/* Tabs */

.tabs{
    display:flex;
    justify-content:center;
    gap:12px;
    flex-wrap:wrap;
    margin-bottom:30px;
}

.tab-btn{
    border:none;
    background:#e7d9cc;
    color:#6b5d52;
    padding:12px 24px;
    border-radius:999px;
    cursor:pointer;
    transition:0.3s;
}

.tab-btn.active{
    background:#cdb7a4;
    color:white;
}

/* Page */

.page{
    display:none;
    max-width:960px;
    margin:auto;
    padding:0 20px 40px;
}

.page.active{
    display:block;
}

/* Card */

.card{
    background:#fffaf5;
    border-radius:22px;
    padding:24px;
    margin-bottom:22px;
    box-shadow:0 4px 14px rgba(0,0,0,0.05);
}

.card h2{
    margin-top:0;
    color:#8a7260;
    border-bottom:1px solid #eadfd5;
    padding-bottom:10px;
}

/* Item */

.item{
    display:flex;
    justify-content:space-between;
    padding:10px 0;
    border-bottom:1px dashed #eadfd5;
    gap:20px;
}

.item:last-child{
    border-bottom:none;
}

/* Service */

.service-list{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
    gap:16px;
}

.service-box{
    background:#f4ebe3;
    border-radius:18px;
    padding:18px;
    text-align:center;
}

/* Notice */

.notice{
    line-height:1.9;
}

/* Footer Buttons */

.footer-buttons{
    display:flex;
    justify-content:center;
    gap:16px;
    flex-wrap:wrap;
    margin-top:40px;
}

.footer-buttons a{
    text-decoration:none;
    background:#d8c4b2;
    color:white;
    padding:12px 22px;
    border-radius:999px;
}

/* Mobile */

@media(max-width:600px){
    .item{
        font-size:14px;
    }

    .header h1{
        font-size:28px;
    }
}
</style>
</head>

<body>

<!-- Header -->

<div class="header">
    <h1>Beauty Studio</h1>
    <p>手部美甲 / 足部美甲 / 手足深層保養 / 熱蠟除毛 / 睫毛管理</p>
</div>

<!-- Tabs -->

<div class="tabs">
    <button class="tab-btn active" onclick="openTab('home',this)">首頁</button>
    <button class="tab-btn" onclick="openTab('price',this)">價目表</button>
    <button class="tab-btn" onclick="openTab('notice',this)">預約須知</button>
</div>

<!-- Home -->

<div id="home" class="page active">

    <div class="card">
        <h2>經營項目</h2>

        <div class="service-list">
            <div class="service-box">手部美甲</div>
            <div class="service-box">足部美甲</div>
            <div class="service-box">手足深層保養</div>
            <div class="service-box">熱蠟除毛</div>
            <div class="service-box">睫毛管理</div>
        </div>
    </div>

    <div class="footer-buttons">
        <a href="#home">返回首頁</a>
        <a href="#">IG</a>
        <a href="#">我要預約</a>
    </div>

</div>

<!-- Price -->

<div id="price" class="page">

    <div class="card">
        <h2>手部凝膠</h2>

        <div class="item">
            <span>單色（可跳一色）</span>
            <span>1100</span>
        </div>

        <div class="item">
            <span>貓眼</span>
            <span>1300</span>
        </div>

        <div class="item">
            <span>法式 / 鏡面</span>
            <span>1400</span>
        </div>

        <div class="item">
            <span>造型款式</span>
            <span>1300起</span>
        </div>
    </div>

    <div class="card">
        <h2>足部凝膠</h2>

        <div class="item">
            <span>單色（可跳一色）</span>
            <span>1300</span>
        </div>

        <div class="item">
            <span>貓眼</span>
            <span>1500</span>
        </div>

        <div class="item">
            <span>法式 / 鏡面</span>
            <span>1500</span>
        </div>

        <div class="item">
            <span>造型款式</span>
            <span>1500起</span>
        </div>
    </div>

    <div class="card">
        <h2>卸甲項目</h2>

        <div class="item">
            <span>本店卸甲續作</span>
            <span>200</span>
        </div>

        <div class="item">
            <span>他店卸甲續作</span>
            <span>300</span>
        </div>

        <div class="item">
            <span>純卸甲不續作</span>
            <span>600</span>
        </div>
    </div>

    <div class="card">
        <h2>深層保養</h2>

        <div class="item">
            <span>足部超值豪華組合（含保養及上色）</span>
            <span>2200</span>
        </div>

        <div class="item">
            <span>足部基礎升級保養</span>
            <span>1580</span>
        </div>

        <div class="item">
            <span>足部深層美白保養</span>
            <span>2080</span>
        </div>

        <div class="item">
            <span>足部抗齡煥膚保養</span>
            <span>2280</span>
        </div>

        <div class="item">
            <span>手部基礎升級保養</span>
            <span>880</span>
        </div>

        <div class="item">
            <span>手部深層美白保養</span>
            <span>1480</span>
        </div>
    </div>

    <div class="card">
        <h2>睫毛管理</h2>

        <div class="item">
            <span>上睫毛</span>
            <span>1280</span>
        </div>

        <div class="item">
            <span>野生眉</span>
            <span>1080</span>
        </div>
    </div>

    <div class="card">
        <h2>熱蠟除毛</h2>

        <div class="item"><span>VIO+腋下組合</span><span>1850</span></div>
        <div class="item"><span>全腿+全臂組合</span><span>2500</span></div>
        <div class="item"><span>VIO+小腿組合</span><span>2500</span></div>
        <div class="item"><span>VIO全除</span><span>1600</span></div>
        <div class="item"><span>V區</span><span>1000</span></div>
        <div class="item"><span>I區</span><span>800</span></div>
        <div class="item"><span>O區</span><span>800</span></div>
        <div class="item"><span>比基尼線</span><span>800</span></div>
        <div class="item"><span>腹部</span><span>1000</span></div>
        <div class="item"><span>全背</span><span>1200</span></div>
        <div class="item"><span>腋下</span><span>500</span></div>
        <div class="item"><span>手指手背</span><span>300</span></div>
        <div class="item"><span>前臂</span><span>900</span></div>
        <div class="item"><span>全臂</span><span>1300</span></div>
        <div class="item"><span>腳趾腳背</span><span>300</span></div>
        <div class="item"><span>小腿</span><span>1200</span></div>
        <div class="item"><span>全腿</span><span>1600</span></div>
        <div class="item"><span>小鬍子</span><span>300</span></div>
    </div>

</div>

<!-- Notice -->

<div id="notice" class="page">

    <div class="card notice">
        <h2>美甲</h2>

        ▫️需保留3小時施作時間，切勿趕時間。<br>
        ▫️依皮膚狀況與款式不同可能提早或延後。<br>
        ▫️指甲建議預留0.2-0.3公分。<br>
        ▫️皮膚疾病、病甲不接受預約。<br>
        ▫️不接待同行、不接延甲。
    </div>

    <div class="card notice">
        <h2>睫毛管理</h2>

        ▫️無卸除嫁接睫毛服務。
    </div>

    <div class="card notice">
        <h2>熱蠟除毛</h2>

        ▫️請於Line回覆預約表格。<br>
        ▫️請勿自行刮除毛髮，至少需預留0.5公分。
    </div>

    <div class="card notice">
        <h2>共同須知</h2>

        ▪️預約保留10分鐘。<br>
        ▪️超過時間本店有權取消或調整施作項目。<br>
        ▪️更改時間或取消請提前3日以上Line告知。<br>
        ▪️不得攜伴。<br>
        ▪️禁止吃東西，可以喝飲料或喝水。<br>
        ▪️只收現金或Line Pay。
    </div>

</div>

<script>
function openTab(tabId, btn){

    const pages = document.querySelectorAll('.page');
    const buttons = document.querySelectorAll('.tab-btn');

    pages.forEach(page=>{
        page.classList.remove('active');
    });

    buttons.forEach(button=>{
        button.classList.remove('active');
    });

    document.getElementById(tabId).classList.add('active');
    btn.classList.add('active');
}
</script>

</body>
</html>
