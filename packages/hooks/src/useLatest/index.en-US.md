---
title: useLatest
nav:
  title: Hooks
  path: /hooks
group:
  title: Advanced
  path: /advanced
---

# useLatest

<Tag lang="en-US" tags="ssr&crossPlatform"></Tag>

The Hook that returns the latest value, can avoid the closure problem.

## Examples

### Basic usage

<code src="./demo/demo1.tsx" />

## API

```typescript
const latestValueRef = useLatest<T>(value: T): MutableRefObject<T>;
```