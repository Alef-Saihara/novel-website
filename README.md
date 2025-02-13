<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NIT - ホーム</title>
    <link rel="stylesheet" href="styles.css">
    <script>
        function loadAuthorNames() {
            for (let i = 1; i <= 13; i++) {
                let savedAuthorName = localStorage.getItem('homeAuthorName' + i);
                if (savedAuthorName) {
                    document.getElementById('author-name-display-' + i).innerText = savedAuthorName;
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #1A1A1A;
            color: #E0E0E0;
            font-family: 'Noto Sans JP', sans-serif;
            text-align: center;
        }
        .content-box {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
            max-width: 800px;
            margin: 40px auto;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.3);
            text-align: left;
        }
        .author-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .author-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 8px;
            cursor: pointer;
            transition: background 0.3s;
        }
        .author-item:hover {
            background: rgba(255, 255, 255, 0.2);
        }
    </style>
</head>
<body onload="loadAuthorNames()">
    <header>
        <h1>NIT 作家一覧</h1>
        <nav>
            <ul>
                <li><a href="index.html">ホーム</a></li>
                <li><a href="edit/edit.html">編集(作者のみ)</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section class="content-box">
            <h2>NITとは？</h2>
            <p>
                2024年3月12日に開設した小説チームです。Discordを活用し、作家同士の交流だけでなく、読者も参加し、
                より良い小説を作り上げることを目的としています。
            </p>
            <h3>NITの参加条件</h3>
            <p>
                まずは書き手・読み手のどちらも参加可能なDiscord鯖、<br>
                <a href="https://discord.com/invite/KCBVYQvE">NITオープンチャット</a>
                に参加していただきます。
            </p>
            <h3>参加後の活動</h3>
            <p>
                特に制限はなく、大きな活動予定もありません。気軽に参加してください。
            </p>
        </section>
        
        <section class="content-box">
            <h2>所属作家一覧</h2>
            <div class="author-list">
                <div class="author-item" onclick="location.href='edit_author1.html'">
                    <p id="author-name-display-1">作家1</p>
                </div>
                <div class="author-item" onclick="location.href='edit_author2.html'">
                    <p id="author-name-display-2">作家2</p>
                </div>
                <div class="author-item" onclick="location.href='edit_author3.html'">
                    <p id="author-name-display-3">作家3</p>
                </div>
                <div class="author-item" onclick="location.href='edit_author4.html'">
                    <p id="author-name-display-4">作家4</p>
                </div>
                <div class="author-item" onclick="location.href='edit_author5.html'">
                    <p id="author-name-display-5">作家5</p>
                </div>
                <div class="author-item" onclick="location.href='edit_author6.html'">
                    <p id="author-name-display-6">作家6</p>
                </div>
            </div>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2025 NIT All Rights Reserved.</p>
    </footer>
</body>
</html>
