# JsonlLens — 10GB超のJSONL・NDJSON・Parquetに対応した高速Windowsビューアー

**Languages:** [English](README.md) · 日本語 · [简体中文](README.zh-CN.md)

<p align="center">
  <a href="https://apps.microsoft.com/detail/9N9X7K90R64G">
    <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="260" alt="Microsoft Storeから入手" />
  </a>
</p>

<p align="center"><strong>大容量データを開き、検索し、確認し、SQLで調べるためのWindowsネイティブな読み取り専用ワークベンチ。</strong></p>

![実際に動作しているJsonlLensの画面](assets/jsonllens-demo.gif)

上のGIFは実際に起動したJsonlLens Windowsデスクトップ版をキャプチャしたものです。JsonlLensは、通常のテキストエディターでは重くなりやすい大容量ファイルを、スパースインデックス、仮想化された行表示、DuckDBストリーミングで扱います。

## 主な機能

- JSONL / NDJSONの最初のページをすばやく表示
- ファイル全体をUIへ読み込まずにページングできるメモリ使用量
- 推論したフィールドを並べ替え可能な列として表示
- クイックフィルターとDuckDB SQLコンソール
- JSONの詳細インスペクターと生の行表示
- 誤編集を防ぐ読み取り専用設計
- `.jsonl`、`.ndjson`、`.parquet`、`.csv`、構造化ログに対応

## ベンチマークスナップショット

Windows 11 x64、SSD、拡張機能なしで5 GBの合成JSONLを開いた代表値です。実際の結果はディスク、ウイルス対策、拡張機能、ファイル構造によって変わるため、同じ手順で再測定してください。

| ビューアー | 最初に操作できるまで | 最大ワーキングセット | 結果 |
| --- | ---: | ---: | --- |
| **JsonlLens** | **0.84秒** | **183 MB** | ページングとフィルターを操作可能 |
| VS Code（5 GB JSONL） | 2分41秒 | 2.78 GB | 読み込み中に応答しなくなった |

## Microsoft Storeから入手

署名済みWindowsパッケージと通常のStore更新を利用できます。

<p align="center">
  <a href="https://apps.microsoft.com/detail/9N9X7K90R64G">
    <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="260" alt="Microsoft Storeから入手" />
  </a>
</p>

- Windows 10 / 11、x64
- 読み取り専用の大容量データビューアー
- SQLとエクスポートのPro機能

## フィードバック

問題を報告する場合は、Windowsのバージョン、ファイル形式、再現手順をIssueに記載してください。サンプルやスクリーンショットから秘密情報を削除してください。

