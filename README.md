## 全体概要　https://github.com/city-soja-chiiki/QGIS  
# 5.QGISプラグイン等の開発・保守  
　【概算】130万円/年（650万円/5年）  
　**開発したプラグイン等はオープンソースによりGitHUB等に公開されます。**
　
### 5-1.ログイン画面  
　【概算】20万円/年（100万円/5年）  
　起動時（プロジェクトファイル読み込み完了時）に認証する。認証情報はローカルDBに保存することを想定  
　ユーザの操作により、認証画面再表示可能  
　ユーザ認証後、プロジェクトファイルの変更をし、再読み込み  
### 5-2.プロジェクト変数編集プラグイン
　【概算】20万円/年（100万円/5年）  
　読み込んでいるプロジェクトファイルの変数をグループごとにタブ表示  
　各変数について、名称、説明、内容をリスト表示  
　内容の編集については、テキスト、日付、ＪＳＯＮとする  
　グループ、変数については別途プロジェクト変数で指定可能とする  
### 5-3.レイヤ属性編集プラグイン  
　【概算】40万円/年（200万円/5年）  
　直接接続はできないため、編集するレイヤ属性を選択しEXCELに出力  
　出力したデータを編集し、ファイル選択してQGISに入力  
　ジオメトリについては、WKT形式による指定を想定（点データのみであれば座標値の指定でも対応可）  
　ジオメトリがないレイヤの場合には、EXCEL、CSV出力時にジオメトリフィールドの指定ができるようにする  
　データチェック方法  
　　　出力時は非表示シートへ元データを追加  
　　　入力時は非表示シートの元データとQGISにある現在データが同一であるかをチェック  
　　　入力時はフィールド名、型のチェックを実施  
### 5-4.汎用調書作成機能[機能強化]  
　【概算】20万円/年（100万円/5年）   
　https://github.com/yamamoto-ryuzo/QGIS-exportExcel  
　QDATE,QDATETIME対応  
### 5-5.属性検索プラグイン[機能強化]   
　【概算】20万円/年（100万円/5年）   
　https://github.com/yamamoto-ryuzo/GEO-search-plugin  
　レイヤ変数に検索用JSONを埋め込み他のプロジェクトファイルでも検索表示可能とする。  
　3.22対応  
### 5-6.凡例表示プラグイン[機能強化]   
　【概算】10万円/年（50万円/5年）   
　https://github.com/yamamoto-ryuzo/QGIS-legendView  
　ﾃﾞﾌｫﾙﾄ表示「カレントビュー」の追加  
　チェックボックス、プロジェクト変数（表示優先順位,表示非表示）による複数選択の追加  
　（検討）埋込レイヤで埋め込まれた先への変数引き渡しが可能なら、レイヤ変数の採用もあり！  
　　　　　常に表示したいレイヤは、レイヤ変数へ設定すれば、他のプロジェクトでも自動で表示！  
