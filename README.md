# 🙏 致谢

本页面基于 [阿东玩AI](https://github.com/adongwanai) 的 [LLM-Resume-Template](https://github.com/adongwanai/LLM-Resume-Template) 修改而来。原项目采用 CC BY 4.0 许可证 进行授权。

本页面基于 [Tao Jiang](https://github.com/hijiangtao) 的 [resume](https://github.com/hijiangtao/resume) 修改而来。原项目采用 MIT License 许可证 进行授权。请注意，原模板中包含的特定字体不适用此许可证。

感谢原作者们的优秀工作！

作者基于个人审美与爱好进行了深度优化和内容重构。

# 更新


- 2026.04.05

  [初始化] Fork 原项目，并在 README 中完善对原作者的致谢。

  [模板调整] 删除了“个人总结”部分，微调了一些内容并更新README。

# 适用于各专业学生的简历模板 | Professional LaTeX resume template for students of various majors

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![LaTeX](https://img.shields.io/badge/LaTeX-Template-green.svg)](https://www.latex-project.org/)
[![GitHub stars](https://img.shields.io/github/stars/suanlilog/student-resume-template)](https://github.com/suanlilog/student-resume-template)

> **💡 如果这个模板对你有帮助，请先点击右上角的 ⭐️ Star 支持一下！你的 Star 是对我们最大的鼓励！**  
> **🔥 推荐 Fork 本项目后进行修改，这样你可以保留自己的版本，也方便后续更新！**

## 📸 效果预览

<div align="center">
  <img src="https://obsidian-hexo-blog-1357454370.cos.ap-beijing.myqcloud.com/hexo/%E7%A4%BA%E4%BE%8BPDF_pages-to-jpg-0001.jpg" alt="头像简历效果展示" width="800"/>
  <p><i>简历模板有头像效果展示</i></p>
</div>

## ✨ 特性

- 📸 **支持头像**：提供带头像版本，让简历更加个性化和专业（可选）
- 📝 **专业内容结构**：涵盖科研经历、实习经历、项目经历等完整板块
- 🔧 **易于修改**：提供完整的占位符模板，方便快速替换个人信息
- 🎨 **排版精美**：基于优秀的 LaTeX 简历模板
- 🚀 **一键编译**：支持 Overleaf 在线编辑，无需本地配置环境

## 📁 文件说明

```
Resume-Template/
├── resume-photo.tex       # 带头像简历⭐️
├── resume-photo.cls       # 带头像支持的样式文件 ⭐️
├── suanligongfang.jpg         # 示例头像图片
├── Makefile               # 编译脚本
├── fontawesome5/          # 图标字体文件
└── README.md              # 本文件
```

## 🚀 快速开始

### 使用 Overleaf（强烈推荐，无需配置环境）

#### 步骤 0: Star 和 Fork 项目（重要！）

1. 点击页面右上角的 ⭐️ **Star** 按钮，支持一下项目！
2. 点击右上角的 **Fork** 按钮，将项目 fork 到你的账号下
3. 在你 fork 的仓库页面，点击 **Code** → **Download ZIP** 下载项目

> 💡 **为什么推荐 Fork？**  
> - 你可以在自己的仓库中自由修改，不会影响原项目
> - 方便追踪你的修改历史
> - 当原项目更新时，你可以轻松同步最新内容
> - Fork 和 Star 能让更多人发现这个项目！

#### 步骤 1: 导入 Overleaf

1. 访问 [Overleaf](https://www.overleaf.com/) 并登录/注册
2. 点击左上角 **New Project** → **Upload Project**
3. 上传刚才下载的 ZIP 文件
4. 等待项目导入完成

#### 步骤 3: 设置编译器【重点】

1. 【重点】确保编译器设置为 **XeLaTeX**：点击左上角`文件 -> 设置 -> 编译器`，选择`XeLaTeX`
2. 点击 **Recompile** 即可预览 PDF

#### 步骤 4: 替换头像

1. 准备一张正方形或圆形的照片（推荐尺寸 500×500 像素以上）
2. 在 Overleaf 左侧文件列表中，点击上传图标上传你的照片
3. 打开 `resume-photo.tex`，修改第 17 行：
   ```latex
   \ResumePhoto{你的照片文件名.jpg}
   ```
4. 如果不想使用头像，直接删除或注释掉这一行即可

#### 步骤 5: 开始编辑

直接在 Overleaf 编辑器中修改对应的 `.tex` 文件，保存后会自动重新编译并更新 PDF 预览。


## 📝 编辑教程

### 1. 修改个人信息

```latex
\ResumeName{算栗工坊} % 修改为你的姓名
\ResumePhoto{suanligongfang.png} % 修改为你的头像文件名，或删除这行不使用头像

\begin{document}

\ResumeContacts{
  138-XXXX-XXXX,%
  \ResumeUrl{mailto:lzihan1226@163.com}{lzihan1226@163.com},
  %
  \ResumeUrl{https://www.suanlilog.com/}{suanlilog.com}%或者写个人主页https://xxxx.github.io/，没有主页就注释这一行。
  %前面括号写真实链接，后面括号可以写简称
  %
}
```

### 2. 替换其他内容

在overleaf网页右边编译出来的PDF文件中，双击你想要修改的地方，左边会自动跳转到对应源代码处，删除模板内容并修改为你的信息即可。

### 3. 调整板块顺序

根据你的求职重点，可以调整各个板块的顺序。例如，如果你的项目经历更出色，可以把项目经历放在实习经历之前。

### 4. 添加/删除板块

如果某个板块不需要，直接删除/注释对应的 `\sectionTitle` 和 `\begin{...} \end{...}` 部分即可。

## 🤖 AI 提示词参考

使用 Cursor、ChatGPT 或 Claude 时，可以参考以下提示词快速修改简历：

### 提示词 1: 修改个人基本信息

```
请帮我修改简历的个人信息部分：
- 姓名：张三
- 手机：138-1234-5678
- 邮箱：zhangsan@pku.edu.cn
- 学校：北京大学
- 专业：计算机科学与技术
- 学位：硕士
- 生日：1999-03
```

### 提示词 2: 填充科研经历

```
请帮我填充科研经历部分，我的研究方向是：
- 方向：多模态大模型的指令微调
- 时间：2024.03 - 至今
- 问题：现有多模态模型在细粒度视觉理解任务上表现不佳
- 方法：设计了区域级别的对齐策略，在 RefCOCO 数据集上训练
- 效果：相比 LLaVA baseline，准确率提升了 8.5%
- 成果：论文已投稿 CVPR 2025

请保持专业的学术写作风格，突出技术细节和量化指标。
```

### 提示词 3: 填充实习经历

```
请帮我填充实习经历，信息如下：
- 公司：字节跳动
- 部门：AI Lab - 大模型团队
- 时间：2024.06 - 2024.12
- 工作内容：
  1. 参与豆包大模型的数据构造，构造了 3B tokens 的代码数据，HumanEval 得分提升 6pp
  2. 负责模型的 SFT 训练，使用 LoRA 微调，训练了 5 个版本
  3. 优化推理性能，使用 vLLM，推理速度提升 50%

请用专业的方式描述，突出数据规模、技术方案和量化效果。
```

### 提示词 4: 填充项目经历

```
请帮我填充项目经历，我做了一个 RAG 项目：
- 项目名称：企业知识库智能问答系统
- 时间：2023.09 - 2024.01
- 背景：公司内部文档分散，员工查找信息效率低
- 方案：搭建了基于 RAG 的问答系统，使用 BGE-large 做向量化，FAISS 做检索，GPT-4 做生成
- 优化：加入了 HyDE 和重排序，召回率从 72% 提升到 88%
- 效果：系统上线后，员工查询效率提升 60%，好评率 91%

请用项目报告的风格描述，突出问题、方案、优化和效果。
```

### 提示词 5: 批量替换占位符

```
请帮我把简历中的所有占位符 XXXX 和 XX 替换为合理的示例内容，要求：
1. 内容贴合大模型算法工程师的工作场景
2. 使用真实存在的模型名称（如 LLaMA、Qwen、GPT-4）
3. 使用真实的 benchmark（如 MMLU、HumanEval、GSM8K）
4. 数字要合理（如提升幅度通常在 5%-20% 之间）
5. 保持专业性和可信度
```

### 提示词 6: 优化语言表达

```
请帮我优化简历中的"实习经历"部分，要求：
1. 使用更专业的技术术语
2. 突出量化指标和业务影响
3. 使用动词开头，增强行动力
4. 控制每条不超过 2 行
5. 遵循 STAR 法则（情境-任务-行动-结果）
```

## 📄 模板预览

### 科研经历示例

```latex
\item \textbf{基于强化学习的自主决策 Agent 系统研究} \hfill 2024.03 --- 至今
\begin{itemize}
    \item \textbf{问题背景}: 现有 LLM-based Agent 在复杂任务中存在决策路径冗余...
    \item \textbf{研究内容}: 1) 提出基于 PPO 的 Agent 决策优化框架...
    \item \textbf{相关成果}: 第一作者论文已投稿 NeurIPS 2025...
\end{itemize}
```

### 项目经历示例

```latex
\item \textbf{基于自我纠错机制的智能 RAG 检索系统} \hfill 2024.01 --- 2024.05
\begin{itemize}
    \item \textbf{项目背景}: 为解决企业内部知识库检索效率低下问题...
    \item \textbf{核心痛点}: 最初版本召回率仅 65%...
    \item \textbf{技术方案}: 1) 借鉴 ReAct 思想, 设计迭代式检索策略...
    \item \textbf{最终效果}: 召回率从 65% 提升至 85%...
\end{itemize}
```

## 💡 内容建议

### 科研经历

- 突出**问题背景**、**技术方案**和**量化效果**
- 提及具体的模型（LLaMA、GPT-4）、方法（LoRA、DPO）和 benchmark（MMLU、HumanEval）
- 强调论文发表、开源项目等学术成果

### 实习经历

- 使用 **STAR 法则**：情境（Situation）→ 任务（Task）→ 行动（Action）→ 结果（Result）
- 量化你的贡献：数据规模（XB tokens）、性能提升（X pp）、业务影响（XX% 提升）
- 突出你在团队中的角色和独立负责的模块

### 项目经历

- 描述**项目背景**和**痛点**，体现问题意识
- 详细说明**技术方案**，展示技术深度
- 强调**创新点**和**最终效果**，最好有对比数据

### 个人荣誉

- 优先列出与 AI/算法相关的荣誉
- 顶会论文 > 竞赛奖项 > 奖学金
- 注明具体排名（如 Top 1%、金牌）和参与人数

## 🚧 TODO (未来计划)

- [ ] 尝试增加 Prism 平台进行自动化编译


## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个模板！

如果这个模板对你有帮助，欢迎给个 ⭐️ Star！

## 📮 联系方式

- GitHub: [@zihan12ai](https://github.com/zihan12ai), [@算栗工坊](https://github.com/suanlilog)
- 项目地址: [student-resume-template](https://github.com/suanlilog/student-resume-template)

## 📜 许可证

本项目采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 许可证。

你可以自由地：
- ✅ **分享** — 复制和再分发本模板
- ✅ **修改** — 重新组合、转换和构建本模板
- ✅ **商用** — 将本模板用于商业目的

唯一要求：**署名** — 你必须给出适当的署名，提供指向本许可的链接，同时说明是否有做修改。


---

**祝你求职顺利，拿到心仪的 Offer！🎉**

如有问题，欢迎提 Issue 或加入讨论！
