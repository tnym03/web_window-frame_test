<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RPA マクロマン フレーム切り替えテスト（更新版）</title>
    <style>
        body {
            font-family: sans-serif;
            margin: 20px;
            background-color: #f0f0f0;
        }
        h1 {
            color: #333;
        }
        .main-content {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        iframe {
            border: 2px solid #007bff;
            width: 100%;
            height: 250px; /* 高さを少し増やしました */
            margin-top: 20px;
            background-color: #e6f2ff;
        }
        .iframe-content {
            padding: 15px;
            color: #0056b3;
        }
        .iframe-button {
            padding: 10px 15px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
            margin-right: 10px; /* ボタン間のスペース */
        }
        .iframe-button:hover {
            background-color: #218838;
        }
        .iframe-inner-button { /* 新しいボタンのスタイル */
            padding: 8px 12px;
            background-color: #ff5722; /* オレンジ系の色 */
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
        }
        .iframe-inner-button:hover {
            background-color: #e64a19;
        }
    </style>
</head>
<body>
    <h1>RPA マクロマン フレーム切り替えテストサイト（更新版）</h1>

    <div class="main-content">
        <p>ここはメインフレームのコンテンツです。以下のiframeに切り替えてテストしてください。</p>
        <button onclick="alert('メインフレームのボタンがクリックされました！')">メインフレームのボタン</button>
    </div>

    <h2>テスト用 iframe</h2>
    <p>このiframeの中に別のコンテンツがあります。</p>

    <iframe id="myFrame" name="myTestFrame">
        <!DOCTYPE html>
        <html lang="ja">
        <head>
            <style>
                body {
                    font-family: sans-serif;
                    margin: 10px;
                    background-color: #e6f2ff;
                }
                p {
                    color: #0056b3;
                }
                button {
                    padding: 8px 12px;
                    background-color: #ffc107;
                    color: #333;
                    border: none;
                    border-radius: 4px;
                    cursor: pointer;
                    margin-right: 8px; /* iframe内ボタン間のスペース */
                }
                button:hover {
                    background-color: #e0a800;
                }
                .input-field {
                    margin-top: 10px;
                    padding: 8px;
                    border: 1px solid #ccc;
                    border-radius: 4px;
                }
            </style>
        </head>
        <body>
            <div class="iframe-content">
                <h3>iframe内のコンテンツ</h3>
                <p>このテキストはiframeの中にあります。</p>
                <button class="iframe-button" onclick="alert('iframe内の「基本ボタン」がクリックされました！')">iframe内の基本ボタン</button>
                <button class="iframe-inner-button" onclick="alert('iframe内の「追加ボタン」がクリックされました！')">iframe内の追加ボタン</button>
                <p>iframe内の別のテキストです。</p>
                <input type="text"
