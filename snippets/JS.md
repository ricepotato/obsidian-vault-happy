
### 잠시 대기하는 함수

```
const deplay = (ms) => {
  return new Promise((resolve) => setTimeout(resolve, ms));
}
```


### Timeout Component

```typescript
import type { AwaitedReactNode } from "react";

type Props = {
  children: AwaitedReactNode;
  timeout?: number;
};

export async function Timeout({
  children,
  timeout = 2000,
}: Props): Promise<AwaitedReactNode> {
  await new Promise((resolve) => setTimeout(resolve, timeout));
  return children;
}
```