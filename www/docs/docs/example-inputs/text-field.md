# TextField

```tsx
function TextField() {
  const {
    field: { onChange, value },
    error,
  } = useZodController<string>();

  return (
    <>
      <input
        onChange={(e) => onChange(e.target.value)}
        value={value ? value : ""}
      />
      {error && error.errorMessage}
    </>
  );
}
```
