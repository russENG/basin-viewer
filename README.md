# 流域データ確認ビューア（公開版）

全国の観測所と算出流域・河川を確認する Web マップ。静的ホスティング（Cloudflare Pages 等）
に置くだけで動く（タイルサーバ不要）。

## 収録レイヤと出典（CC-BY / ODbL のみ）

- 水位・雨量観測所: 出典 国土交通省 水文水質データベース (https://www1.river.go.jp/)
  を加工して作成（PDL1.0、CC BY 4.0 互換）
- 算出流域（①水位観測所トラック 62 / ②ダム流入トラック 41、束ねて 91 流域の最終選定）:
  J-FlwDir (Yamazaki et al., CC BY 4.0) を加工して作成
- 河川（線）: © OpenStreetMap contributors, ODbL（waterway を加工して作成）
- 背景地図: Geolonia / 国土地理院 / OpenStreetMap

国土数値情報（河川 W05・ダム W01・流域界 W12）は**非商用利用のみ**のため公開版には収録していない。
河川は OSM（ODbL）で代替している。

## Geolonia 背景

Geolonia 背景には API キー（ドメイン制限）が必要。`config.js` の `geoloniaKey` に設定する。
未設定でも国土地理院 淡色を初期背景として動作する。
