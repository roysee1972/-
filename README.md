# English Reader · 英文文本逐句朗读器

> 把一个 `.txt` 丢进去，就能**逐句听、点句翻译**——
> 给想练英语听力跟读、又不想被生词表和背单词 App 绑架的人用。
> **单个 HTML 文件，双击即用，不用安装、不用注册。**

- 在线直接用：<https://roysee1972.github.io/english-text-reader/>
- 下载：`index.html`（约 19 KB），保存后用浏览器打开即可

[English](#english)

---

## 一、为什么做这个

作者三十多岁才开始认真学英语，底子薄，传统方法基本无效。后来靠"逆向式"学习法（先大量听、听懂了再回过头看文字）才真正有起色。
但当年条件有限，只能**用电脑放音频 → 听一句 → 手动暂停 → 跟读 → 默写**，效率极低。

现在有了浏览器自带的语音合成，这个过程可以自动化：

| 当年的笨办法 | 现在 |
|---|---|
| 手动暂停、手动重放 | 点哪一句就读哪一句，随时重听 |
| 语速固定 | 0.5× ～ 2.0× 无级调速，听不清就放慢 |
| 查词要翻词典 | 点句子直接出中文翻译 |
| 材料要自己找音频 | 任意英文 `.txt` 都能当材料 |

**核心目的**：把"有一段英文文本"变成"可以反复磨耳朵的听力材料"，让听与读的循环尽可能短。

---

## 二、主要功能

1. **导入 TXT 即读** —— 选一个 `.txt` 文件，自动按句拆分，逐句渲染成可点击的段落
2. **点句即读** —— 点任意一句立刻朗读；当前句有高亮，读到哪一眼能看到
3. **美式 / 英式发音切换** —— 优先匹配英式女声（`en-GB`）／美式女声（`en-US`），默认英式
4. **语速 0.5× ～ 2.0×** —— 滑杆连续可调，默认 1.0×，适合从慢速起步逐步加速
5. **点句翻译** —— 点句子可显示中文翻译（走 MyMemory 免费翻译接口）
6. **深浅色主题** —— 按钮一键切换，夜间阅读不刺眼
7. **偏好记忆** —— 发音口音、语速、主题存本地，下次打开还是原来的设置

---

## 三、怎么用

1. 下载 `index.html`，用 **Chrome / Edge** 打开（这两个浏览器自带的英语语音最全、效果最好）
2. 点「选择文件」，挑一个英文 `.txt`
3. 点任意一句开始听；需要中文就再点一下看翻译
4. 听不清就把语速拉到 0.6× 左右，听顺了再往上加

**找练习材料**：Project Gutenberg（古登堡计划）有海量英文公版书 TXT，下载后直接拖进来就能听。

---

## 四、说明与限制

- **语音来自浏览器/系统内置合成**（Web Speech API），没有打包音频文件，所以文件只有 19 KB；
  代价是发音质量取决于浏览器自带的语音包——**Chrome / Edge 明显好于其他浏览器**。
- **翻译功能需要联网**（调用 MyMemory 免费接口），断网时朗读不受影响，只是翻译不可用。
- 只支持 `.txt`，不支持 PDF / Word / EPUB。
- 超长文本会渲染成很多句子，属于正常现象；建议按章节拆成多个小文件练。

---

## 五、许可

MIT。自用、改、分发都随意。

---

<a name="english"></a>
## English

**English Reader** — a single-file HTML tool that turns any English `.txt` into a
listen-and-repeat exercise: it splits the text into sentences, reads any sentence aloud on click,
and shows a Chinese translation on demand.

Built by a Chinese learner who started English in his thirties and found conventional methods useless —
what worked was the "reverse" approach (listen first, read later). This tool automates the tedious part
of that loop: pause, replay, dictate.

Features: TXT import with automatic sentence splitting; click-to-read with highlight;
British / American voice switch (prefers female voices); speed 0.5×–2.0×; per-sentence translation
(MyMemory API, requires internet); light/dark theme; preferences saved locally.

Open `index.html` in **Chrome or Edge** (they ship the best built-in English voices).
Audio comes from the browser's built-in speech synthesis — that is why the whole tool is only 19 KB.

MIT licensed.
