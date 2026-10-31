# 示例：一次你能亲眼看到的产品改动

本示例按照 Skill 的指引，查阅了 [Aspectory 的 v0.2.0 公开改动](https://github.com/LydiaTools/aspectory/commit/e749fd51e4e3bfed4e673a951964b2bb2b18aa96)、[发行说明](https://github.com/LydiaTools/aspectory/releases/tag/v0.2.0)和已有检查记录后撰写，不是独立的模型行为评测。

**你能看到什么变化：** 横图、方图、竖图现在可以放进同一画幅，图片完整显示，不会为了统一比例裁掉边缘。调整顺序后，可以一次下载带编号的 PNG 压缩包；原来的内容配图功能仍然保留。

**怎么自己检查：** 打开[批量保留整图](https://lydiatools.github.io/aspectory/carousel.html?lang=zh)，点击“试用示例图片”，选择 **4:5**，查看三张预览。用箭头调整顺序，再点“下载 PNG 压缩包”。内置示例是虚构图片，你也可以添加自己的 PNG、JPEG 或 WebP。

**已经检查过什么：** v0.2.0 的发行记录写明，13 项 Node 测试和本机 Chrome 检查通过，覆盖导出尺寸、图片边角、排序和离线导出。之后的 [CI 检查](https://github.com/LydiaTools/aspectory/actions/runs/40088687278)还使用了三张分别署名的 CC0 练习照片。这些是功能检查，不代表已经有人用它成功发布或获得流量。

![真实 Carousel Fit 页面：三张不同形状的练习照片完整放在统一的 4:5 画幅中。](https://raw.githubusercontent.com/LydiaTools/aspectory/c8293abbc337aacd733cae5ef0a19607995fa951/docs/screenshots/carousel-photos-zh.jpg)

*这是后来加入的 CC0 练习照片在实际应用中的截图，和工具内置的虚构示例不是同一组图片。工具通过缩放重采样把完整输入放进画幅。[照片署名与截图来源](https://github.com/LydiaTools/aspectory/blob/c8293abbc337aacd733cae5ef0a19607995fa951/docs/screenshots/PROVENANCE.md)。该截图晚于固定的 v0.2.0 发行包。*

**还需要你确认：** 发行记录没有宣称实机手机或 Safari 验收。导出后请在要发布的平台预览；这个功能负责整理画幅，不会替你发布。上述检查发生在 2026 年 10 月 24 日，不代表已经在你的设备上重新测试。
