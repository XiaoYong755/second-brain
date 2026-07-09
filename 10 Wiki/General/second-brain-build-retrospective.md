# Second Brain Build Retrospective

## One-line summary

今天这次搭建的核心成果，不只是把目录建出来，而是把这套第二大脑从“一个空文件夹”推进成了“已经可以长期使用和持续扩展的本地知识系统”。

## Why this build happened

这次搭建的起点很明确：

- 想参考 Andrej Karpathy 的 LLM wiki 思路
- 但又不想只做一个 LLM 学习仓库
- 更希望把 LLM 学习、个人知识和项目推进放进同一个系统里

所以这次不是在做一个“资料夹”，而是在搭一个以后可以持续长大的知识底盘。

## What went well

今天比较顺的地方主要有 4 个：

### 1. 很早就把方向定对了

一开始没有急着堆目录，而是先明确了这套系统的核心定位：

- 纯本地
- Markdown 优先
- Obsidian 友好但不绑定 Obsidian
- `LLM 学习库` 做核心
- 同时承接个人知识和项目推进

这个判断很关键，因为一旦方向模糊，后面的目录和笔记模板都会越搭越乱。

### 2. 很快找到了适合的整体结构

最后定下来的不是纯 PARA，也不是纯 wiki，而是混合型结构：

- `Inbox`
- `Wiki`
- `Projects`
- `Journal`
- `Library`
- `Archive`

这里最有效的一点是把 `Wiki` 定成了系统中心，而不是让资料页和项目页平铺。这样以后知识沉淀会有重心，不容易变成到处散落的材料库。

### 3. 首页和入口页做得比较及时

今天不是只建了目录，也把入口体验同步做了：

- `README` 负责欢迎和说明
- `Home` 负责日常启动
- `LLM Index` 负责专题地图

这让整个系统从一开始就不只是“有文件”，而是“知道从哪开始用”。

### 4. 很早就把版本管理接上了

今天把本地文件夹补成了 Git 仓库，也接上了 GitHub 远程。这个动作很有价值，因为第二大脑这类系统会持续变化，没有版本历史，后面很容易越改越心虚。

## Where the process got stuck

今天也有几个明显卡点，值得记下来。

### 1. GitHub 不是一开始就能直接打通

本地最初没有：

- GitHub CLI
- HTTPS 凭据
- 可用的 SSH key

所以虽然本地仓库和远程地址很快都配好了，但真正推上 GitHub 中间还是经历了几步：

- 检查登录状态
- 创建 GitHub 仓库
- 生成新的 SSH key
- 把 SSH key 加到 GitHub 账号
- 切换远程到 SSH

这部分说明一个现实问题：知识库搭建不只有内容结构，基础设施也会占一部分时间。

### 2. 浏览器侧的 GitHub 操作不是完全线性的

在创建仓库和添加 SSH key 时，浏览器会话有过几次“标签页释放”或按钮点击不生效的情况，最后是通过重新接管页面和更稳的点击方式完成的。

这类卡点虽然技术上不大，但会打断节奏。下次如果再做类似操作，应该默认把“认证、浏览器状态、远端权限”提前当成一个独立环节。

### 3. 推送结果一度看起来和真实状态不一致

今天有一次推送返回了 “Everything up-to-date”，但本地分支实际上仍然领先远程 1 个提交。最后通过再次推送和重新核验，才把状态真正对齐。

这提醒我一个很重要的原则：

- 不能靠一次返回信息就认定成功
- 必须再看一眼 `git status` 和提交指针是否真的一致

## What got built

今天最终搭出来的东西可以分成 5 层：

### 1. 本地知识库结构

- `00 Inbox`
- `10 Wiki`
- `20 Projects`
- `30 Journal`
- `40 Library`
- `90 Archive`
- `_templates`
- `_assets`

### 2. 入口页面

- `README.md`
- `10 Wiki/Home.md`
- `10 Wiki/LLM/LLM Index.md`

### 3. 模板系统

- inbox note
- wiki note
- paper note
- project note
- daily note

### 4. 初始样例内容

- 一个 Inbox 示例
- 一个论文示例
- 一个项目示例
- 一个概念示例

### 5. 第一批 LLM 核心页面

- `Transformer`
- `Attention`
- `Tokenization`
- `Pretraining`
- `Post-Training`
- `Reasoning`
- 再加上已有的 `In-Context Learning`

到这里为止，这套系统已经不只是“框架”，而是已经有了最小骨架。

## Principles that proved useful

今天这次搭建里，最有用的原则有 5 条：

### 1. 先定信息流，再定目录

目录本身不是重点，重点是每条新信息要流向哪里。

### 2. `Wiki` 应该是理解层，不是收藏层

`Library` 放你看到的东西，`Wiki` 放你真正想清楚的东西。

### 3. 入口要尽早做

一个知识库如果没有好入口，就算结构再完整，也会让人懒得打开。

### 4. 不追求一次搭满

今天没有试图把所有主题都建完，而是先把最核心的结构、首页和第一批概念页做扎实。

### 5. 尽早接 Git

第二大脑会持续调整，没有版本历史，后面会很难放心演化。

## What I learned today

今天最大的收获不是“学会怎么建知识库”，而是更确定了一件事：

真正能长期用下去的第二大脑，不是最复杂的那种，也不是最漂亮的那种，而是：

- 足够轻
- 足够清楚
- 足够容易重新打开

也就是说，它要让人每次回来都觉得：

- 我知道从哪开始
- 我知道该把什么放在哪里
- 我知道这套东西会随着我一起变得更清晰

## Next steps

接下来最自然的延续动作有 3 个：

- 给 `LLM` 区域补第二批核心页面
- 开始养成 `Inbox -> Wiki` 的真实整理习惯
- 把这套系统真正接到每天的项目推进里，而不是只停留在“搭好了”

## Related

- [Home](/Users/taobao/Desktop/第二大脑/10%20Wiki/Home.md)
- [LLM Index](/Users/taobao/Desktop/第二大脑/10%20Wiki/LLM/LLM%20Index.md)
- [Second Brain Bootstrap Project](/Users/taobao/Desktop/第二大脑/20%20Projects/second-brain-bootstrap/project.md)
