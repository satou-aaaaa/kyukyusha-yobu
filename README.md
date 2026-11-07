# 救急車よぶ？

具合の悪い場面（顔の片方がゆがむ・突然の激しい頭痛・胸の締め付け・のどにつまる・迷ったとき など）から、すぐ119番か・救急相談（#7119など）か・子どもの相談（#8000）か・救急車の出番ではないかを当て、119番のかけ方も覚える学習ゲーム。だれでも同じ1日5問。

- 遊ぶ: <https://satou-aaaaa.github.io/kyukyusha-yobu/>
- 場面が出ます。札（すぐ119番・救急相談・子どもの相談・救急車の出番ではない など）から1つ選びます。
- 正しく選ぶと「なぜそうなるか」と消防庁の資料の名前・出典が出て、救急帳に集まります（8種類）。
- ★はまちがい＋ヒントの数で決まります（0で★3）。時間の制限はありません。
- 今日の5問と上級（3問・ヒントなし・札4枚）は1日1回。とことんは何度でも、「ここでやめる」まで続きます。遊べなかった日は7日前まで、カレンダーから「あとから」遊べます。
- 答えと説明は、総務省消防庁の次の資料に沿っています（2026年11月に確かめた内容）。
  - 救急車利用リーフレット（成人版・高齢者版）「ためらわず救急車を呼んでほしい症状」<https://www.fdma.go.jp/publication/portal/items/portal009_seijim.pdf>・<https://www.fdma.go.jp/publication/portal/items/portal009_kourei.pdf>
  - 救急車利用マニュアル「救急車を上手に使いましょう」<https://www.fdma.go.jp/publication/portal/items/portal002_japanese121.pdf>
  - 救急安心センター事業（#7119）<https://www.fdma.go.jp/mission/enrichment/appropriate/appropriate007.html>
  - 全国版救急受診アプリ（Q助）<https://www.fdma.go.jp/mission/enrichment/appropriate/appropriate003.html>
- #7119 は地域によって番号や受付の時間がちがい、まだ無い地域もあります。子ども（15歳未満）は #8000 の子ども医療電話相談です。
- 医療の相談ではなく、医療機器でもありません。本当に具合が悪いときは、迷わず119番に電話してください。
- 記録は遊ぶ人のブラウザにだけ残り、ゲームから自動で外へ送ることはありません。例外は2つ：文字（Google Fonts）を読み込むとき、Google に IP アドレスが届きます。「X」「LINE」「コピー」を押したときだけ、結果の四角が選んだ先に渡ります（答えは入りません）。

## 開発

```bash
bash scripts/setup.sh   # 最初に一度
node qa/run.mjs         # 検査（CI と同じ）
node tools/make-icons.cjs && node tools/make-og.cjs   # アイコンと SNS 用の絵を作り直すとき
```

感想は [Issue のフォーム](https://github.com/satou-aaaaa/kyukyusha-yobu/issues/new?template=feedback.yml) からどうぞ。
