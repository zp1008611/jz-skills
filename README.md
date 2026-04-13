# jz-skills

本项目用于开发和管理 jz  的 skill 文件。

## 开发流程

### 1. 克隆仓库

```bash
git clone https://github.com/zp1008611/jz-skills.git
cd jz-skills
```

### 2. 首次设置 dev 分支

如果是第一次开发，需要在本地创建并切换到 dev 分支：

```bash
# 创建并切换到本地 dev 分支（基于当前 main 分支）
git checkout -b dev
```

### 3. 日常开发流程

**重要：每次开发前，请先更新远程 dev 分支的内容，避免代码冲突。**

```bash
# 1. 切换到 dev 分支
git checkout dev

# 2. 拉取远程 dev 分支的最新内容
git pull origin dev

# 3. 进行 skill 文件开发...
# 编辑你的 skill 文件

# 4. 开发完成后，添加更改
git add .

# 5. 提交更改
git commit -m "描述本次修改内容"

# 6. 推送到远程 dev 分支
git push origin dev
```

### 4. 关键命令速查

| 操作 | 命令 |
|------|------|
| 切换分支 | `git checkout dev` |
| 更新远程代码 | `git pull origin dev` |
| 查看当前状态 | `git status` |
| 添加所有更改 | `git add .` |
| 提交更改 | `git commit -m "提交说明"` |
| 推送到远程 | `git push origin dev` |

## 注意事项

- **开发前务必先执行 `git pull origin dev`**，确保本地代码与远程保持同步
- 如果远程 dev 分支有更新但你本地也有修改，可能需要先解决冲突
- 如需将 dev 分支合并到 main，请创建 Pull Request 或在确认无误后手动合并
