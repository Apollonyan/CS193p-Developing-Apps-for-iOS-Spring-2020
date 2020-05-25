# 翻译校对步骤

> 1. 如果对已经翻译的字幕有意见或者建议，请通过 [新建 issue](https://github.com/Apollonyan/CS193p-Developing-Apps-for-iOS-Spring-2020/issues/new) 的方式反馈
> 2. 因为规则和往年变化较大，如果有什么意见和建议，欢迎使用 issue 提出，或是在群里讨论

首先，感谢您对翻译/校对字幕感兴趣。为了解决之前几年的问题，今年进行如下改革：

## 任务申领

0. 翻译的内容可能会被要求修改，甚至不被合并进入最终的字幕当中
1. 相关事宜将在 QQ 群 [639775967](https://qm.qq.com/cgi-bin/qm/qr?k=bbFbbt0CNs8lp5KegWf5dNMBiuYskt3v&authKey=SSRNAQTcd8lKGJb6bfx+LUz6tTZgaIZTO65ftpmSq7Kh0aN+ooLt2xUaFQML4rxX&noverify=0) 讨论，加群请备注 GitHub 用户名（如没有 QQ，Tel@ApolloZhu）
2. 翻译请通过编辑群内 [腾讯文档](https://docs.qq.com/sheet/DVnBxdUdKcUh0dldE?tab=p5e8m3) 的形式认领，并在群内通知
    1. 发消息的建议格式为：@自己 翻译第 X 集 Y - Z 条字幕
3. 申领翻译条数
    1. **注意：翻译、校对字幕的条数不是指字幕文件中行数，而是指**

        ```srt
        67 <----此处的数字
        00:03:04,860 --> 00:03:06,960
        we talked about the NSNumber format and all that.
        ```

    2. 需要翻译结束的那一条，并请将结束定在在自然语句结束的部分
    3. 第一次最多申领翻译 50 条（熟悉翻译流程，避免合并的时候需要修改的太多）
    4. 第二次翻译的内容合并，且总翻译条数超过 100 条之后，可在校对期间同时申领新的翻译
    5. 如果同时申领多个翻译任务，请合理使用 git 的分支功能避免新提交进入到之前的校对任务中
4. 请在自己定的截止日期前完成翻译，或在该日期之前自行转让任务给接班人
    1. 建议不超过 3 天，最长不超过一周
    2. 请结合个人情况进行估时，我个人的翻译速度约每小时 50 条
5. 为了避免其他人也翻译同样的内容：
    1. 请在任务申领文档中确认没有人申领了同样的部分
    2. 请只翻译申领的条数。如果您不小心翻译了其他部分，请在群里面沟通，避免重复劳动
7. **翻译一句后立刻** commit 并提交草稿 PR（[如何提交 Draft PR？](https://github.blog/2019-02-14-introducing-draft-pull-requests/)）
8. 翻译或校对的过程中有拿不准的地方（如这个词该不该翻译，该翻译成什么等），请在群内沟通

## 翻译方法

1. 请认真阅读并遵循 [翻译标准](./translation-style-guide.md)
2. Fork 本项目到您的账户下，然后 Clone 保存到本地
    1. 如果已经 fork 过了，请通过 sync/merge into/update from master/fetch origin 等方式完成同步
    2. 翻译过程中如无特殊情况请不要 update from master
3. 需要翻译的文件在 `subtitles/zh-Hans/` 文件夹中
4. srt 就是普通的文本文件，可以使用任何能够保存为同样格式的编辑器编辑
    1. 个人偏好是 Visual Studio Code
    2. 如果您有兴趣，也可以帮助开发 [Subtitle Editor](https://github.com/Apollonyan/Subtitle-Editor)
5. 翻译时需同时观看视频了解上下文，特别是无法理解的地方可以重复看视频
    1. 如果有可以同时看视频，编辑并保存 srt 的编辑器，请在群里讨论
6. 可以参考机器翻译的结果，但不能不加确认地使用
    1. 如果有放视频+编辑并保存 srt+提供机器翻译参考的编辑器，请在群里讨论
7. 建议每完成一部分就 commit 一次，这样我们能对进度有个大概的把握
8. **不要** 关闭/重复提交新 PR。你所有的 commit 都会自动加入到 pull request 里
9. （可选）校对结束后，你可以安全地删除 fork/分支/本地文件

## 初校方法

1. 所有校对应当以 [翻译标准](./translation-style-guide.md) 作为校对准则，并通过 Pull Request Review 的形式进行
2. Pull Request 如在 1 天内无人在评论区申领校对，将由 @ApolloZhu 执行
    1. 申领校对前请和 @ApolloZhu 单独沟通
    2. 翻译不得校对自己翻译的内容
    3. 校对者将被 assign 为 PR 的 reviewer
3. 校对期限为开始校对后 + max(翻译使用天数的一半, 一天)
4. 校对应当将字幕和视频一起观看，确认符合上下文，且在 b 站播放器中效果理想
5. 校对者可以直接 Approve，或提供建议的修改（suggest changes），但不得直接修改 PR 内容
    1. 如需要修改，翻译者需尽快更具提出的建议进行修改，最长不得超过一周
    2. 超过一周将视情况重新分配翻译，或进行其他调整
6. 如无其他问题，Pull Request 在 approve 后不超过一天内合并

## 精校方法

1. 因为每一集可能由多人翻译/校对，为保证最终字幕的统一性，（如无其他情况）将由 @ApolloZhu 在上传前最后检查
2. 如无特殊情况，校对时间不超过 3 天
3. 如由需要更改，由校对者直接执行，但需在原 PR 下通知翻译/校对，以便下次执行
4. 校对完成后发布 release，上传 bilibili
