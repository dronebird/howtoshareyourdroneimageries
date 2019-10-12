災害ドローン救援隊DRONEBIRD流

# howtoshareyourdroneimageries 
How to share your drone imageries. あなたのドローン空撮画像を共有する方法

v0.9
適宜更新していきます。

## 標準仕様
* 各種SfMツールでオルソモザイク処理を行う。
* 撮影時のオーバーラップ率はサイドラップ共に70%以上を目指す。
* ローリングシャッターカメラよりグローバルシャッターカメラが良いが、災害時はどちらでも良い。
* 位置補正は単独測位GPSによるジオタギングで十分。RTK利用は理想だが作業効率を重視。
* マニュアルGCP補正は極力行わず、データ公開のスピードを重視。
* GeoTIFFファイルとして出力（測地系設定は EPSG:4326, WGS84）。
* 4GBを超える GeoTIFFの場合は BigTIFFタイプを優先


## Google Drive
* GeoTIFFファイルをそのまま置いておく。
* ファイルの共有設定を誰でも閲覧可能にする。

## OpenAerialMap
* Googleアカウントでログイン
* アップロード画面で各種情報を入力後 Google Driveにアップロードした GeoTIFFファイルをリストから表示

## GitHub
* 撮影データセットごとに公開リポジトリを立てる。
* XYZタイルデータセットを GitHub Desktop ツールを用いてPush(アップロード)
* リポジトリを GitHub Pages 設定にして、ホスティングする。
* GeoTIFFファイルはファイルサイズが大きいので、LFSでアップロードできるのであれば実施(無理はしない)。
