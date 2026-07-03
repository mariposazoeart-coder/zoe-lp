---
title: Testimonials ボード
tags: [feedback, board]
---

# ⭐ LP/SNS 転用ボード

LP・SNS に使える「掲載OK」のお客様の声を集約します。

> **公開前チェック**：ここに出てくるのは `testimonial: true` かつ `permission: "ok"` のものだけ。
> 未許可の声は次のセクションで洗い出し、公開前に必ず許可を取ること。

## ✅ 掲載OK（LP/SNS で使える声）

> Dataview プラグインが有効な場合、下のクエリで自動一覧になります。

```dataview
TABLE customer AS "顧客", service AS "サービス", sentiment AS "感情", themes AS "テーマ", date AS "日付"
FROM "20_Knowledge/Feedback"
WHERE testimonial = true AND permission = "ok"
SORT date DESC
```

## ⏳ 掲載候補だが未許可（公開前に許可確認）

```dataview
TABLE customer AS "顧客", permission AS "許可", date AS "日付"
FROM "20_Knowledge/Feedback"
WHERE testimonial = true AND permission != "ok"
SORT date DESC
```

---

### Dataview を入れていない場合

上のクエリはただの表示になり、自動では動きません。その場合は、
- `/feedback-find` を使って「掲載OKの声」を抽出してもらう、または
- このファイルに手動でOKの声を追記していってください。

#### 手動リスト（掲載OKの声）
- 
