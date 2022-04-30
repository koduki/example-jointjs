# joint.jsを使ってみる

## dockerの準備
dockerイメージを作成します。

```:bash
$ docker-compose build
```

## パッケージをインストールする
npmコマンドでインストールします。

```:bash
$ docker-compose run --rm node npm install
```

## デモページ
- graphモデル: ./src/demo/graph.html
- ORG-組織図: ./src/demo/org.html

## デモページを作ってみる
下記テンプレートを使ってdemoフォルダ内にhtmlファイルを作成する。

```:html
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="utf-8">
    <title>ページタイトル</title>

    <link rel="stylesheet" type="text/css" href="../node_modules/jointjs/dist/joint.min.css">
    <style type="text/css">
        h1, p, div { padding:0; margin:0; }
        h1 { font-size:14px; }
        #canpas { border:solid 1px #ccc; background-color: #eee; margin-top: 10px; }
    </style>
</head>
<body>
    <h1>サンプル</h1>
    <p>jointjsを動かしてみる！！</p>

    <div id="canpas"></div>
    <script src="../node_modules/jquery/dist/jquery.min.js"></script>
    <script src="../node_modules/lodash/lodash.min.js"></script>
    <script src="../node_modules/backbone/backbone-min.js"></script>
    <script src="../node_modules/jointjs/dist/joint.min.js"></script>
    <script>
        // ここに処理を記載する
    </script>
</body>
</html>
```

以上

## 参考サイト
- [jointjs.com](https://www.jointjs.com/opensource#Download-JointJS)
- [joint api](https://resources.jointjs.com/docs/jointjs/v3.1/joint.html)
