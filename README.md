<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NIT - ホーム</title>
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
        .site-title {
            font-size: 28px;
            font-weight: bold;
            color: #C0A060;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            gap: 20px;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            text-decoration: none;
            color: #E0E0E0;
            font-weight: bold;
            transition: color 0.3s, background 0.3s;
            padding: 10px 15px;
            border-radius: 5px;
        }
        nav ul li a:hover {
            color: #1A1A1A;
            background: #C0A060;
        }
        main {
            padding: 40px 20px;
        }
        .content-box {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
            max-width: 800px;
            margin: 0 auto;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.3);
            text-align: left;
        }
        .authors-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .author-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
            transition: transform 0.3s, background 0.3s;
            cursor: pointer;
            position: relative;
            width: 200px;
            text-align: center;
        }
        .author-item:hover {
            transform: scale(1.05);
            background: rgba(255, 255, 255, 0.2);
        }
    </style>
</head>
<body>
    <header>
        <h1 class="site-title">NIT</h1>
        <nav>
            <ul>
                <li><a href="#home">ホーム</a></li>
                <li><a href="#authors">所属小説家一覧</a></li>
                <li><a href="edit.html">編集(作者のみ)</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section id="home">
            <div class="content-box">
                <h2>NITについて</h2>
                <p>NITは2024年3月12日に設立された小説家チームです。Discordを活用し、作家同士の交流だけでなく、読者も参加し、より良い小説を作り上げることを目的としています。</p>
                <h3>参加条件</h3>
                <p>まずは読み手・書き手のどちらも参加可能なDiscordサーバー「NITオープンチャット」に参加してください。<br>
                <a href="https://discord.com/invite/KCBVYQvE">NITオープンチャットに参加する</a></p>
                <p>「NITに入りたい！」と申し出るか、近況ノートにコメントをいただければ、NITのDiscordの招待リンクを配布します。また、こちらからお誘いする場合もあります。</p>
                <p>ただし、NIT本体は書き手のみの参加が可能です。また、倫理観のない方の参加はご遠慮いただく場合があります。</p>
                <h3>活動について</h3>
                <p>特に強制的な活動はなく、自由にご参加いただけます。現時点では大きな活動予定もございませんので、気軽にご参加ください。</p>
                <p>ただし、NITの知名度向上のため、名前の最後に「@NIT所属」と付けていただけると助かります。</p>
            </div>
        </section>
        
        <section id="authors">
            <div class="content-box">
                <h2>所属小説家一覧</h2>
                <div class="authors-container">
                    <div class="author-item" onclick="location.href='author1.html'">作家1</div>
                    <div class="author-item" onclick="location.href='author2.html'">作家2</div>
                    <div class="author-item" onclick="location.href='author3.html'">作家3</div>
                    <div class="author-item" onclick="location.href='author4.html'">作家4</div>
                    <div class="author-item" onclick="location.href='author5.html'">作家5</div>
                    <div class="author-item" onclick="location.href='author6.html'">作家6</div>
                </div>
            </div>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2025 NIT All Rights Reserved.</p>
    </footer>
</body>
</html>
