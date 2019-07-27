# ファイルパーミッション
ubuntuにおけるファイルパーミッションの仕組みが分かりにくいので、まとめてみる。
## ファイルのオーナーシップ
Linuxにおけるオーナーシップは以下の３タイブに分けられる。
### ユーザー

### グループ

### その他

## ファイルパーミッション
### Read
Readパーミッションはファイルを開いたり、読んだりする権利を与えます。
### Write
Writeパーミッションは、ファイルのコンテンツを変える権利を与えます。
### Execute

<!--
## ファイルマネージャーでの取扱い 
ファイルマネージャーでの取扱いはファイルかフォルダーかによって変わってくる。

### ファイルの場合
ファイルにおいて、プログラムとして実行可能かはチェックポックスで一括して設定するので、以下では省略する。  
Read-only=r-  
Read and write=rw  
None=--

### フォルダーの場合
List files only=r--  
Access files=r-x  
Create and delete files=rwx  
None=---
-->

## デフォルトでの設定
デフォルトでは  umaskの値は044ですが、ファイルの属性はバラバラです。  
File 044=rw--w--w-  
File 022=rw-r--r--  
File 002=rw-rw-r--



## 参考文献
[File Permissions in Linux/Unix with Example](https://www.guru99.com/file-permissions.html)  
[Set the default permissions for newly created files](https://geek-university.com/linux/set-the-default-permissions-for-newly-created-files/)

