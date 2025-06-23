# web_window-frame_test
ブラウザフレームを切り替え（要素指定）
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RPA マクロマン フレーム切り替えテスト</title>
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
            height: 200px;
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
        }
        .iframe-button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <h1>RPA マクロマン フレーム切り替えテストサイト</h1>

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
                }
                button:hover {
                    background-color: #e0a800;
                }
            </style>
        </head>
        <body>
            <div class="iframe-content">
                <h3>iframe内のコンテンツ</h3>
                <p>このテキストはiframeの中にあります。</p>
                <button class="iframe-button" onclick="alert('iframe内の
