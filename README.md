# mkfifo 一個他媽bash就可以玩的job queue

```sh
# 先製造一個 broker
mkfifo broker

# 讓消費者 輪詢監聽fifo + 背景執行
sh consumer.sh &

# 推入工作,即可開始消費
sh producer.sh
```

### 管理
```sh
# 使用
jobs  #看
bg %1  #背後運行
fg %1   #拿到前台
kill %1   #讓他死
```

### 持久化
```
保留 broker 黨就好
```
