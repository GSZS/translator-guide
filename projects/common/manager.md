## 管理员 操作指南（包括：任务管理、分支合并、校对审校）

* 将官方官网仓库 fork 到 docschina 下，将文档许可修改为 [“保留署名—非商用”创意共享 4.0 许可证（CC BY-NC 4.0）](https://creativecommons.org/licenses/by-nc/4.0/deed.zh) 授权方式
* 创建专用的 cn 翻译分支，在中文仓库 Setting -> Branches -> Default branch 中，将默认分支设置为 cn 分支
* 将网站运行起来
* 在 issues -> labels 中创建状态标签，一般分为：待翻译、翻译中、待校对、校对中、待审校、审校中、审校完成（可以参考 [webpack.js.org](https://github.com/webpack-china/webpack.js.org/labels) 的标签）。
* 统计文档情况，在 github 仓库的 `issues` 面板下（参考 [Babel](github.com/docschina/babeljs.io/projects/1)），创建对应的`子任务 issue`，在每个`子任务 issue` 中添加表示初始状态的`待翻译`标签，类似 JIRA/Worktile/Trello 的任务管理面板（多人协作情况下，单人维护的仓库可以省略认领流程）
* 创建`翻译词汇规范表 - 翻译部分 & 不翻译部分`来约定词语
* 邀请其他社区人员参与翻译项目
* 维护任务管理面板中任务的状态，例如，当有人在`子任务 issue` 中认领后，将 `待翻译` -> `翻译中`
* 合并 `上游英文仓库(upstream repository)` 更新
* 校对、审校、合并 `下游个人仓库(personal repository)` 向 `中游中文仓库(chinese repository)` 提交的 pr，维护贡献人员列表
* 联系 李成熙(@lcxfs1991) 和 李其昌(QC-L) 配置持续集成(CI)以自动部署网站（参考 [印记中文 & 腾讯云文档 CDN + COS 部署方案技术细节](https://github.com/lcxfs1991/blog/issues/22)）
* 部署成功后，添加相应的百度统计
* 联系 李志华(@dear-lizhihua)，在印记中文首页添加链接
