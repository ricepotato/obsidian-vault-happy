
### 잠시 대기하는 함수

```
const deplay = (ms: number) => {
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


#### Typescript 의 enum 대체제



```typescript
export const AddressErrors = {
  DuplicateAddress: "DuplicateAddress",
  FileSizeExceeded: "FileSizeExceeded",
  SizeLimitExceeded: "SizeLimitExceeded",
  InvalidAddress: "InvalidAddress"
}

export type AddressError = (typeof AddressErrors)[keyof typeof AddressErrors];
```

출처 : https://velog.io/@leehaeun0/typescript-enum-%EC%9D%84-union%EC%9C%BC%EB%A1%9C-%EB%B3%80%EA%B2%BD%ED%95%98%EA%B8%B0