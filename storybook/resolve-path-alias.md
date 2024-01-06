If the import path alias `@` is not being resolved in Storybook, add a Webpack configuration to resolve the path alias.

```typescript
webpackFinal: async (config) => {
  if (config.resolve) {
    config.resolve.alias = {
      ...config.resolve.alias,
      '@': path.resolve(__dirname, '../src'),
    };
  }
  return config;
},
```