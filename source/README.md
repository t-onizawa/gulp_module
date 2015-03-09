# gulpの使い方

- node.jsをインストールしてください。
- sassをインストールしておいてください。 

## インストール

このファイルのディレクトリからcompornentsに移動して下さい。

```
cd compornents
```




グローバルにgulpをインストールします。

```
npm install gulp -g
```

ローカルのプロジェクトにもgulpをインストールします

```
npm install gulp
```

### 初期作成の場合

gulpのプラグインをインストールします。

```
npm install gulp-ruby-sass gulp-autoprefixer gulp-minify-css gulp-jshint gulp-uglify gulp-imagemin gulp-csscomb gulp-notify gulp-plumber gulp-cached gulp-spritesmith gulp.spritesmith require-dir js-yaml gulp-changed --save-dev
```

### 通常インストール

```
npm install
```


## 設定

path.yml内の読み込み・書き出しパスを確認します。

## 実行

CSS, JavaScriptタスクは以下で起動します。

pcファイル
- /javascript/pc
- /scss/pc

```
gulp pc
```

spファイル
- /javascript/sp
- /scss/sp

```
gulp sp
```



※ 画像のminify化をするときは、/image/pc, sp内に入れ
画像用のtaskを起動させます。

画像の圧縮値は都度変えてください。デフォルト設定になっています。

pc (htdocs/base/image/pc → htdocs/img)
 ```
 gulp pc-imgmin
 ```

sp (htdocs/base/image/sp → htdocs/imgSP)
```
gulp sp-imgmin
```


※ 画像のspriteを作るときは、/image/sprite/pc, sp内に入れ
下記taskを起動します。

pc (htdocs/base/image/sprite/pc → htdocs/img)
```
gulp pc-sprite
```

sp (htdocs/base/image/sprite/sp →  htdocs/imgSP                                                                                                                                                                                                                                                                                                                                                                                                                       )
```
gulp sp-sprite
```

