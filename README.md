# BMS Bundle Manifest Specfication (WIP)

**まだ WIP なので、v1 ではありません、ご注意。**

BMS のリソース情報を記述するマニフェスト仕様です。  
JSON Schema で定義されています。

主に本体や差分のダウンロード先を記述・公開するために使用します。  
あくまで BMS 作品を単位としてリソースの集合体を定義するもので、譜面の情報に着目しない点で難易度表とは異なるフォーマットです。

自動生成の [docs](https://github.com/bmssearch/bms-bundle-spec/blob/master/docs/v1/README.md) もありますが、冗長なので実際の [schema](https://github.com/bmssearch/bms-bundle-spec/tree/master/schemas) を見たほうがいいと思います。

## Helpers

Online Validator(coming soon) を使うと記述したマニフェストが仕様に合致しているか確認することができます。

マニフェストのパースや作成、バージョン互換の操作を簡単に行えるモジュールを公開しています。

| Language   | Link                                                |
| ---------- | --------------------------------------------------- |
| JavaScript | https://github.com/bmssearch/bms-bundle-manifest-js |
| PHP        | ない                                                |

## Usage

マニフェストを作成し、web 上に json として公開します。  
マニフェストには `BMS`, `グループ`, `更新` の 3 種類が存在します。

### BMS マニフェスト

BMS の基本的な情報とダウンロード先を記述します。  
最小限このマニフェストだけ用意すればリーダーは BMS のリソース情報を把握することができます。

### グループマニフェスト

イベントやプレイリストなど、BMS の集合を記述できます。  
内包する BMS として言及できるのは同一ドメイン内にマニフェストが存在する BMS のみという点に注意してください。

### 更新マニフェスト

BMS マニフェストに加わった変更を記述します。  
このマニフェストを用意することで、リーダーは手元のマニフェストを常に最新の状態に保つことができるようになります。  
更新マニフェストを提供するページは、 `?from=XXXXX(millisec)` のパラメーターでいつ以降の更新を返却するか絞り込めるようにすることを推奨しています。

## Examples

BMS SEARCH venue は Bms Bundle Manifest を公開しています。  
たとえば以下のページで確認できます。

- https://venue.bmssearch.net/bmsshuin3/1/manifest
- https://venue.bmssearch.net/bmsshuin3/manifest
- https://venue.bmssearch.net/updates_manifest?timestamp=1618498070417

## Contributing

必要に応じて変更を加えてバージョンを上げていく予定です。  
気軽に Issues を作成してください。
