# 翻译标准／校对规则 | Translation Standards (for Proofreading)

0. **重要**：因为 bilibili 支持的字幕分语言，今年翻译的字幕中只应该有中文，请替换掉现在文件里的英文字幕。
1. 如果我们从翻译阶段就能做到统一规范，相信校对也能事半功倍，尽快让观众能看上翻译的版本。
2. 请校对以下标准完成每一集的校对，并尽量确保每一集各个部分的翻译是统一的。
3. 欢迎大家根据实际情况，在群里讨论/issue 中提出修订意见

## 基本要求 | Basics

1. 请参与者 ***务必*** 对照原视频（字幕，若听力好可不看字幕）并结合视频中具体场景进行翻译和校对工作，请勿望文生义，切记不要生硬翻译
2. 如保持英文顺序会影响对应中文理解，为保观看者理解的流畅，应采用中文理解优先原则，优先按中文的表达方式断句
3. 注意代词的指代对象，区分“它”，“他”，“她”的使用，“其他”除外
4. 当说话者变更时，请加 `>>` 来区分。如：Question? >> Is it？ >> Yes.
5. 出现 Okay，All Right，Now 等语气词，请结合上下文选择合适的翻译，或直接省略不翻
6. 学生提问的部分如果听不清楚，字幕也不全（[INAUDIBLE]），但是老师回答时候把问题复述了一遍，字幕可译为 `>> [学生提问]`
7. 出现 [COUGH]，[LAUGH]，[NOISE]，[BLANK_AUDIO]，[INAUDIBLE] 等，请自行把握，可结合上下文选择省略不翻译
8. 卖萌请不要使用字符表情，比如（*3）看起来就像是备注；如果是标注说了三遍，请使用 x3 标记

## 格式要求 | Formatting

1. 不要合并多条 **字幕**，两条字幕之间保持一个空行
2. 字幕 **开头结尾** 均不留空格，并以 Unix 样式的 LF（Line Feed 的缩写，即 `\n`）换行
3. 省略字幕 **开头结尾** 不影响表意的标点。如省略如逗号、句号等，但可以保留问号
4. 除了 `[`，`]`，和 `>>` 以外使用全角中文标点。如果可能，使用中文数字
5. 保证每一条字幕中最多两行，且翻译不会过长（导致超过视频平台放映框最大长度）
    1. 如果字幕过长，可以按句中的标点符号分行
    2. 如分行后仍然有一行偏长，根据语义重新分行让上下两行长度接近
    3. （主观评判方法）：你作为观众看视频时候，会期望是什么样的？
6. 英文和阿拉伯数字同中文之间应当有一个空格
7. 如遇到英文词汇或阿拉伯数字和标点符号相邻的情况，则不需要再留空格

例：就算是最新的 iPad，也不能用 Swift Playgrounds 打包应用。

## 错误修正 | Fixing Erratum

1. 修改错别字，明显的笔误，大小写错误（如有时间，可修改 `subtitles/en` 文件夹下原英文字幕中的错误）
2. 如能找到对应的 Swift Evolution 编号，以类似（在 SE-0065 之前）……注明（比如今年课程中提到之后可以省略 `self` 的那个部分）
3. 如能确定特定的 Swift 语言版本，以类似（在 Swift 4 之前）……或（对于 Swift 3）……注明
4. 如果完全错误，尝试以类似……（误：原因）或（注：补充）说明。如空间不够，可适当调整上下文。参考 iOS 10 第三课 [420](https://github.com/ApolloZhu/Developing-iOS-10-Apps-with-Swift/blob/master/subtitles/3.%20More%20Swift%20and%20the%20Foundation%20Framework.srt#L2100) 和 [1304](https://github.com/ApolloZhu/Developing-iOS-10-Apps-with-Swift/blob/master/subtitles/3.%20More%20Swift%20and%20the%20Foundation%20Framework.srt#L6521)

## 翻译术语使用 | Terminology

### 术语的基本处理

1. 尽量和已翻译的内容保持一致，查阅 [术语翻译对照表](https://docs.qq.com/sheet/DVnBxdUdKcUh0dldE?c=B9A0B0)
2. 参考 [术语的特殊处理](#术语的特殊处理)
3. 参考 [Apple Developer 网页中文版](https://developer.apple.com/cn/)，比如有关 [SwiftUI](https://developer.apple.com/cn/xcode/swiftui/) 的介绍
4. 参考 [objccn 系列图书](https://objccn.io/products/) 的翻译
5. 参考历年来 [iOS 8](https://github.com/X140Yu/Developing_iOS_8_Apps_With_Swift)，[iOS 9](https://github.com/SwiftGGTeam/Developing-iOS-9-Apps-with-Swift)，[iOS 10](https://github.com/Apollonyan/Developing-iOS-10-Apps-with-Swift) 和 [iOS 11](https://github.com/Apollonyan/Developing-iOS-11-Apps-with-Swift) 的翻译
6. 查阅 [《The Swift Programming Language》中文版](https://swiftgg.gitbook.io/swift/) 及其 [术语表](https://github.com/SwiftGGTeam/the-swift-programming-language-in-chinese#%E6%9C%AF%E8%AF%AD%E8%A1%A8) 对 Swift 语言相关名词的翻译
7. 参考 [CocoaChina 代码库](http://code.cocoachina.com/) 对 UI 控件的翻译
8. 参考该术语在其它编程语言中的翻译，可以使用 [微软官方术语搜索](https://www.microsoft.com/Language/zh-cn/Search.aspx) 等搜索引擎
9. 如果以上都没有找到合适的结果，你可以在群里面讨论是使用英文原文还是其他合适的翻译

### 术语的特殊处理

1. 如果想在同时翻译并保留原文，请用括号（中文）补充。
    - 例：MVC，即 Model（模型）-View（视图）-Controller（控制器）
2. 不翻译通用的名称，如 MVC，iPhone，Xcode，storyboard 等
3. 不翻译直接引用的代码，包括但不限于：
    - Swift 语言关键字：如 `true`，`false` 等
    - 类／结构体／元组类型的名称：如 `Button`，`String` 等
    - 项目中的代码：如 `var description` 等
