# ぎゅうぎゅうりんちゃん

**ver 1.0.0**（2026-08-22 公開）

Unity WebGL のメダルプッシャーゲーム。https://halkaclub.com/game/gyugyu-rinchan/ から遊べます。

このリポジトリは **ビルド成果物だけ** を置いています。ソースは別管理です。

## 更新のしかた

1. Unity で `RinPusher > Build > WebGL`（または `-executeMethod RinPusher.EditorTools.BuildWebGL.Build`）
2. 出力された `Build/WebGL` の中身をこのリポジトリ直下へ上書き
3. push すると GitHub Pages が自動で反映

## 注意

- `*_BurstDebugInformation_DoNotShip` は含めないこと。Unity が配布禁止と明示しているデバッグ情報です
- `.nojekyll` は消さないこと。GitHub Pages の Jekyll 処理を止めています
- 圧縮は Brotli ですが Unity 側で `decompressionFallback` を有効にしてあるため、
  サーバーのヘッダー設定なしで動きます
