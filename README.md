# parametric-speaker-case-model

Coding by Gemini 3.1 Pro

## 概要
秋月電子のパラメトリックスピーカー実験キット（ https://akizukidenshi.com/catalog/g/g102617/ ）向けの保護ケースを生成するためのブラウザベースの設計アプリケーションです。ユーザが寸法や端子位置などのパラメータを調整して、ケース本体と蓋のSTLファイルを出力できます。

## 使用技術
- 言語: HTML, JavaScript
- ライブラリ/フレームワーク: Three.js（OrbitControls, STLExporter, BufferGeometryUtils 等）
- データベース: なし
- その他: ブラウザで完結（CDN経由でThree.jsを読み込み）

## 使い方
### 前提条件
- WebGL 対応のブラウザ（Chrome, Edge, Firefox など）

### インストール方法
```bash
git clone https://github.com/yourname/parametric-speaker-case-model.git
cd parametric-speaker-case-model
```

### 基本的な使い方
- レポジトリ内の `ControlBoard/index.html` または `SpeakerBody/index.html` をブラウザで開いてください。
- UI上でケース内寸、壁厚、蓋クリアランス、ジャック穴位置やサイズなどを調整します。
- 「ベースを保存」や「蓋を保存」などのボタンを押して、STLファイルをダウンロードしてください。

## 主な機能
- ケース本体（ベース）のパラメトリック生成
- 蓋（リップ形状含む）の生成とクリアランス調整
- DCジャック、Audioジャック、ワイヤー穴などの位置・サイズ調整
- スタンドオフ（スペーサ）やダミー部品のプレビュー表示
- ケース本体 / 蓋 を個別にSTLでエクスポート

## 設定
- 特別な設定ファイルや環境変数は不要です。すべてのパラメータはブラウザ上のUIで変更できます。

## APIリファレンス / ドキュメント
- 実装は主に `ControlBoard/index.html` と `SpeakerBody/index.html` 内のインラインスクリプトにあります。これらのファイルを参照してください。
