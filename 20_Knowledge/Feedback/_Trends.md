---
title: Trends ボード
tags: [feedback, board]
---

# 📊 傾向・改善分析ボード

お客様の声を横断して、良い傾向と改善点を掴むためのボードです。

## 感情（sentiment）別の集計

```dataview
TABLE length(rows) AS "件数"
FROM "20_Knowledge/Feedback"
WHERE sentiment
GROUP BY sentiment AS "感情"
SORT length(rows) DESC
```

## 改善のヒント（negative の抽出）

```dataview
TABLE customer AS "顧客", themes AS "テーマ", date AS "日付", file.link AS "ノート"
FROM "20_Knowledge/Feedback"
WHERE sentiment = "negative"
SORT date DESC
```

## テーマ（themes）別の集計

```dataview
TABLE length(rows) AS "件数"
FROM "20_Knowledge/Feedback"
WHERE themes
FLATTEN themes AS theme
GROUP BY theme AS "テーマ"
SORT length(rows) DESC
```

---

### Dataview を入れていない場合

上のクエリは自動では動きません。その場合は `/feedback-find` に
「傾向を出して」「改善点をまとめて」と頼めば、ノートを横断して集計・抽出します。
