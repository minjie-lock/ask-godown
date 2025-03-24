# ask-godown

_轻量的集中状态管理库_

```ts
import { createGodown } import 'ask-godown'

type Store = {
  value: number;
  setValue: () => void;
}

const useGodown = createGodown<Store>((set) => {
  return {
    value: 0,
    setValue: () => {
      set((state) => ({value: state.value++ }))
    }
  }
})
```
