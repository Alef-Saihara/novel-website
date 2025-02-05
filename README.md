<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>宰原アレフ - 作品一覧</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@700&family=Noto+Sans+JP:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            background-color: #1A1A1A;
            color: #E0E0E0;
            font-family: 'Noto Sans JP', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px 30px;
            background: #252525;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.3);
        }
        .logo {
            font-family: 'Cinzel', serif;
            font-size: 40px;
            color: #C0A060;
        }
        .site-title {
            font-size: 24px;
            font-weight: bold;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            gap: 15px;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            text-decoration: none;
            color: #E0E0E0;
            font-weight: bold;
            transition: color 0.3s, background 0.3s;
            padding: 8px 12px;
            border-radius: 5px;
        }
        nav ul li a:hover {
            color: #1A1A1A;
            background: #C0A060;
        }
        main {
            padding: 40px 20px;
        }
        .works-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .work-item, .worldline-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
            transition: transform 0.3s, background 0.3s;
            cursor: pointer;
            position: relative;
        }
        .work-item:hover, .worldline-item:hover {
            transform: scale(1.05);
            background: rgba(255, 255, 255, 0.2);
        }
        .worldline-list {
            display: none;
            position: absolute;
            top: 100%;
            left: 50%;
            transform: translateX(-50%);
            background: #2C2C2C;
            padding: 10px;
            border-radius: 8px;
            width: 200px;
        }
        .worldline-item:hover .worldline-list {
            display: block;
        }
        .worldline-list p {
            padding: 5px;
            cursor: pointer;
        }
        .worldline-list p:hover {
            background: #C0A060;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">ℵ</div>
        <h1 class="site-title">宰原アレフ</h1>
        <nav>
            <ul>
                <li><a href="#">ホーム</a></li>
                <li><a href="#works">作品一覧</a></li>
                <li><a href="#worldlines">世界線</a></li>
                <li><a href="#profile">プロフィール</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section id="works">
            <h2>作品一覧</h2>
            <div class="works-container">
                <div class="work-item" onclick="location.href='workA.html'">作品A</div>
                <div class="work-item" onclick="location.href='workB.html'">作品B</div>
                <div class="work-item" onclick="location.href='workC.html'">作品C</div>
                <div class="work-item" onclick="location.href='workD.html'">作品D</div>
                <div class="worldline-item" onclick="location.href='worldline1.html'">世界線1
                    <div class="worldline-list">
                        <p onclick="location.href='workA.html'">作品A</p>
                        <p onclick="location.href='workB.html'">作品B</p>
                    </div>
                </div>
                <div class="worldline-item" onclick="location.href='worldline2.html'">世界線2
                    <div class="worldline-list">
                        <p onclick="location.href='workC.html'">作品C</p>
                        <p onclick="location.href='workD.html'">作品D</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2025 宰原アレフ All Rights Reserved.</p>
    </footer>
</body>
</html>
