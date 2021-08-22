# intro-programming

子供にプログラミングを教えるためのリポジトリ

## 環境

Raspberry Pi 4 Model B 4GB

- モデル
  ```shell
  $ cat /proc/device-tree/model
  Raspberry Pi 4 Model B Rev 1.4
  ```

- OS

  Raspberry Pi OS with desktop 32 bit

  ```shell
  $ lsb_release -a
  No LSB modules are available.
  Distributor ID:	Raspbian
  Description:	Raspbian GNU/Linux 10 (buster)
  Release:	10
  Codename:	buster
  ```

- カーネル
  ```shell
  $ uname -a
  Linux raspberrypi 5.10.17-v7l+ #1421 SMP Thu May 27 14:00:13 BST 2021 armv7l GNU/Linux
  ```


## 記録

- 2021.07.18

  組み立て＆初期設定

  [参考資料](./raspi/RaspberryPi組み立てと初期設定.pdf)

- 2021.07.22
  - ソフトウェアをインストール

    [参考資料](./raspi/install-software-to-raspi.md)

    Scratch3、LibreOffice、Sonic Pi、tuxtype

  - ターミナル＆コマンドの簡単な説明
    - ターミナルの起動
    - コマンド

      `ls`、`cd`、`pwd`、`sudo`、`apt`等

- 2021.07.31
  - Scratch 1回目

    素材はあの有名な(？)ねこ歩き。

    [資料](./raspi/scratch3-intro.md)

    ※ 少し簡単過ぎたようだ。

  - 数当てゲーム

    ２分法の話

- 2021.08.14
  - Scratch 2回目

    codedojo参加 ---- [プログラミングでポケモンをうごかしてみよう](https://coderdojo-hamamatsu.connpass.com/event/218934/)

- 2021.08.22
  - Sonic Pi 1回目

    [資料](./sonicpi/sonicpi-01.md)
    - `play`で音符再生
    - `sleep`でリズムをつける
    - `use_bpm`でテンポを変える
    - 繰り返す

    参考：

    [Music Programming Basics](https://mehackit.org/en/courses/music_programming_basics/)
