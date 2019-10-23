# mkfifo 一個他媽bash就可以玩的job queue

```sh
# 先製造一個 broker
mkfifo broker

# 讓消費者 不斷工作 + 背景執行
sh consumer.sh &

# 推入工作,即可開始消費
sh producer.sh
```

