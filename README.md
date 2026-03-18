# K-Pop街舞AI助手试炼：Web仿真系统

这是一个纯前端静态 Demo，用来模拟 K-Pop 街舞 AI 助手的完整交互闭环：内容上传、AI 分析、结果可视化、学习引导、历史记录与收藏。

## 功能概览

- `DanceActionAnalysis`：舞蹈动作分析，展示走位网格、难度系数、齐舞整齐度、动作亮点
- `AudioToneRecognition`：音频音色识别，展示成员音色占比、歌词段落联动、成员音色标签
- `DancePracticeAssistant`：舞蹈陪练纠错，展示标准动作 vs 用户动作对比、节奏力度评分、纠错建议
- `DanceStepLearning`：舞步学习推荐，展示舞步识别结果、难度分级、抖音教学链接与学习顺序
- `HistoryAndCollection`：保存最近分析记录，支持收藏分析结果与教学链接
- 加分项：个性化设置、练习计划生成、分享功能模拟

## 文件说明

- `index.html`：页面结构
- `styles.css`：K-Pop 风格视觉与响应式布局
- `app.js`：预设数据、交互逻辑、AI 分析流程模拟、历史收藏持久化

## 运行方式

1. 直接双击 `index.html`，或在浏览器中打开它
2. 选择任一分析模式
3. 使用预设内容，或者切换到“本地上传”模拟上传文件
4. 点击“开始 AI 分析”
5. 查看结果、收藏、生成分享卡片，并在左侧查看历史与收藏

## 交互流程

1. 选择分析模式
2. 选择预设内容或上传文件
3. 触发 AI 模拟分析进度
4. 查看对应结果可视化
5. 获取学习建议 / 练习计划 / 教学链接
6. 收藏结果并在历史记录中回看

## 预设数据修改方法

所有预设数据都集中在 `app.js` 的 `presetLibrary` 常量中。

- 修改舞蹈动作分析数据：编辑 `presetLibrary.danceAction`
- 修改音频音色识别数据：编辑 `presetLibrary.audioTone`
- 修改舞蹈陪练纠错数据：编辑 `presetLibrary.practiceAssistant`
- 修改舞步学习推荐数据：编辑 `presetLibrary.stepLearning`

## 技术说明

- 无需构建工具，无第三方依赖
- 使用 `localStorage` 存储历史记录、收藏夹与个性化偏好
- 使用 CSS 渐变、进度条、卡片布局和响应式断点实现演示效果
- 所有 AI 能力均为前端模拟，重点展示产品逻辑与交互闭环
