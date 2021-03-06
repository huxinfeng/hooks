---
title: useMount
nav:
  title: Hooks
  path: /hooks
group:
  title: LifeCycle
  path: /life-cycle
---

# useMount

<Tag lang="en-US" tags="ssr&crossPlatform"></Tag>

A hook that executes a function at mount.

## Examples

### Default Usage

<code src="./demo/demo1.tsx" />

## API

```typescript
useMount(fn: () => void);
```

### Params

| Property | Description                      | Type         | Default |
|----------|----------------------------------|--------------|---------|
| fn       | The function need to be executed | `() => void` | -       |
