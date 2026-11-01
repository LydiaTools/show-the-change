# 示例：安装说明变清楚了

下面的说明根据[公开 README 改动](https://github.com/LydiaTools/claude-session-image-audit/commit/8e469db6d35f80e3c20ec0c242b07e64cb49f780)和已有检查记录撰写，用来展示解释方式，并非模型评测。

**你能看到的变化：** 图片审计工具的 README 增加了直接安装已有 v0.1.0 预览包的命令，以及不会扫描文件的帮助命令；还说明虚构示例文件在源码中，不在安装包里。这次改动只修改说明，没有改变工具功能，也没有发布新包。

**你去哪里看：** 打开[更新后的快速开始](https://github.com/LydiaTools/claude-session-image-audit/blob/8e469db6d35f80e3c20ec0c242b07e64cb49f780/README.md#quick-start)；[v0.1.0 发布页](https://github.com/LydiaTools/claude-session-image-audit/releases/tag/v0.1.0)可下载安装包并查看校验值。

**已经检查：** 维护者在临时 Python 3.10 环境中安装公开下载包并运行虚构样本，又单独克隆 v0.1.0 源码运行示例；两次联网使用进程级代理。README 改动的[自动测试](https://github.com/LydiaTools/claude-session-image-audit/actions/runs/41255834866)通过。

**还不能据此判断：** 这不能证明 Skill 独立生成了这段说明、真实用户会话已被检查，或工具能诊断 API 错误。固定 v0.1.0 安装包早于本次 README 更新；新说明在项目页面。本示例位于 Show the Change 当前源码，先前发布的 v0.1.1 ZIP 不包含本示例。
