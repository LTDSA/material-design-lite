
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

如果您对如何使用Material Design Lite有疑问，请将它们指向[StackOverflow] [stackoverflow]并使用`material-design-lite`标签。 我们也可以在GitHub问题上找到它们。

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
如果您在源代码中发现错误或文档中存在错误，您可以通过向我们的[GitHub存储库][github]提交问题来帮助我们。更好的是你可以提交一个Pull Request
修复。

See [below](#submit) for some guidelines.

## <a name="feature"></a> 想要一个功能？
You can request a new feature by submitting an issue to our [GitHub Repository][github].

Here is a template to get you started:

```
这是一个新组件，还是现有组件中缺少的功能？
组件名称：
组件的Material Design规范URL（如果有）：

这个组件或功能允许您做什么，目前是不可能的？

请提供您可能遇到的此组件或功能的良好使用示例的任何URL或屏幕截图。
```

If you would like to implement a new feature then consider what kind of change it is:

* **Major Changes** that you wish to contribute to the project should be discussed first on our
[issue tracker][] so that we can better coordinate our efforts, prevent
duplication of work, and help you to craft the change so that it is successfully accepted into the
project.
* **Small Changes** can be crafted and submitted to the [GitHub Repository][github] as a Pull Request.

## <a name="submit"></a> Submission Guidelines

### 提交问题
Before you submit your issue search the archive, maybe your question was already answered.

If your issue appears to be a bug, and hasn't been reported, open a new issue.
Help us to maximize the effort we can spend fixing issues and adding new
features, by not reporting duplicate issues.  Providing the following information will increase the
chances of your issue being dealt with quickly:

* **Overview of the Issue** - if an error is being thrown a non-minified stack trace helps
* **Motivation for or Use Case** - explain why this is a bug for you
* **Material Design Lite Version(s)** - is it a regression?
* **Browsers and Operating System** - is this a problem with all browsers or only IE9?
* **Reproduce the Error** - provide a live example (using JSBin) or a unambiguous set of steps.
* **Related Issues** - has a similar issue been reported before?
* **Suggest a Fix** - if you can't fix the bug yourself, perhaps you can point to what might be
  causing the problem (line of code or commit)

**If you get help, help others. Good karma rulez!**

Here's a template to get you started:

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
Before you submit your pull request consider the following guidelines:

* Search [GitHub](https://github.com/google/material-design-lite/pulls) for an open or closed Pull Request
  that relates to your submission. You don't want to duplicate effort.
* Please sign our [Contributor License Agreement (CLA)](#cla) before sending pull
  requests. We cannot accept code without this.
* Make your changes in a new git branch:

     ```shell
     git checkout -b my-fix-branch master
     ```

* Create your patch, **including appropriate test cases**.
* Follow our [Coding Rules](#rules).
* Run the full Material Design Lite test suite (`gulp test`),
  and ensure that all tests pass.
* Avoid checking in files that shouldn't be tracked (e.g `node_modules`, `gulp-cache`, `.tmp`, `.idea`). We recommend using a [global .gitignore](https://help.github.com/articles/ignoring-files/#create-a-global-gitignore) for this.
* Make sure **not** to include a recompiled version of the files found in `/css` and `/js` as part of your PR. We will generate these automatically.
* Commit your changes using a descriptive commit message.

     ```shell
     git commit -a
     ```
  Note: the optional commit `-a` command line option will automatically "add" and "rm" edited files.

* Build your changes locally to ensure all the tests pass:

    ```shell
   gulp
    ```

* Push your branch to GitHub:

    ```shell
    git push origin my-fix-branch
    ```

* In GitHub, send a pull request to `material-design-lite:master`.
* If we suggest changes then:
  * Make the required updates.
  * Re-run the Material Design Lite test suite to ensure tests are still passing.
  * Rebase your branch and force push to your GitHub repository (this will update your Pull Request):

    ```shell
    git rebase master -i
    git push origin my-fix-branch -f
    ```

That's it! Thank you for your contribution!

#### 合并拉取请求后

After your pull request is merged, you can safely delete your branch and pull the changes
from the main (upstream) repository:

* Delete the remote branch on GitHub either through the GitHub web UI or your local shell as follows:

    ```shell
    git push origin --delete my-fix-branch
    ```

* Check out the master branch:

    ```shell
    git checkout master -f
    ```

* Delete the local branch:

    ```shell
    git branch -D my-fix-branch
    ```

* Update your master with the latest upstream version:

    ```shell
    git pull --ff upstream master
    ```

## <a name="rules"></a> 编码规则

We generally follow the [Google JavaScript style guide][js-style-guide] with a few minor exceptions documented in our [JSCS configuration][jscs-config].

[JSCS](http://jscs.info) is a tool for linting code against a style guide and has plugins available for both editors and build tools. Should
you find that you would prefer to automatically format your code to match our style guide, you can use the JSCS [autoformatting][autoformatting]
feature.

## <a name="cla"></a> 签署CLA

Please sign our Contributor License Agreement (CLA) before sending pull requests. For any code
changes to be accepted, the CLA must be signed. It's a quick process, we promise!

* For individuals we have a [simple click-through form][individual-cla].
* For corporations we'll need you to
  [print, sign and one of scan+email, fax or mail the form][corporate-cla].

*This guide was inspired by the [AngularJS contribution guidelines](https://github.com/angular/angular.js/blob/master/CONTRIBUTING.md).*

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
