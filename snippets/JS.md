
### 잠시 대기하는 함수

```
const deplay = (ms) => {
  return new Promise((resolve) => setTimeout(resolve, ms));
}
```