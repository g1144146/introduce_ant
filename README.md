# MacでのAntの導入方法
ここでは、Homebrewなどのパッケージ管理ソフトを使わずに  
環境変数やらを使って導入する方法をメモ程度に。

---

## Antをダウンロード

1. [Apache Ant](http://ant.apache.org/)にてAntをダウンロード
2. ダウンロードされたAntがあるディレクトリにてzipを解凍  
    $ unzip apache-ant-1.x.x-bin.zip
3. 解凍したフォルダを移動
    * コピーする場合
        * $ cp apache-ant-1.x.x/ /usr/local/
    * 移動する場合
        * $ mv apache-ant-1.x.x/ /usr/local/
    * 権限がないと言われたら、先頭に'sudo'をつける