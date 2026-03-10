# Blog Plugin Market

独立插件市场仓库，存放 `Blog` 后台插件的公开目录与 manifest。

## 目录结构

- `index.json`
  插件索引。后端会先读取这里，再按 `manifest_path` 抓取每个插件的 manifest。
- `plugins/<plugin-id>/manifest.json`
  单个插件的元数据定义。
- `plugins/_template/manifest.template.json`
  新插件上架时可复制的模板。

## 设计目标

- 市场目录与业务仓库分离
- 支持发布者、版本、兼容性、权限、能力、文档链接等常见市场字段
- 当前应用优先支持 `builtin-toggle` 安装策略
- 后续可以扩展为 `iframe`、`package`、`remote-worker` 等运行方式

## 当前收录

- `ai-assistant`
- `wechat-official-account`
