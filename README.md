# kadai1
This isa a kadai1 repository.
授業で作成したコードにLEDをもう一つ追加し一つづつ点灯，二つ同時に点灯するようにしました．

#使い方
以下の(1)~(6)の手順で動作させます．
(1)リポジトリを複製する．$ git clone https://github.com/yukihorio/myled.c.git
(2)ディレクトリを移動.cd myled/
(3)コンパイル$ vi Makefile $ make $ vi myled.c $ make
(4)モジュールをロード$sudo insmod myled.c
(5)権限を与える$ sudo chmod 666 /dev/myled0
(6)LED1点灯 $ echo 1 > /dev/myled0
   LED2点灯 $ echo 2 > /dev/myled0
   LED1,2点灯 $ echo 3 > /dev/myled0
   LED消灯 $ echo 0 > /dev/myled0
