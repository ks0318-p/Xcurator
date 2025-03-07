
## 推奨アーキテクチャ: NestJS + Dify + NextJS

```
[NestJS バックエンド] ⟷ [Dify API] ⟷ [Coze API] ⟷ [Dify 送信文の作成] → [NestJS Discord/Slackへの送信]

[NextJS フロントエンド] ←→ [NestJS バックエンド]
```

### コンポーネント詳細

1. **NestJS バックエンド**
   - TypeScriptの型安全性や依存性注入などの強力な機能を活用
   - API化されたDifyを呼び出す
   - スケジュール実行や定期実行を管理
   - Discord/SlackのWebhookを使用したメッセージ送信を担当

2. **Dify API**
   - AI機能の統合
   - Coze APIと連携し、送信文の作成を担当
   - ローカルで構築する

3. **Coze API**
   - X APIへのアクセス、データ収集、ルール処理を担当
   - API化して、Difyから呼び出す

4. **NextJS フロントエンド**
   - ユーザー用設定画面のみを提供
   - ルールの設定、管理、結果確認用のUI

5. **Supabase**
   - 認証基盤として使用
   - データベースとして使用
   - ルール設定や収集したデータの保存

6. **Vercel**
   - デプロイメントとホスティング

