# 翻译校对步骤

> 如果对已经翻译的字幕有意见或者建议，请通过 [新建 issue](https://github.com/Apollonyan/CS193p-Developing-Apps-for-iOS-Spring-2020/issues/new) 的方式反馈。

首先，感谢您对翻译/校对字幕感兴趣。为了解决之前几年的问题，今年进行如下改革：

## 任务分配

1. 相关事宜将在 QQ 群 [639775967](https://qm.qq.com/cgi-bin/qm/qr?k=bbFbbt0CNs8lp5KegWf5dNMBiuYskt3v&authKey=SSRNAQTcd8lKGJb6bfx+LUz6tTZgaIZTO65ftpmSq7Kh0aN+ooLt2xUaFQML4rxX&noverify=0) 讨论，加群请备注 GitHub 用户名。（如果没有 QQ，Tel@ApolloZhu）
2. 翻译请通过 [新建 issue](https://github.com/Apollonyan/CS193p-Developing-Apps-for-iOS-Spring-2020/issues/new?labels=%E7%BF%BB%E8%AF%91%E4%B8%AD&template=translate.md&title=%E7%BF%BB%E8%AF%91+X+%E9%9B%86+Y+-+Z+%E6%AE%B5%E5%AD%97%E5%B9%95) 的形式认领，根据模版
3. 任务分配后看板会自动更新，@ApolloZhu 会在 [README](README.md) 中更新任务分配情况

## 翻译方法



1.
2. 在正式提交之前，需要先翻译

   2.
   2. 每次校对不得超过 3 天

## 初校方法

1. 所有校对将通过 Pull Request Review 的形式进行。
2. Pull Request 1 天内无人申领校对，将由 @ApolloZhu 执行。
   1. 申领校对前请和 @ApolloZhu 单独沟通。
   2. 翻译不得校对自己翻译的内容。
3. 校对期限为开始校对后 + max(翻译使用天数的一半, 一天)。
4. 校对者可以直接 Approve，或提供建议的修改（suggest changes），但不得直接修改 PR 内容。
   1. 如需要修改，翻译者需尽快更具提出的建议进行修改，最长不得超过一周。
   2. 超过一周将视情况重新分配翻译，或进行其他调整。
5. Pull Request 在 approve 后

## 精校方法

1. 因为每一集可能由多人翻译/校对，为保证最终字幕的统一性，将由 @ApolloZhu 在上传前最后检查。
2. 如无特殊情况，校对时间不超过 3 天。
3. 如由需要更改，由校对者直接执行，但需在原 PR 下通知翻译/校对，以便下次执行。
4. 校对完成后发布 release，上传 bilibili。

## 领取任务

1. 每节新内容发布以后，[issue 区](https://github.com/Apollonyan/Developing-iOS-11-Apps-with-Swift/issues) 会开一个当节的「任务分配」issue。
2. ***请确认不和他人重复之后*** ，到每节的 issue 中评论「翻译」或「校对」。评论的内容包括：
    1. 段数。建议选择 issue 下第一条里公布的，一般会是 300 或 500 段，也可以自定义。
    2. 预计完成时间。我个人的翻译速度是每小时 50 段，请结合个人情况进行估计，建议控制在一个星期以内。海外党请用本地时，并注明时区。

**翻译、校对任务的段数不是指字幕文件中行数，而是指**

    67 <----此处的数字
    00:03:04,860 --> 00:03:06,960
    we talked about the NSNumber format and all that.

## 进行翻译

1. 请认真阅读并遵守 [翻译标准／校对规则](./translation-style-guide.md)。
2. 为了避免其他人也翻译同样的内容，请只翻译分配的段数。如果您不小心翻译了其他部分，请立刻告诉我，避免重复劳动。
3. 如果忙碌或者有困难一定要及时提出来，我也可以把任务转给其他人。这并不会对您有任何影响，觉得难为情可以邮件/私信我。
4. Fork 本项目到您的账户下，然后 Clone 保存到本地。
5. 如果已经 fork 过了，请通过 sync/update from master/fetch origin 等方式完成同步。
6. 翻译过程中请不要 update from master。
7. 翻译 **subtitles** 文件夹下对应 srt 文件的对应段，在英文行下面添加中文翻译。
    - srt 就是普通的文本文件，所以使用的程序只要能够保证保存为同样格式就行，个人偏好是 Visual Studio Code，也可以直接在 GitHub 上编辑。
    - 千万 **不要** 翻译 en/subtitles 文件夹里的，那些是保留原版字幕以备后用。区别方法如下：
        - 要翻译的文件所有的英文都只有一行；
        - 要翻译的文件至少第一句和最后一句都已经翻译过了。
8. 建议每完成一部分就 **commit** 一次，这样我们能对进度有个大概的把握。
9. 翻译或校对的过程中有拿不准的地方，请先尝试按照标准里提到的方法解决，也可以进入该节的 issue 中讨论（如这个词该不该翻译，该翻译成什么等）。

## 提交翻译

1. **全部** 翻译完之后提交 pull request，你会看到它出现在 [这里](https://github.com/Apollonyan/Developing-iOS-11-Apps-with-Swift/pulls)，具体步骤可以参考 [教程](https://help.github.com/articles/creating-a-pull-request-from-a-fork/)。
2. 如果有，请在提交信息中注明我们需要特别注意的地方，和其他任务行之外的改动。
3. 为了加快进度，我们会采用每一集整体校对的形式，所以我们基本会马上 merge 你的 pull request。
4. 如果翻译格式不正确，或是有严重问题等，我们会在 pull request 的 comment 里提出，请修改并 commit。（不需要关闭 pull request，所有的 commit 会自动加入 pull request 里）
5. 在看到主项目出现一个标题为 `集数_开始段-结束段 翻译 @你` 的 commit 之后就算完成了。如果有需要，这个时候就可以安全地删除 fork 和本地文件了。

----

本规则基于 [github.com/SwiftGGTeam/Developing-iOS-9-Apps-with-Swift/issues/3](https://github.com/SwiftGGTeam/Developing-iOS-9-Apps-with-Swift/issues/3) 修订而成。
