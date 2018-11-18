
# 为Material Design Lite做贡献

我们很乐意为您贡献我们的源代码，让Material Design Lite比现在更好！ 以下是我们希望您遵循的指南：

 - [行为守则](#coc)
 - [疑问或问题？](#question)
 - [问题和错误](#issue)
 - [功能请求](#feature)
 - [提交指南](#submit)
 - [编码规则](#rules)
 - [签署CLA](#cla)

## <a name="coc"></a> 行为守则

作为Material Design Lite项目的贡献者和维护者，我们承诺通过发布问题，更新文档，提交拉取请求，提供评论反馈以及任何其他活动来尊重所有贡献者。

通过任何Material Design Lite的渠道（GitHub、StackOverflow、Google +、Twitter等）进行交流必须具有建设性，不得诉诸于人身攻击，拖钓，公共或私人骚扰，侮辱或其他非专业行为。

无论性别、性别认同、性取向、残疾、年龄、种族、民族、宗教或经验水平如何，我们承诺向参与该项目的每个人提供礼貌和尊重。我们希望任何有助于Material Design Lite项目的人都这样做。

如果社区的任何成员违反了此行为准则，Material Design Lite项目的维护者可以采取行动，删除问题，评论和PR或阻止帐户视为合适。

如果您受到或目击不可接受的行为或有任何其他疑虑，请发送电子邮件至addyo@google.com。

## <a name="question"></a> 有疑问或问题？

如果您对如何使用Material Design Lite有疑问，请将它们指向[StackOverflow][stackoverflow]并使用`material-design-lite`标签。 我们也可以在GitHub问题上找到它们。

如果您觉得我们错过了一些重要的文档，请随意提出问题，以便我们提供帮助。 这是一个让你入门的例子：

```
组件（如果有）：

您想做什么或了解更多信息？

您在哪里看？

您希望在哪里找到这些信息？
```

或者，如果您正在寻找新的设计模板：

```
请提供您正在寻找的模板的简短摘要。

是什么让这个模板从设计角度来看有趣或具有挑战性？

请提供您可能遇到的此类网页的良好示例的任何网址。
```

## <a name="issue"></a> 发现了一个问题？
如果您在源代码中发现错误或文档中存在错误，您可以通过向我们的[GitHub存储库][github]提交问题来帮助我们。更好的是你可以提交一个拉取请求修复。

请参阅[下面](#submit)的一些指南。

## <a name="feature"></a> 想要一个功能？
您可以通过向我们的[GitHub存储库][github]提交问题来请求新功能。

这是一个可以帮助您入门的模板：

```
这是一个新组件，还是现有组件中缺少的功能？
组件名称：
组件的Material Design规范URL（如果有）：

这个组件或功能允许您做什么，目前是不可能的？

请提供您可能遇到的此组件或功能的良好使用示例的任何URL或屏幕截图。
```

如果您想要实现新功能，请考虑它是什么样的更改：

* **主要变更** 您希望为项目做出贡献的主要变更应首先在我们的[问题跟踪器][]上进行讨论，以便我们能够更好地协调我们的工作，防止重复工作，并帮助您制定变更，以便成功接受项目。
* **小更改** 可以制作小更改并将其作为拉取请求提交给[GitHub存储库][github]。

## <a name="submit"></a> 提交指南

### 提交问题
在您提交问题之前搜索存档，也许您的问题已经得到解答。

如果您的问题似乎是一个错误，并且尚未报告，请打开一个新问题。
通过不报告重复问题，帮助我们最大限度地减少修复问题和添加新功能所需的工作量。 提供以下信息将增加您快速处理问题的机会：

* **问题概述** - 如果抛出错误，则非缩小堆栈跟踪会有所帮助
* **动机或用例** - 解释为什么这是您的错误
* **Material Design Lite版本** - 它是回归吗？
* **浏览器和操作系统** - 这是所有浏览器还是只有IE9的问题？
* **重现错误** - 提供一个实例（使用JSBin）或一组明确的步骤。
* **相关问题** - 有没有报道过类似的问题？
* **建议修复** - 如果你不能自己修复bug，也许你可以指出可能导致问题的原因（代码行或提交）

**如果你得到帮助，请帮助他人。好业力统治！**

这是一个让您入门的模板：

```
MDL版本：
浏览器：
浏览器版本：
操作系统：
操作系统版本：
URL，如果适用（您可以使用[codepen作为起点] [http://codepen.io/pen/def?fork=xGWgXa]）：

哪些步骤将重现该问题：
1、
2、
3、

预期结果是什么？

会发生什么而不是那个？

请在下面提供任何其他信息，并在可能的情况下附上屏幕截图。
```

### 提交拉取请求
在提交拉取请求之前，请考虑以下准则：

* 在[GitHub](https://github.com/google/material-design-lite/pulls)中搜索与您的提交相关的开放或已关闭的拉取请求。您不想重复努力。
* 请在发送拉取请求之前签署我们的[贡献者许可协议（CLA）](#cla)。 没有这个我们不能接受代码。
* 在新的git分支中进行更改：

     ```shell
     git checkout -b my-fix-branch master
     ```

* 创建补丁，**包括适当的测试用例**。
* 按照我们的[编码规则](#rules)。
* 运行完整的Material Design Lite测试套件（`gulp test`），并确保所有测试都通过。
* 避免检入不应被跟踪的文件（例如`node_modules`，`gulp-cache`，`。tmp`，`.idea`）。 我们建议使用[global .gitignore](https://help.github.com/articles/ignoring-files/#create-a-global-gitignore)。
* 确保**不要**在`/css`和`/js`中包含重新编译的文件版本作为PR的一部分。 我们将自动生成这些。
* 使用描述性提交消息提交更改。

     ```shell
     git commit -a
     ```
  注意：可选的commit`-a`命令行选项将自动“添加”和“移除”编辑的文件。

* 在本地构建更改以确保所有测试都通过：

    ```shell
   gulp
    ```

* 将您的分支推送到GitHub：

    ```shell
    git push origin my-fix-branch
    ```

* 在GitHub中，向`material-design-lite：master`发送一个拉取请求。
* 如果我们建议更改：
  * 进行必要的更新。
  * 重新运行Material Design Lite测试套件以确保测试仍在通过。
  * 重新启动您的分支并强制推送到您的GitHub存储库（这将更新您的拉取请求）：

    ```shell
    git rebase master -i
    git push origin my-fix-branch -f
    ```

就是这样！感谢您的贡献！

#### 合并拉取请求后

合并拉取请求后，您可以安全地删除分支并从主（上游）存储库中提取更改：

* 通过GitHub Web UI或本地shell删除GitHub上的远程分支，如下所示：

    ```shell
    git push origin --delete my-fix-branch
    ```

* 查看主分支：

    ```shell
    git checkout master -f
    ```

* 删除本地分支：

    ```shell
    git branch -D my-fix-branch
    ```

* 使用最新的上游版本更新您的主服务器：

    ```shell
    git pull --ff upstream master
    ```

## <a name="rules"></a> 编码规则

我们通常遵循[Google JavaScript样式指南][js-style-guide]，我们的[JSCS配置][jscs-config]中记录了一些小的例外情况。

feature.[JSCS](http://jscs.info)是一个用于根据样式指南绘制代码的工具，并且具有可用于编辑器和构建工具的插件。 如果您发现自己希望自动格式化代码以匹配我们的样式指南，则可以使用JSCS [autoformatting][autoformatting]功能。

## <a name="cla"></a> 签署CLA

在发送拉取请求之前，请签署我们的贡献者许可协议（CLA）。 要接受任何代码更改，必须签署CLA。 这是一个快速的过程，我们保证！

* 对于个人，我们有[简单的点击表格][individual-cla]。
* 对于公司，我们需要您[打印，签名以及扫描+电子邮件，传真或邮寄表格][corporate-cla]。

*本指南的灵感来自[AngularJS贡献指南](https://github.com/angular/angular.js/blob/master/CONTRIBUTING.md)。*

[github]: https://github.com/google/material-design-lite
[issue tracker]: https://github.com/google/material-design-lite/issues
[individual-cla]: http://code.google.com/legal/individual-cla-v1.0.html
[corporate-cla]: http://code.google.com/legal/corporate-cla-v1.0.html
[js-style-guide]: http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml
[jsbin]: http://jsbin.com/
[stackoverflow]: http://stackoverflow.com/questions/tagged/material-design-lite
[global-gitignore]: https://help.github.com/articles/ignoring-files/#create-a-global-gitignore
[autoformatting]: https://medium.com/@addyosmani/auto-formatting-javascript-code-style-fe0f98a923b8
[jscs-config]: https://github.com/google/material-design-lite/blob/master/.jscsrc
