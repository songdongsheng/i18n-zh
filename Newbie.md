#summary 新手向导
#labels Featured

## 目的 ##
> 致力于常用软件的中文化工作，推广自由软件。

## 新手向导 ##
  * 页面 [EditPoFilesWithVimOrEmacs](EditPoFilesWithVimOrEmacs.md) 说明了 Vim（详细）和 Emacs（简单）的用法
  * 页面 [GNOME](GNOME.md)                     说明了中文软件的翻译规范
  * 页面 [TP](TP.md)                        详细解释了 TP 的参与方法
  * 页面 [GeneratePo](http://code.google.com/p/i18n-zh/wiki/GeneratePO)                详细说明了从 pot 文件生成 po 文件的方法
  * 页面 [QuestionAndAnswer](QuestionAndAnswer.md)         告诉你错误出现时的处理方法
  * 页面 [TortoiseSVN\_Quick\_Guide](TortoiseSVN_Quick_Guide.md)   说明了 TortoiseSVN 的基本使用方法

## 类别 ##
  * i18n，即国际化，修改不支持 i18n 或支持不彻底的软件。
  * [l10n](L10n.md)，即[本地化](L10n.md)，翻译支持国际化的软件。有的软件翻译通过 [GNU Translation Project](http://translationproject.org/html/welcome.html)，不直接接收翻译成果，我们称之为 TP 软件。
  * [doc](Doc.md)，即[技术文档](Doc.md)翻译，包含 [svnbook](svnbook.md)，[TortoiseMerge](TortoiseMerge.md)，[TortoiseSVN](TortoiseSVN.md)，[DocBook](DocBook.md) 等文档。

## 工具 ##
> 页面 [Toolkit](Toolkit.md) 简要描述了可能用到的工具，以及如何获得这些工具。
  * i18n 需要 gcc 3.3/4.2, vs 98/2005 等开发工具。
  * [l10n](L10n.md) 需要 poedit，gettext 等工具。
  * [doc](Doc.md) 需要 Java SE， Python，python-libxml2，gettext，xsltproc，ant，fop，以及 poedit 等开发工具。

## 格式 ##
**希望你用不到这些方法**
> 大家可能用的翻译工具五花八门，例如文本编辑器，poedit，kbabel，或 gtranslator 等，它们的输出格式都不同，我们\*强烈建议\*你使用标准 gettext 格式。所以在你提交之前，请用 msgmerge 格式化 po 文件，假设有 foo.pot，zh\_CN.po 两个文件，方法如下：
```
    msgmerge --no-wrap -o zh_CN-new.po zh_CN.po foo.pot
    mv -f zh_CN-new.po zh_CN.po
```
> 或者请参看[合并不同的 po 文件](Merge.md)