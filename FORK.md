# Fork 说明

本仓库是 [cmliu/edgetunnel](https://github.com/cmliu/edgetunnel) 的个人 Fork，用于个人部署与测试。

## 🔄 同步机制

- 上游仓库：`https://github.com/cmliu/edgetunnel.git`
- 同步工作流：`.github/workflows/sync.yml`，每天 `00:00 UTC` 自动执行，也可在 Actions 页面手动触发。
- 同步策略：本地无改动时直接对齐上游；本地有改动时以 merge 方式保留本地修改；若产生冲突则暂停同步并提示手动处理。

## 🛠️ 维护约定

- 个性化修改尽量落在新增文件中，降低与上游同一位置的冲突概率。
- 需要手动同步时：

  ```bash
  git fetch upstream
  git merge upstream/main
  ```
