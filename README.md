# Felix Team App Specs

フェリックス共同開発アプリの画面仕様書・機能仕様書・各種設計書を管理するリポジトリ。

公開URL: <https://kotaroblog.github.io/app-specs-felix/>

関連リポジトリ: [app-specs-personal](https://github.com/kotaroblog/app-specs-personal)（個人開発）

## 対象アプリ

- RankingStadium（ランスタ）
- DailyTips（デイリー日めくり）

## ディレクトリ構成

```
app-specs-felix/
├── index.html              # ポータル
├── assets/css/style.css    # 共通スタイル
├── _template/              # 仕様書テンプレ集（個人側と同期）
├── rankingstadium/
└── dailytips/
```

各アプリは以下の構成：
```
[アプリ名]/
├── index.html        # アプリトップ（画面一覧）
├── flow.html         # 画面遷移図
├── data-model.html   # データモデル
├── error-design.html # エラー設計
├── logging.html      # ロギング方針
├── aso.html          # ASOキーワード戦略
├── glossary.html     # 用語集
├── screens/          # 画面ごとの仕様書
└── features/         # 機能仕様書
```

## 仕様書を追加する手順

1. `_template/` から該当テンプレをコピー
2. 配置先パスへ保存
3. アプリの `index.html` のカードリストに追加
4. `git push` → GitHub Pagesに自動反映（30秒〜2分）

## 注意事項

- 検索エンジン除外: 全ページに `<meta name="robots" content="noindex, nofollow">` 設定
- 認証なし（URL を知っている人なら閲覧可）
- **機密情報を書かない**: APIキー、課金実装の内部ロジック詳細、サーバー認証フロー詳細、契約書情報
