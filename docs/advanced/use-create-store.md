# useCreateStore

## Leva vs LevaPanel

Using the `<Leva>` component and `useControls` will default to using the global levaStore. If you need finer grained control or wish to display multiple indendently managed panels you'll want to pass in a new store and use the `LevaPanel` component instead.

```jsx
const store = useCreateStore();

useControls(schema, {store});

return <LevaPanel store={store} />
```

