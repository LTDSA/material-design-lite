# Material Design Lite

[![GitHub version](https://badge.fury.io/gh/google%2Fmaterial-design-lite.svg)](https://badge.fury.io/gh/google%2Fmaterial-design-lite)
[![npm version](https://badge.fury.io/js/material-design-lite.svg)](https://badge.fury.io/js/material-design-lite)
[![Bower version](https://badge.fury.io/bo/material-design-lite.svg)](https://badge.fury.io/bo/material-design-lite)
[![Gitter version](https://img.shields.io/gitter/room/gitterHQ/gitter.svg)](https://gitter.im/google/material-design-lite)
[![Dependency Status](https://david-dm.org/google/material-design-lite.svg)](https://david-dm.org/google/material-design-lite)

> 在vanilla CSS、JS和HTML中实现[Material Design](http://www.google.com/design/spec/material-design/introduction.html)组件。

Material Design Lite（MDL）允许您为静态内容网站添加Material Design外观。 它不依赖于任何JavaScript框架或库。 针对跨设备使用进行了优化，在旧版浏览器中优雅地降级，并提供从一开始就可以访问的体验。

> ### 有限的支持

> Material Design Lite目前在有限的支持下，开发已经转移到了
> [web的Material组件](https://github.com/material-components/material-components-web)存储库。

> 核心团队在MDL中没有进一步的发展，但我们很高兴审查PR，修复关键错误和
> 推出新版本。不接受任何重大变化。

## 在您的网站上使用MDL？

**本文档面向将参与或编译的开发人员
MDL。 如果您希望在您的网站或网络应用程序上使用MDL，请前往
[getmdl.io](http://getmdl.io).**

## 浏览器支持


| IE9 | IE10 | IE11 | Chrome | Opera | Firefox | Safari | Chrome（Android） | 移动Safari |
|-----|------|------|--------|-------|---------|--------|-------------------|-----------|
| B   | A    | A    | A      | A     | A       | A      | A                 | A         |

完全支持A级浏览器。 B级浏览器会优雅地降级到我们仅使用CSS的体验。

### 下载/克隆

使用Git克隆存储库：

```bash
git clone https://github.com/google/material-design-lite.git
```

或者，您可以[下载](https://github.com/google/material-design-lite/archive/master.zip)此存储库。

Windows用户，如果由于行结尾而无法编译，请确保
配置git以使用`lf`（unix）行结尾检出存储库。 这个
可以通过设置`core.eol`来实现。

```bash
git config core.eol lf
git config core.autocrlf input
git rm --cached -r .
git reset --hard
```

> 请记住，主分支被认为是不稳定的。 不要使用它生产。 使用存储库、npm或bower的标记状态来确保稳定性！

## 功能请求

MDL目前处于有限的支持模式，核心团队没有进一步的开发。
我们很高兴接受并审查对新功能的拉取请求，只要没有中断变化。

## 想贡献？

如果您发现了错误、有任何疑问或想要贡献。 关注我们的
[指南](https://github.com/google/material-design-lite/blob/mdl-1.x/CONTRIBUTING.md)，并帮助改进Material Design Lite。 
有关更多信息，请访问我们的[wiki](https://github.com/google/material-design-lite/wiki)。

请使用默认分支`mdl-1.x`。

请注意，[web的Material组件](https://github.com/material-components/material-components-web)，即MDL v2，处于早期Alpha阶段（这意味着一切都是移动目标，我们可以随时改变任何事情）。谨慎使用。

但是，我们绝对喜欢让人们测试MCW并提供有关使用它的经验的反馈，特别是与其他框架和库集成。

## 许可证

© Google，2015。根据[Apache-2](https://github.com/google/material-design-lite/blob/master/LICENSE)许可证获得许可。
