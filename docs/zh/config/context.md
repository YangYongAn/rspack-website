# Context 基础目录

用于设置 Rspack 构建的基础目录。

- **类型：** `string`
- **默认值：** `process.cwd()`

`context` 是一个绝对路径，它被用作为 Rspack 配置中相对路径的基础路径，比如 [entry](/config/entry.html) 和 [loader](/config/loader.html) 等配置中包含的相对路径。

默认情况下，Rspack 会使用 Node.js 进程的当前工作目录作为基础目录。在大多数情况下，我们推荐手动设置一个基础目录，而不是依赖 Node.js 的当前工作目录。

## 示例

比如，你可以使用 `__dirname` 作为基础目录：

```ts title="rspack.config.js"
module.exports = {
  context: __dirname,
  entry: {
    main: './src/index.js',
  },
};
```

在上述例子中，`main` 入口会基于 `path.join(__dirname, './src/index.js')` 路径进行解析。