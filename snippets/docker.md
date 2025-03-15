

### 사용하지 않는 이미지 전부 삭제

```bash
docker rmi $(docker images -q)
```