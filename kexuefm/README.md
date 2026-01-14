
# start

when you have [skill/dev-browser](https://github.com/SawyerHood/dev-browser/tree/main/skills/dev-browser) in your 

Project config: `.opencode/skill/<name>/SKILL.md`
Global config: `~/.config/opencode/skill/<name>/SKILL.md`
Project Claude-compatible: `.claude/skills/<name>/SKILL.md`
Global Claude-compatible: `~/.claude/skills/<name>/SKILL.md`

, you can use claude/opencode and your favorite model provider,

first kexue.fm has it own content page https://kexue.fm/content.html, you should click button “点击加载更多” until there are no more archieves.


> 完美！我已经找到了"点击加载更多"按钮。让我总结一下分析结果：
分析结果
"点击加载更多"按钮的元素是：
> - 选择器: input#more_archives_botton
    - 类型: `<input type="button">`
    - ID: more_archives_botton
    - 显示文本: "点击加载更多..."
    - 点击事件: more_archises()
按钮功能:
当点击按钮时，会调用 more_archives() JavaScript函数，该函数会：
> 1. 获取 #archives 元素（文章列表容器）
    2. 将容器高度增加2048px（每次点击加载更多内容）
    3. 如果容器高度达到或超过滚动高度，按钮文本会变为"全部文章已加载完毕"
按钮位置:
在页面文章列表的底部，#archives_body div容器内。
完整HTML结构:
`<input id="more_archives_botton" type="button" onclick="more_archives()" value="点击加载更多..." style="">`
这个按钮是一个简单的input按钮，通过JavaScript动态加载更多文章内容，而不是传统的分页或AJAX加载。

just put "fetch all html like kexue.fm/archives/11530"

that's all! then we got all datas needed.

# data feature

The source code of the mathematical formula is in the html file, so even if the crawling script only grabs a simple html file and browser cannot render the mathematical formula because of .js missing, LLM can still be parsed easily.

after all, markdown and mathjax are the underlying logic of llm (

# data cleaning

The components that come with the website will also occupy the context。



# what we want?

As we all know, these High-intensity blogger is a minority.

Fortunately, the webmaster of kexue.fm not only blogs intensively, but his blog has also covered his main growth path for more than ten years.

But is a book list or a bunch of research topic terms what we want? Similar, but if the two have a time span of more-than-ten-years and a scale of thousands, they are completely different.

**just skills!**

# skills √ RAG ×

