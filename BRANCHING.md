# 分支策略

这个仓库采用 `main + feature/*` 的轻量分支模型。

## 分支约定

- `main`：稳定主分支，只接受已经验证过、准备保留的内容。
- `feature/*`：日常工作分支，用于新增、修改、整理文档或页面。
- `fix/*`：可选，用于明确的修复类改动。

## 工作流

1. 从 `main` 拉出新分支。
2. 在 `feature/*` 上完成改动。
3. 先本地检查，再提交。
4. 合并回 `main` 前尽量经过一次人工复核。

## 命名建议

- 新功能或新增内容：`feature/add-xxx`
- 文档整理：`feature/docs-xxx`
- 页面改版：`feature/ui-xxx`
- 修复问题：`fix/xxx`

## 提交建议

- 每次提交只做一件事。
- 提交信息尽量短，能看出改了什么。
- 示例：`docs: add branch policy`

## 安全建议

- 不要直接在 `main` 上做大改动。
- 避免把未确认的临时文件一起提交。
- 如果一次改动范围很大，先拆成多个 `feature/*` 分支。

## 推荐命令

```bash
git switch -c feature/docs-branch-policy
git add BRANCHING.md
git commit -m "docs: add branch policy"
```
