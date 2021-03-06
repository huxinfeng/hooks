---
title: useFullscreen
nav:
  title: Hooks
  path: /hooks
group:
  title: Dom
  path: /dom
---

# useFullscreen

<Tag lang="en-US" tags="ssr"></Tag>

manages DOM full screen.

## Examples

### Default usage

<code src="./demo/demo1.tsx" />

### Image full screen

<code src="./demo/demo2.tsx" />

## API

```typescript
const [
  isFullscreen, 
  {
    enterFullscreen, 
    exitFullscreen, 
    toggleFullscreen 
  }] = useFullScreen(
    target,
    options?:Options
  );
```

### Params

| Property   | Description                        | Type        | Default |
|------------|------------------------------------|-------------|---------|
| target     | DOM element or ref          | `Element` \| `() => Element` \| `MutableRefObject<Element>` | -       |
| options | Setting(optional)            | `Options`     | -      |

### Options

| Property   | Description                        | Type        | Default |
|------------|------------------------------------|-------------|---------|
| onExit | Exit full screen trigger | `()=>void`    | -       |
| onEnter     | Enter full screen trigger     | `()=>void`    | -       |

### Result

| Property     | Description        | Type     |
|--------------|--------------------|----------|
| isFullscreen | Is full screen     | `boolean`  |
| enterFullscreen      | Enter full screen    | `()=>void` |
| exitFullscreen     | Exit full screen   | `()=>void` |
| toggleFullscreen   | Toggle full screen | `()=>void` |
