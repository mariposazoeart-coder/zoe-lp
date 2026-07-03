# 20_Knowledge — 目次（MOC: Map of Content）

この知識ベースの入口です。ここから各ボード・フォルダへ辿れます。

## 全体の流れ

```
投げ込む            整理する               活用する
00_Inbox/  ──▶  20_Knowledge/Feedback/  ──▶  _Testimonials.md（LP/SNS転用）
                20_Knowledge/Notes/          _Trends.md（傾向・改善）
```

1. **Inbox**：お客様の声・文字起こし・メモを、まず `00_Inbox/` に投げ込む
2. **整理**：`/feedback-sort` や「Inbox整理して」で、1感想=1ノートにして `Feedback/{顧客名}/` へ振り分け（移動前に確認）
3. **活用**：`/feedback-find` や各ボードで、LP用の声・顧客履歴・傾向/改善点を抽出

## フォルダ構成

| 場所 | 役割 |
|---|---|
| [00_Inbox](../00_Inbox/README.md) | 未整理の投げ込み先。何でもOK |
| [Feedback](Feedback/) | お客様の声。`Feedback/{顧客名}/` に 1感想=1ノート |
| [Notes](Notes/) | 気づき・アイデア・参考メモ |
| [_templates](_templates/) | ノート雛形（feedback / note / transcript） |

## 活用ボード

- [[_Testimonials]] … LP/SNS転用ボード（掲載OKの声を集約）
- [[_Trends]] … 傾向・改善分析ボード（sentiment / themes 集計）

## 掲載許可の注意（重要）

- お客様の声を **公開（LP/SNS）に使う前に `permission` を必ず確認** すること。
- 明記が無い声は `permission: unknown`。**勝手に `ok` にしない**。
- `_Testimonials.md` に載るのは `testimonial: true` かつ `permission: ok` のものだけ。
