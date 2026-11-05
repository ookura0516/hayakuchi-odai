# hayakuchi-odai

ハヤクチ道場（iOS / Android）の「今日の1文」のお題データ。

- `odai.json` をアプリが jsDelivr から1日1回取得する:
  `https://cdn.jsdelivr.net/gh/ookura0516/hayakuchi-odai@main/odai.json`
- お題はすべてこのアプリのための自作（ookura, 2026-11）。本やサイトの早口言葉集からは写していない。
- `schedule[n]` が `start`（2026-11-02・月曜）から n 日目のお題。lv は曜日の難しさ（1=月 短い 〜 7=日 長い）。
- アプリは先頭63日分を同梱している。**`start` と、先頭63日の並びは変えないこと**（変えるとアプリは配信分を採らず同梱分のまま動く）。足すときは `schedule` の末尾に7日単位で追加する。
- 生成元: アプリのリポジトリの `tools/odai/odai_src.txt` → `python3 tools/odai/build_odai.py`。

## 中身（2026-11-05）
- 147文（暦に載る126文＝18週・2026-11-02〜2027-03-07、難問パック21文）
- 暦の外の日付では、アプリは曜日が合うように7の倍数で回して使う
