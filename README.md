# Mineradio 插件市场

Mineradio 的插件目录站点：歌词预设、界面工具与音源插件。

## 目录内容

- `index.html` — 插件市场网页（搜索、分类、详情、下载）
- `plugins.json` — Mineradio 插件仓库目录（`schemaVersion: 1`）
- `packages/` — 插件安装包（zip），每个包都附有 SHA-256 与大小

## 在 Mineradio 中使用

1. 打开 Mineradio →「扩展插件」→「在线插件商店」→「仓库管理」。
2. 添加本仓库的 `plugins.json` 地址，例如：
   `https://<用户名>.github.io/mineradio-plugins/plugins.json`
3. 回到商店列表，选择插件安装；安装前 Mineradio 会按目录里的 SHA-256 复核文件。

## 更新插件

保持插件 `id` 不变，提升 `version` 并替换 `packages/` 下的包，然后重新运行生成脚本或手动更新 `plugins.json` 中的 `sha256`、`size`、`url`。插件 ID 与包内 `manifest.json` 必须一致。

## 许可

各插件自带 `LICENSE` / `NOTICE` / 第三方许可证声明，随包分发；本仓库仅提供目录与分发。
