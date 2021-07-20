# よく使うソフトウェアをインストール

## プログラミング ➖ Scratch3

Raspberry Piではおすすめソフトをインストールするためのツールが用意されている。

「ラズベリマーク」ー>「設定」ー>「Recommand　Software」の順をクリックすると、「Recommand　Software」が起動される。

![](./img/Recommandsoftware.png)


「Recommand　Software」の画面左で「Programming」をクリックし、右側のリストでScratch３のチェックボックスをチェックして、「Apply」ボタンを押すと、Scratch３がインストールされる

![](./img/install-Scratch3.png)

## ワープロ ➖ LibreOffice

Scratch 3と同様にインストールする。
![](./img/install-libreoffice.png)

## プログラミング ➖ Visual Studio Code

![](./img/install-vscode.png)


## スクリーンショット ➖ Shutter

スクリーンショットを取るソフトShutterをsnap　storeからインストールする。

ターミナルで以下のコマンドを実行する。

- snap storeをインストール
  ```shell
  sudo apt update
  sudo apt install snapd
  ```
- 再起動
  ```shell
  sudo reboot
  ```
- 最新のsnapを取得
  ```shell
  sudo snap install core
  ```
- shutterをインストールする
  ```shell
  sudo snap install shutter
  ```

## タイピング練習

### 算数タイピング ➖ tuxmath

画面に出ている四則計算の答えを打てゲーム感覚で数値入力の練習ができる。
シェルからインストールする。
```shell
sudo apt install tuxmath
```
実行完了すると、メニュー「教育・教養」の中に「Tux Math」というアプリケーションがインストールされる。


### キータイピング ➖ tuxtype

数値以外のタイピング練習用に`tuxtype`を利用します。
```shell
sudo apt install tuxtype
```
実行完了すると、メニューの「教育・教養」の中に「Tux Typing」というアプリケーションがインストールされる。
![](./img/TuxTypingMenu.png)

## ライブプログラミング ➖ Sonic Pi

「Recommand　Software」の中にあるSonic Piのバージョンが古く、起動時に失敗するので、最新版を本家ホームページからダウンロードしてインストール。

- 古いバージョンのSonic Piをアンインストールする。
  ``` shell
  sudo apt purge sonic-pi
  ```
- 別のパッケージを残っていないかを確認
  ```shell
  dpkg -l | grep sonic-pi
  ```
  なにか残っていれば、`sudo apt purge xxx`でアンインストールする。
- [本家ホームページ](https://sonic-pi.net/)からパッケージをダウンロードする。
  ![](./img/SonicPi-dl.png)
- 「Download」をクリックすると、`sonic-pi_3.3.1_1_armhf.deb`というファイルが自分の「Downloads」フォルダにダウンロードされる。
- インストール
  ```shell
  cd ~/Downloads
  sudo dpkg -i sonic-pi_3.3.1_1_armhf.deb
  ```
  実行が終わると、何か依存されているライブラリがインストールされていない云々が言われるので、言われた通り以下のコマンドを実行する。
  ```shell
  sudo apt --fix-broken install
  ```
  実行完了すると、メニュー「プログラミング」の中に「Sonic Pi」というアプリケーションがインストールされる。
  ![](./img/SonicPi-menu.png)
- 上記「Sonic Pi」をクリックすると、アプリケーションが起動される。
  ![](./img/SonicPiStartup.png)
