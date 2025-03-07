# Xcurator 仕様書

## アプリの目的
このアプリはXでの情報収集効率の改善を目指しています。ユーザーはX上で収集できるルールを設定できます。例えば、bynameで人を指定したり、いいね数、リプライ数、リポスト数などの条件を指定して、特定の条件に合致する投稿のみを取得することができます。最終的には取得結果がDiscordやSlackのチャンネルに自動でポストされます。

## ページと機能
- @pages.md [[pages]]

##  Coze経由でのX APIの利用と制限
- @coze.md [[coze]]

## 出力先一覧
- Discord
- Slack

## アプリケーションタイプ
- ブラウザベースのウェブアプリ

## アーキテクチャ
- @Architecture.md [[Architecture]]

## 出力先への連携方法
- Webhook

## 出力形式
- @OutputFormat.md [[OutputFormat]]
