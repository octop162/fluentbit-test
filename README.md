
### 流れ

fluent-bit.confを修正

docker-composeで起動

```
docker-compose run fluent-bit
```

data.logを適当に変更して保存する

標準出力されるはず

### 実行例

```
❯ docker-compose run fluent-bit
Fluent Bit v1.8.12
* Copyright (C) 2019-2021 The Fluent Bit Authors
* Copyright (C) 2015-2018 Treasure Data
* Fluent Bit is a CNCF sub-project under the umbrella of Fluentd
* https://fluentbit.io

[2022/03/01 14:04:53] [ info] [engine] started (pid=1)
[2022/03/01 14:04:53] [ info] [storage] version=1.1.5, initializing...
[2022/03/01 14:04:53] [ info] [storage] in-memory
[2022/03/01 14:04:53] [ info] [storage] normal synchronization mode, checksum disabled, max_chunks_up=128
[2022/03/01 14:04:53] [ info] [cmetrics] version=0.2.2
[2022/03/01 14:04:53] [ info] [sp] stream processor started
[2022/03/01 14:04:53] [ info] [input:tail:tail.0] inotify_fs_add(): inode=369067 watch_fd=1 name=/tmp/data.log
[0] blue: [1646143494.060900000, {"color"=>"blue", "label"=>{"name"=>nil}}]
[0] blue: [1646143495.394483400, {"color"=>"blue", "label"=>{"name"=>nil}}]
[0] blue: [1646143496.053268200, {"color"=>"blue", "label"=>{"name"=>nil}}]
```