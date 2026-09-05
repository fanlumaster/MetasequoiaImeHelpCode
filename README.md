> **本仓库已迁移并归档 / This repository has moved and is archived.**
>
> 当前源码与后续维护位于 [MSIME-Engine 的 `helpcode/`](https://github.com/metasequoiaime/MSIME-Engine/tree/main/helpcode)。
> 请在 [MSIME-Engine](https://github.com/metasequoiaime/MSIME-Engine) 提交 Issue 和 Pull Request。
> 完整提交历史已保留在 Engine 中；本仓库保留历史代码、标签与已有 Release，供旧版本追溯和下载。
> 迁移来源见 [consolidation-sources.json](https://github.com/metasequoiaime/MSIME-Engine/blob/main/docs/consolidation-sources.json)。
>
> 以下为归档前的历史说明，当前构建与使用方式请以 Engine 中的文档为准。

# FanImeHelpCode

Helpcodes for [MetasequoiaImeTsf](https://github.com/metasequoiaime/MetasequoiaImeTsf).

所有辅助码文件统一放在 `helpcodes\` 目录下。当前 server 使用的方案和文件为：

- `lantian`：`helpcode.txt`（蓝天小雨点）
- `ziranma`：`zrm_helpcode_big_unique.txt`（自然码）
- `shouyou2_0`：`shouyou2_0_helpcode.txt`（首右2.0）
- `shouyouplus`：`shouyouplus_helpcode.txt`（首右plus）
- `xiaohe`：`xiaohe_helpcode.txt`（小鹤）

本地调试时，可以把整个目录链接到 server 的数据目录：

```powershell
$target = Join-Path $env:LOCALAPPDATA 'metasequoiaime\helpcodes'
if (Test-Path -LiteralPath $target) {
    Remove-Item -LiteralPath $target -Recurse -Force
}
New-Item -ItemType SymbolicLink -Path $target `
    -Target 'C:\Users\SonnyCalcr\EDisk\CppCodes\IMECodes\MetasequoiaImeHelpCode\helpcodes'
```

## 参考

- 自然码辅助码：<https://github.com/copperay/ZRM_Aux-code>
