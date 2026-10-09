# 生成AIのコーディング技法

川原 純（京都大学）, 2026年10月9日

## スライド

- [slides_20261009.pdf](slides_20261009.pdf)

## 概要

コーディングエージェント（Claude Code, Codex など）を使って、自分用のソフトウェアを作ってみようという講演です。
3D テトリスを題材にコーディングエージェントによる開発の流れを紹介し、発表者がエージェンティックコーディングで作成したソフトウェアの例を、軽めのものから本格的な研究ソフトウェアまで紹介します。
最後に、生成 AI を使う上での注意点（ハルシネーション、PC の操作権限）を述べます。

## 講演で紹介したソフトウェア

| 作例 | 内容 | リンク |
|---|---|---|
| 3D テトリス | コーディングエージェントによる開発の実演例 | — |
| 作例1 | アドバイザー面談予約システム | — |
| 作例2 | 学生実験の学生証カードリーダーによる出席管理システム | — |
| 作例3 | 計算機科学実験及演習3（ハードウェア）: FPGA 上の CPU 実装とレポート | — |
| 作例4 | 講義「グラフ理論」のアルゴリズム可視化ツール | — |
| 作例5 | TikZ 形式で編集できるグラフ描画ツール | https://github.com/junkawahara/graph_svg |
| 作例6 | CoReViewer（組合せ遷移のソルバーと可視化ツール）の Web 移植 | https://github.com/junkawahara/coreviewer-web-test <br> （デスクトップ版: https://github.com/junkawahara/coreviewer） |
| 作例7 | トリプレット距離・カルテット距離を計算するアルゴリズム [Brodal et al., SODA 2013] の実装 | — |
| 作例8 | 75 種類超のグラフクラスの認識・列挙ライブラリ | https://github.com/junkawahara/ai-coded-graph-recognition-test |

## 講演で紹介したプロンプト

### コードのレビュー

```
リポジトリ内のコードやテスト、ドキュメントを徹底的に敵対的レビューして、見つかったバグは細かいものを含めて、すべて review_yyyyMMdd_X.md にリストアップしてください。yyyyMMdd は現在の年月日、X は連番です。ただし、 既存の KNOWN_ISSUES.md や review*.md （ファイルがもしあれば）にある項目は無視してください。各項目ごとに、連番、チェックボックス [ ]、重要性（重大・高・中・低） をつけてください。書式例は "1. [ ] 【低】" です。重要性でソートしてください（重大を先に並べて、次は高、その次は中）。
```

### 論文の参考文献のチェック

```
.bib に書かれた各文献が、出版社のページに存在するか調べて、情報が間違っていないかをチェックしてください。
```

## 参考文献・関連情報

- G. S. Brodal, R. Fagerberg, T. Mailund, C. N. S. Pedersen, and A. Sand.
  Efficient algorithms for computing the triplet and quartet distance between trees of arbitrary degree.
  In *Proceedings of the 24th Annual ACM-SIAM Symposium on Discrete Algorithms (SODA 2013)*, pages 1814–1832, 2013.
- 「AIで調べた沖縄戦の判例、存在せず　掲載本を回収・絶版に　琉球大・島袋純教授、高文研から刊行」（公開日: 2026年10月9日）
  https://www.okinawatimes.co.jp/articles/-/1941134
