# 翻译校对步骤

> 1. 如果对已经翻译的字幕有意见或者建议，请通过 [新建 issue](https://github.com/Apollonyan/CS193p-Developing-Apps-for-iOS-Spring-2020/issues/new) 的方式反馈
> 2. 因为规则和往年变化较大，如果有什么意见和建议，欢迎使用 issue 提出，或是在群里讨论

首先，感谢您对翻译/校对字幕感兴趣。为了解决之前几年的问题，今年进行如下改革：

## 任务申领

1. 相关事宜将在 QQ 群 [639775967](https://qm.qq.com/cgi-bin/qm/qr?k=bbFbbt0CNs8lp5KegWf5dNMBiuYskt3v&authKey=SSRNAQTcd8lKGJb6bfx+LUz6tTZgaIZTO65ftpmSq7Kh0aN+ooLt2xUaFQML4rxX&noverify=0) 讨论，加群请备注 GitHub 用户名（如没有 QQ，Tel@ApolloZhu）
2. 翻译请通过 **新建 issue** 的形式认领，认领时请完整填写模版中的内容（及标题）
    1. 第一次最多申领翻译 50 条（熟悉翻译流程，避免合并的时候需要修改的太多）
    2. 第二次翻译的内容合并之后，可在校对期间同时申领新的翻译
    3. 如果同时申领多个翻译任务，请合理使用 git 的分支功能避免新提交进入到之前的校对任务中
3. 任务申领后 [看板](https://github.com/Apollonyan/CS193p-Developing-Apps-for-iOS-Spring-2020/projects/1) 会自动更新，@ApolloZhu 会在一天内更新 [README](README.md) 中任务分配情况
4. 为了避免其他人也翻译同样的内容，请只翻译申领的条数。如果您不小心翻译了其他部分，请在群里面沟通，避免重复劳动
5. 翻译或校对的过程中有拿不准的地方（如这个词该不该翻译，该翻译成什么等），请在群内沟通
6. **注意：翻译、校对字幕的条数不是指字幕文件中行数，而是指**

        67 <----此处的数字
        00:03:04,860 --> 00:03:06,960
        we talked about the NSNumber format and all that.

## 翻译方法

1. 请认真阅读并遵守 [翻译标准](./translation-style-guide.md)
2. Fork 本项目到您的账户下，然后 Clone 保存到本地
    1. 如果已经 fork 过了，请通过 sync/update from master/fetch origin 等方式完成同步
    2. 翻译过程中如无特殊情况请不要 update from master
3. 需要翻译的文件在 `subtitles/zh-Hans/` 文件夹中
4. srt 就是普通的文本文件，可以使用任何能够保存为同样格式的编辑器编辑
    1. 个人偏好是 Visual Studio Code
5. 翻译时需同时观看视频了解上下文，特别是无法理解的地方可以重复看视频
    1. 如果有可以同时看视频，编辑并保存 srt 的编辑器，请在群里讨论
6. 可以参考机器翻译的结果，但不能不加确认地使用
    1. 如果有放视频+编辑并保存 srt+提供机器翻译参考的编辑器，请在群里讨论
7. **翻译一句后立刻** commit 并提交草稿 PR。（[如何提交 Draft PR？](https://github.blog/2019-02-14-introducing-draft-pull-requests/)）
8. 建议每完成一部分就 commit 一次，这样我们能对进度有个大概的把握
9. 不要重复关闭/提交新 PR。你所有的 commit 都会自动加入到 pull request 里
10. （可选）校对结束后，你可以安全地删除 fork/分支/本地文件

## 初校方法

1. 所有校对应当以 [翻译标准](./translation-style-guide.md) 作为校对准则，并通过 Pull Request Review 的形式进行
2. Pull Request 如在 1 天内无人在评论区申领校对，将由 @ApolloZhu 执行
    1. 申领校对前请和 @ApolloZhu 单独沟通
    2. 翻译不得校对自己翻译的内容
    3. 校对者将被 assign 为 PR 的 reviewer
3. 校对期限为开始校对后 + max(翻译使用天数的一半, 一天)
4. 校对者可以直接 Approve，或提供建议的修改（suggest changes），但不得直接修改 PR 内容
    1. 如需要修改，翻译者需尽快更具提出的建议进行修改，最长不得超过一周
    2. 超过一周将视情况重新分配翻译，或进行其他调整
5. 如无其他问题，Pull Request 在 approve 后不超过一天内合并

## 精校方法

1. 因为每一集可能由多人翻译/校对，为保证最终字幕的统一性，（如无其他情况）将由 @ApolloZhu 在上传前最后检查
2. 如无特殊情况，校对时间不超过 3 天
3. 如由需要更改，由校对者直接执行，但需在原 PR 下通知翻译/校对，以便下次执行
4. 校对完成后发布 release，上传 bilibili
