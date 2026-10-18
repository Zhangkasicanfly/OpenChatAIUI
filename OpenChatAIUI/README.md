# OpenChatAIUI

一个开箱即用的开源 AI 对话界面模板。

## 特性

- **单文件**：一个 HTML 文件，零依赖，双击即可打开
- **深度思考滑块**：关闭 / 低 / 中 / 高 / 2×
- **增强 Markdown**：表格、任务列表、图片、高亮、代码块、嵌套列表
- **用户消息折叠**：超过 4 行自动折叠，可展开
- **停止后继续生成**：中断的输出可以继续
- **深色 / 浅色主题**：支持跟随系统
- **快捷键**：Ctrl / ⌘ + K 新建对话

## 快速开始

1. 下载 index.html
2. 双击打开
3. 点击左下角「设置」
4. 填入 API Base URL 与 API Key
5. 关掉「演示模式」
6. 开始对话

## 配置

编辑文件顶部的 `CONFIG` 对象即可自定义：

- `appName`：应用名称
- `models`：模型列表（`reasoning: true` 的模型会显示深度思考滑块）
- `defaultApiBase`：默认 API 地址
- `defaultMaxChars`：默认字数上限

## 生产环境注意

以下功能仅用于开源演示，上线时请按需替换：

- **演示模式**：不调用 API，返回示例回复
- **前端输入 API Key**：生产环境应走后端代理
- **localStorage 持久化**：应使用数据库
- **项目文件浏览器**：仅开源时展示

## 兼容性

任何兼容 OpenAI `/chat/completions` 格式的接口都可以接入，包括：

- OpenAI 官方
- DeepSeek（支持 `reasoning_content`）
- 各类中转站
- 自建服务

## 许可证

MIT License
