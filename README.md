# GEMS Web App

GEMS v9.9.2 Scriptable版を、通常のWebブラウザで動作する構成に変換したものです。

## 構成
- index.html : 画面
- style.css  : 既存UIのCSS
- app.js     : 既存GEMSロジック + Web版互換レイヤー

## 起動
ローカルファイルを直接開くより、HTTPサーバー経由を推奨します。

例:
python -m http.server 8000
→ http://localhost:8000/

## Web版で保持している主な機能
現場・遠征・分析・設定・テーマ変更・データ保存・CSV/JSON出力・JSON復元・画像追加・画像回転・画像トリミング・フィードバック記録など。

## 保存
データはブラウザのlocalStorage、画像はブラウザのlocalStorage内のWeb用メディア領域に保存します。

## Scriptable固有機能について
Yahoo!距離自動取得、MusicBrainz/X等の外部連携、iOS固有の共有・GEMS SCANなどはWeb環境では同一APIがないため代替動作/無効化しています。
