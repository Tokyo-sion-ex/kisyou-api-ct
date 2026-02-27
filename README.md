# kisyou-api-ct
気象庁APIを使用した気象情報を提供するChannel Talk用のBOTです。

# 構成
## ver.1-0-0-β
**2026/2/27 公開**
新規で作成。デバッグは実施中。
```both
project/
├── index.js                 # エントリポイント（サーバ起動、cron登録）
├── config.js                # 環境変数・定数（Channel Talkトークン、ルームIDなど）
├── prefectures.json         # 都道府県名 → 気象庁コードのマッピング
├── weatherFetcher.js        # 気象庁APIからデータ取得・整形
├── channelTalkClient.js     # Channel Talk API呼び出し（メッセージ送信）
├── messageHandler.js        # デバッグコマンドのパース・実行
└── scheduler.js             # cronスケジュール設定
```
