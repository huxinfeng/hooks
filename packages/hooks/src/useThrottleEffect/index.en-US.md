---
title: useThrottleEffect
nav:
  title: Hooks
  path: /hooks
group:
  title: LifeCycle
  path: /life-cycle
---

# useThrottleEffect

<Tag lang="en-US" tags="ssr&crossPlatform"></Tag>

Throttle your `useEffect`.

## Examples

### Default usage

<code src="./demo/demo1.tsx" />

## API

```typescript
useThrottleEffect(
  effect: EffectCallback,
  deps?: DependencyList,
  options?: Options
);
```

### Params

| Property | Description                                                  | Type             | Default |
|----------|--------------------------------------------------------------|------------------|---------|
| effect   | The effect callback.                                         | `EffectCallback` | -       |
| deps     | The dependencies list.                                       | `DependencyList` | -       |
| options  | Config the throttle behavior. See the Options section below. | `Options`        | `{}`    |

### Options

| Property | Description                                           | Type      | Default |
|----------|-------------------------------------------------------|-----------|---------|
| wait     | The number of milliseconds to delay.                  | `number`  | `1000`  |
| leading  | Specify invoking on the leading edge of the timeout.  | `boolean` | `true`  |
| trailing | Specify invoking on the trailing edge of the timeout. | `boolean` | `true`  |
