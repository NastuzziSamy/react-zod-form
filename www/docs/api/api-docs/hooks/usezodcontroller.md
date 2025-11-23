---
sidebar_position: 1
---

# useZodController

## `useZodController`

A typesafe hook that automatically connects to your form state:

```tsx
function TextField() {
  const {
    field: { onChange, value },
    error,
  } = useZodController<string>();
  // ...
}
```

Returns everything that `react-hook-form`'s [useController](https://react-hook-form.com/api/usecontroller) returns plus an extra `error` object and slightly modified typings to make the form state more intuitive to work with.
