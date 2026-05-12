# WebStylePrompt 隐私政策 / Privacy Policy

> 末次更新 / Last updated: 2026-05-11
> 适用版本 / Applies to: WebStylePrompt v0.1.4 及以上 / and later

---

## 中文版

### 一、我们是谁

WebStylePrompt 是一款 Chrome 浏览器扩展程序，帮助开发者快速解析任意网页的视觉风格并生成 AI 编程提示词。

### 二、我们收集什么数据

**我们不收集任何用户数据。** 包括但不限于：

- ❌ 不收集个人身份信息（姓名、邮箱、电话等）
- ❌ 不收集浏览历史、Cookie、登录状态
- ❌ 不收集页面内容、表单数据、文本输入
- ❌ 不使用任何分析、追踪或广告 SDK
- ❌ 不向任何第三方服务器发送数据

### 三、扩展如何工作

当你**主动点击插件图标并触发"解析当前页面风格"**时，扩展会：

1. 在你当前打开的网页中读取**已渲染元素的 CSS 计算样式**（颜色、字体、圆角、阴影、间距等）；
2. 在你的浏览器**本地**完成统计与聚类分析；
3. 将分析结果以文本形式展示在弹窗中，仅你本人可见。

整个过程**完全在你的浏览器本地完成**，不联网、不上传、不存档。

### 四、本地存储说明

为了实现免费版的每日生成次数限制，扩展会在浏览器本地存储一条记录：

```json
{
  "date": "2026-5-11",
  "count": 3
}
```

- 仅存储在 `chrome.storage.local`（浏览器本地）
- 存储内容仅为日期字符串和整数计数
- 卸载扩展即自动清除
- 不会同步到任何云端服务

### 五、权限说明

| 权限 | 用途 |
|---|---|
| `activeTab` | 仅在你点击插件图标时，读取当前活动标签页的样式 |
| `scripting` | 向当前页面注入只读的分析脚本 |
| `storage` | 仅用于本地存储每日使用次数 |
| `host_permissions: <all_urls>` | 让你能在任意网页（不限网站）使用本工具，仅在你主动触发时执行 |

### 六、第三方服务

本扩展不集成任何第三方服务。

### 七、儿童隐私

本扩展不针对 13 岁以下儿童设计，也不会主动收集任何用户数据。

### 八、变更通知

如本政策有更新，新版本的扩展上架时会同步更新本页面，并在文档顶部标注「末次更新」日期。

### 九、联系方式

如有疑问，请通过 Chrome Web Store 商品页留言或邮件联系：
**[edenchylu@gmail.com]**

---

## English Version

### 1. Who We Are

WebStylePrompt is a Chrome browser extension that helps developers parse the visual style of any web page and generate AI coding prompts.

### 2. What We Collect

**We do not collect any user data.** Specifically:

- ❌ No personal information (name, email, phone, etc.)
- ❌ No browsing history, cookies, or login state
- ❌ No page content, form data, or text input
- ❌ No analytics, tracking, or advertising SDKs
- ❌ No data is sent to any third-party server

### 3. How the Extension Works

When **you actively click the extension icon and trigger "Analyze current page style"**, the extension:

1. Reads **computed CSS styles** of rendered elements on your active page (colors, fonts, radius, shadows, spacing, etc.);
2. Performs frequency analysis and clustering **locally in your browser**;
3. Displays the resulting text report in the popup, visible only to you.

The entire process happens **locally in your browser** — no network requests, no uploads, no archiving.

### 4. Local Storage Disclosure

To implement the free-tier daily generation limit, the extension stores a single record in your browser:

```json
{
  "date": "2026-5-11",
  "count": 3
}
```

- Stored only in `chrome.storage.local` (local to your browser)
- Content is limited to a date string and an integer counter
- Cleared automatically when you uninstall the extension
- Never synced to any cloud service

### 5. Permission Justification

| Permission | Purpose |
|---|---|
| `activeTab` | Read styles of the currently active tab only when you click the extension icon |
| `scripting` | Inject a read-only analysis script into the active page |
| `storage` | Locally persist the daily usage counter |
| `host_permissions: <all_urls>` | Let you use the tool on any website you visit, executed only on your explicit action |

### 6. Third-Party Services

This extension integrates with no third-party services.

### 7. Children's Privacy

This extension is not directed at children under 13, and we do not knowingly collect any user data.

### 8. Changes to This Policy

If this policy is updated, the new version of the extension will reflect the change at the top of this document.

### 9. Contact

For inquiries, please reach out via the Chrome Web Store listing or email:
**[edenchylu@gmail.com]**
