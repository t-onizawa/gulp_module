# gulpの使い方

- node.jsをインストールしてください。
- sassをインストールしておいてください。 

## インストール

このファイルのディレクトリからsource内のcompornentsに移動して下さい。

```
cd sourse/compornents
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

CSS, JavaScript, imgタスクは以下で起動します。

```
gulp
```




※ 画像のminify化のみをするときは、/images/内に入れ
画像用のtaskを起動させます。

画像の圧縮値は都度変えてください。デフォルト設定になっています。

```
gulp img
```


※ 画像のspriteを作るときは、/image/sprite/に入れ
下記taskを起動します。

```
gulp sprite
```

起動後、読み込むscssファイルに@import parts/spriteしてください
