#summary 文档翻译首页

# 简介 #

  * 新手参见 [Newbie](Newbie.md)
  * 使用的工具参见 [Toolkit](Toolkit.md)
  * 翻译流程和校对参见 [Flow](Flow.md)

# 翻译信息 #
  * [TortoiseMerge](TortoiseMerge.md)
  * [TortoiseSVN](TortoiseSVN.md)
  * [Version Control with Subversion](svnbook.md)
  * [DocBook 5.0: The Definitive Guide](DocBook.md)
  * [DocBook: The Definitive Guide>DocBook: The Definitive Guide](DocBook4.md)
  * ...

# 翻译 DocBook XML 文档的注意事项 #
  * 象 

&lt;placeholder-1/&gt;

 和 

&lt;placeholder-2/&gt;

 等是不能翻译的，必须原封不动。
  * “indexterm” 元素内的部分，英文有单复数，而中文没有，所以翻译的时候，要删除复数部分。为了方便，建议先不要翻译，直接复制即可。
  * 建议构建后通过精读复审，不然可能会有翻译了不该翻译的部分，语句不通顺，有错别字等问题。