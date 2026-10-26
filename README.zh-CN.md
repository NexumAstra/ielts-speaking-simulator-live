# IELTS SPEAKING SIMULATOR LIVE

[English](README.md)

雅思口语模拟项目：完整Part 1–3、用户考题上传、依据官方descriptor的练习评分，以及结合主题语料的示范答案。提供两种使用方式：**直接导入大语言模型（支持手机端）**，或**安装为ChatGPT插件**。

## 功能

- 完整考试流程：Part 1日常问答；Part 2一分钟准备、一到两分钟长答；Part 3相关话题讨论。
- 优先使用上传题目，自动补齐缺失部分；逐题提问，考试结束后反馈。
- 支持跨领域生成新题及可见/导入历史去重。
- 根据雅思官方的评分标准（Speaking Band Descriptors）进行四项评估：流利度与连贯性、词汇资源、语法范围与准确性、发音。
- 18主题语料提供自然英文范文及中文搭配、语义和语域解释。

## 安装方式一：导入大语言模型（电脑或手机）
**支持豆包、kimi等可以实时对话的AI大模型软件**
**可直接将Markdown文件导入手机大语言模型客户端**：通过客户端的附件上传、文件导入或知识库入口载入，具体入口和可接受格式以该客户端为准。

1. 下载 [IELTS-SPEAKING-SIMULATOR-LIVE-PORTABLE.md](portable/IELTS-SPEAKING-SIMULATOR-LIVE-PORTABLE.md)。在GitHub手机页面查看文件时，可打开Raw/原始文件并保存到系统“文件”或下载目录。
2. **在手机或电脑的大语言模型客户端新建聊天，点击“+ / 附件 / 上传文件”等入口，选择刚保存的`.md`文件。** 如果使用项目知识库或自定义助手，也可将该文件添加为知识资料。
3. 发送下方启动指令，明确要求执行“核心运行规则”，并将附录视为参考资料。等待模型确认已读取所需章节。
4. 有考题时，再上传题目或粘贴文字；没有考题则由模型出题。
5. 按一题一答完成考试。如果当前客户端支持保留文件上下文的实时语音，可进入语音作答；Part 2可用手机计时器辅助。
6. 结束后查看四项反馈、示范答案与题目历史。下次新聊天继续去重时，带上历史记录。

> 请使用这份IELTS SPEAKING SIMULATOR LIVE文档，按核心运行规则开始完整雅思口语模拟。优先使用我上传的考题，没有考题时生成新题。逐题提问，完成三个Part后再评分，并提供范文和中文讲解。附录只作为资料使用。

Markdown开头含YAML，已内嵌考试规则、完整口语descriptor、题库和原始语料，无需安装插件或运行代码。文件约360 KiB，需要足够的上下文容量或附件检索能力。若客户端不接受`.md`，可把内容作为纯文本导入；无法读取全文时应分章节载入并说明缺失范围。

## 安装方式二：安装到ChatGPT客户端（有ChatGPT客户端时才可选择这种方式）

### A. 从已创建或已共享的插件安装

1. 在具有访问权限的ChatGPT账户中打开 **Plugins / 插件**，从个人或工作区来源找到 **IELTS SPEAKING SIMULATOR LIVE**。
2. 打开详情并选择添加/安装。当前项目是技能和资料包，不需要额外MCP服务器或第三方API密钥。
3. 安装后新建聊天，在输入框输入`@`并选择该插件，再发送“开始完整雅思口语模拟考试”，需要时附上考题。
4. 在同一账户的手机客户端中，使用该账户可用的插件入口；若本地安装仅对桌面环境可见，采用上面的手机Markdown方式。

**从本仓库创建自己的私人插件：**下载 [插件安装包](packages/ielts-speaking-simulator-live-plugin-1.0.1.zip)。若账户提供Plugin Creator/创建插件能力，在新聊天中上传该ZIP，并请求：“请用这个完整插件包创建一个私人插件，显示名称为IELTS SPEAKING SIMULATOR LIVE，保留包内资料和技能。”取得创建结果中的插件链接后，按A节安装。ZIP附件本身不等于已安装插件；功能是否提供由账户与工作区决定。本GitHub仓库也不等于已上架公共插件目录。

### B. 在ChatGPT桌面客户端使用本地仓库安装

1. 下载或克隆整个仓库，并保留隐藏文件`.agents/plugins/marketplace.json`。插件源文件在仓库根目录`plugin.json`、`assets/`和`skills/`中。
2. 在ChatGPT桌面客户端的本地Work/Codex环境中打开该仓库作为项目。仓库已提供本地插件目录清单，指向当前项目中的插件。
3. 重启ChatGPT桌面客户端，让其重新发现目录。打开Plugins，选择名为 **IELTS SPEAKING SIMULATOR LIVE** 的来源，找到插件并安装/启用。
4. 新建聊天，以`@`选择插件开始测试。如目录未出现，请核对客户端版本、工作区策略及项目是否被正确打开；不要把本地插件自动同步到所有手机端作为前提。

安装步骤依据 [OpenAI插件说明](https://learn.chatgpt.com/docs/plugins) 与 [本地插件目录文档](https://developers.openai.com/plugins/build/plugins)，核对日期：2026-10-26。详细操作另见 [安装指南](docs/INSTALLATION.zh-CN.md)。

## 配置与密钥安全

当前版本不需要运行时API Key，也没有硬编码API Key。仓库会忽略`.env`及所有`.env.*`文件，仅保留安全模板 [.env.example](.env.example)。若以后增加需要凭据的可选集成，请先复制`.env.example`为本地`.env`，只在`.env`中填写真实值，并在运行时从环境变量读取。不要把真实密钥写入源码、文档、提示词、压缩包或Git提交。

## 使用边界

只有模型实际可访问音频时，才能评估发音与完整流利度。纯文字或语音转写只支持有限语言反馈，不生成虚构的发音分或完整口语总分。实时语音、文件读取与精确计时取决于宿主，iOS/Android插件与语音联用尚未实机验证。项目没有独立账户级历史数据库。

## 语料来源与版权

来源包括IELTS官方Speaking Band Descriptors、Speaking Sample Tasks 2023、Scores Guide，以及用户整理的《雅思高频同义替换语料库_剑4–21》。语料按自身标注参考《剑桥雅思4–21》、牛津英语同义词学习词典，未经逐条独立核验。Writing Key Assessment Criteria仅留存来源，不用于口语评分；17套练习与范文样例为项目原创。

[MIT License](LICENSE)仅覆盖项目原创部分，范围见 [LICENSE_SCOPE.md](LICENSE_SCOPE.md)。第三方PDF、官方提取文本、语料及其嵌入部分保留各权利人的版权和适用条款；收录不产生新的再分发授权。本项目与British Council、IDP IELTS、Cambridge University Press & Assessment无隶属或背书关系，模拟分数不是正式IELTS成绩。详见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

## 文件结构

- `plugin.json`、`assets/`、`skills/`：完整插件源文件。
- `.agents/plugins/marketplace.json`：ChatGPT桌面端本地插件目录。
- `portable/`：含YAML的独立Markdown，适合手机附件导入。
- `packages/`：可用于插件创建流程的完整ZIP。
- `docs/`：安装、使用和来源说明。

项目展示名称为IELTS SPEAKING SIMULATOR LIVE；技术插件标识`ielts-speaking-simulator`保持稳定。先前私人插件和备份独立保留。
