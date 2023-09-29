# 「PythonとScrapyを使ったWebスクレイピング」 川原英明 著

2023/9/29 ~ 9/29  

## 環境構築

- scrapy フレームワーク
- Python

仮想環境の構築  
```mkdir -p scrapy-source```
```python -m venv .venv```

仮想環境へ切替(PowerShell)  
cdをscrapy-sourceフォルダに切り替えて、  
```.venv\Scripts\activate.ps1```

Scrapy フレームワークのインストール  
```python -m pip install --upgrade pip```
```pip install scrapy```

Dockerの準備  

## スクレイピング

ヤフーニュースのビジネスページをスクレイピング

Scrapyの構成  

- Spider の作成
- Item の設定
- Scrapy の設定
- Pipeline の設定(設定しないときもある)

プロジェクトの作成  
```scrapy startproject yahoo_news_scrapy```

Spider のひな形の作成  
プロジェクトディレクトリに移り、  
```scrapy genspider yahoo_news news.yahoo.co.jp```

アイテム設定  
items.pyの編集  

Scrapy の設定  
settings.py の編集  

- DOWNLOAD_DELAY = 3 のコメントアウト解除
- キャッシュの設定 HTTPCACHE＿～のコメントアウト解除

Spider 作成  
yahoo_news.py の編集  

クローラーの実行  

## POST メソッドがあるサイトでのスクレイピング

## データベースを使用してのスクレイピング

## 動的画面のスクレイピング

## Lazy loading 画面のスクレイピング

## Dropbox と連携する
