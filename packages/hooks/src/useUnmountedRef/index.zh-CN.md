---
title: useUnmountedRef
nav:
  title: Hooks
  path: /hooks
group:
  title: LifeCycle
  path: /life-cycle
---

# useUnmountedRef

<Tag lang="zh-CN" tags="ssr&crossPlatform"></Tag>

获取当前组件是否已经卸载的 Hook。

## 代码演示

### 基础用法

<code src="./demo/demo1.tsx" />

## API

```typescript
const unmountRef: { current: boolean } = useUnmountedRef();
```

### Result

| 参数       | 说明             | 类型                   |
|------------|------------------|------------------------|
| unmountRef | 组件是否已经卸载 | `{ current: boolean }` |
