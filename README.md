
# GitHub Actions PAT_TOKEN 配置和生成步骤

## 1. 确认 PAT_TOKEN 的权限
确保你在 GitHub 仓库的 Secrets 中配置的 PAT_TOKEN 具备以下必要权限：

- **repo** 权限：允许对仓库进行推送、更改等操作。
- **workflow** 权限：允许管理工作流运行记录（与 `Mattraks/delete-workflow-runs@v2` 相关）。

### 生成新的 Token：
1. 前往 [GitHub 的个人访问令牌页面](https://github.com/settings/tokens)。
2. 点击 **"Generate new token"**。
3. 选择所需的权限（`repo` 和 `workflow`）。
4. 生成并复制 Token。

## 2. 更新 GitHub Secrets
1. 进入你的 GitHub 仓库主页。
2. 点击 **Settings** > **Secrets and variables** > **Actions**。
3. 在 **Secrets** 中找到现有的 `PAT_TOKEN`，如果没有，可以新建。
4. 将刚刚生成的新的 Token 粘贴到 `PAT_TOKEN` 中并保存。
