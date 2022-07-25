# 第３回課題
## RailsのSample AppをcloneしてCloud9にデプロイする
### APサーバー
| name | version | 起動コマンド |
| ---- | ---- | ---- |
| puma | 5.6.4 | rails s |


#### APサーバを停止させた場合
| 停止コマンド | access | 表示 |
| ---- | ---- | ---- |
| Ctrl-C | 不可  |**Oops**<br>No application seems to be running here! |


### DBサーバー
| name | version | バージョン確認コマンド |
| ---- | ----| ---- |
| MySQL | 8.0.29 | mysql --version |


#### DBサーバーを停止させた場合

| 停止コマンド | access | 表示 |
| ---- | ---- | ---- |
| sudo service mysqld stop | 不可 | ActiveRecord::ConnectionNotEstablished |

### Railsの構成管理ツール
Bundler

### 第３回の課題で学んだこと
* RailsにはpumaというAPサーバが組み込まれているため、
ApacheやNginxなどのWebサーバーなしでもWebアプリを起動することができる。 

* RailsはAPサーバーとDBサーバーが両方起動していないと正常に起動しない。

* Railsは簡単にWebアプリをデプロイできるフレームワークと言われているが、
実際にやってみるとdatabase.yml、credentials.yml.enc、webpackerと、ハマりどころが多い。  

* Railsのアプリケーションをデプロイする場合
ec2のt2.microだと、CPUもメモリもギリギリ過ぎて、時々止まってしまう。

* 他の人が作ったアプリをCloneして起動させるのは、
自作のアプリをデプロイするより難しく感じた。

### 気になっている点
* 先生のsample app と自分がデプロイしたappのnodeとyarnのバージョンが異なっている。
バージョンの揃え方が調べてもよくわからかった。


