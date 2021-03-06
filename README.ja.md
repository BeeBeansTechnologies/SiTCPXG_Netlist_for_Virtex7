Read this in other languages: [English](README.md), [日本語](README.ja.md)

# SiTCPXG Netlist for Virtex7

Xilinx Virtex7用のSiTCPXG Netlist File(edif file)です。


## SiTCPXG とは

物理学実験での大容量データ転送を目的としてFPGA（Field Programmable Gate Array）上に実装されたシンプルなTCP/IPであるSiTCPの10GbE専用ライブラリです。

* SiTCP、SiTCPXGについては、[SiTCPライブラリページ](https://www.bbtech.co.jp/products/sitcp-library/)を参照してください。
* その他の関連プロジェクトは、[こちら](https://github.com/BeeBeansTechnologies)を参照してください。

![SiTCP](sitcp.png)


## 履歴

#### 2021-12-02 Ver.2.0

* 受信時の最小 IFG を 12Byte から 4Byte に短縮
* 送信時の IFG を 74Byte（1518Byte パケット時）から平均 12Byte に短縮
* RST 受信後の送信が異常になる不具合を修正
* クライアントモード時、セッション確立前のタイムアウト機能を削除
* ファスト・リトランスミッションの改善（不要な再送の削減）
* セッション終了時のタイムアウト追加

#### 2021-04-02 Ver.1.0

* 新規登録。

