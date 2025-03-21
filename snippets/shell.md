

#### 특정 port 를 사용하는 process kill


```
sudo lsof -t -i:$1 | xargs -r kill -9
```
