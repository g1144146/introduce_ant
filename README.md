# MacでのAntの導入方法
ここでは、Homebrewなどのパッケージ管理ソフトを使わずに  
環境変数やらを使って導入する方法をメモ程度に。

---

## Antをダウンロード

1. [Apache Ant](http://ant.apache.org/)にてパッケージをダウンロード

2. ダウンロードされたAntがあるディレクトリにて、パッケージを解凍

    `$ unzip apache-ant-1.x.x-bin.zip`

3. 解凍したフォルダを移動（移動先はお好みで）

    * コピーする場合

        `$ sudo cp apache-ant-1.x.x/ /usr/local/`

    * 移動する場合

        `$ sudo mv apache-ant-1.x.x/ /usr/local/`

    * シンボリックリンクの場合

        `$ sudo ln -s apache-ant-1.x.x/ /usr/local/`

## 環境変数を設定

1. .bash_profileを編集

    `$ nano ~/.bash_profile`

2. .bash_profileにPATHを追加

    export ANT_HOME=/usr/local/apache-ant-1.x.x  
    export PATH=$PATH:$ANT_HOME/bin

3. 追加したPATHを反映

    `$ source ~/.bash_profile`

4. 確認
```
    $ ant -version
    Apache Ant(TM) version 1.x.x compiled on [month] [day] [year]
```
Apache Ant... が表示されれば成功

