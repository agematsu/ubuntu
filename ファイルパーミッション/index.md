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
### ファイルの場合
ファイルにおいて、プログラムとして実行可能かどうかはチェックポックスで一括して設定できる。
Read-only=r--  
Read and write=rw-  
None=---
### フォルダーの場合
List files only=r--  
Access files=r-x  
Create and delete files=rwx  
None=---
-->

## デフォルトでの設定
デフォルトでは  umaskの値は044ですが、ファイルの属性はバラバラです。  
044=-rw--w--w-, drwx-wx-wx  
022=-rw-r--r--, drwxr-xr-x   gedit  
002=-rw-rw-r--, drwxrwxr-x   nautilus, others



## 参考文献
[File Permissions in Linux/Unix with Example](https://www.guru99.com/file-permissions.html)  
[Set the default permissions for newly created files](https://geek-university.com/linux/set-the-default-permissions-for-newly-created-files/)

