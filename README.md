# F5 BIG-IP URL转换器 🚀

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)

一个功能强大的F5 BIG-IP URL编解码工具，支持单个URL解码、批量文件处理和URL加密功能。提供直观的图形用户界面。

## 📱 界面预览

### 单个解码界面

![单个解码.png](https://github.com/worlik/F5_BIG_IP_URL/blob/main/%E5%8D%95%E4%B8%AA%E8%A7%A3%E7%A0%81.png?raw=true)

### 批量处理界面

![批量解码.png](https://github.com/worlik/F5_BIG_IP_URL/blob/main/%E6%89%B9%E9%87%8F%E8%A7%A3%E7%A0%81.png?raw=true)

### URL加密界面

![url加密.png](https://github.com/worlik/F5_BIG_IP_URL/blob/main/url%E5%8A%A0%E5%AF%86.png?raw=true)

## 📖 使用指南

### 1. 单个URL解码

1. **输入URL**：在输入框中粘贴F5编码的URL
   ```
   示例: https://f5server/f5-w-7777772e676f6f676c652e636f6d$$/path
   ```

2. **执行解码**：点击"🚀 解码"按钮

3. **查看结果**：系统将显示详细的解码信息
   - F5服务器地址
   - 原始目标地址
   - 附加路径
   - 最终完整URL
   - 十六进制编码

4. **复制结果**：点击"📋 复制结果"将结果复制到剪贴板

### 2. 批量文件处理

1. **准备文件**：创建包含URL列表的文本文件
   ```
   # 示例文件内容
   https://f5server/f5-w-7777772e676f6f676c652e636f6d$$/admin
   https://f5server/f5-w-68747470733a2f2f7777772e6578616d706c652e636f6d$$/login
   # 支持注释行和空行
   ```

2. **选择文件**：点击"浏览..."选择文件，或点击"创建示例"生成模板

3. **执行批量解码**：点击"🚀 批量解码"开始处理

4. **查看进度**：实时查看处理进度和统计信息

5. **保存结果**：处理完成后点击"💾 保存结果"导出结果文件

### 3. URL加密

1. **输入URL**：在输入框中输入普通URL
   ```
   示例: www.google.com
   ```

2. **执行加密**：点击"🔒 加密"按钮

3. **获取结果**：系统将生成F5编码格式
   ```
   结果: f5-w-7777772e676f6f676c652e636f6d$$
   ```

4. **使用说明**：根据提示在F5服务器上使用加密后的URL

## 📝 文件格式说明

### 输入文件格式
支持多种URL格式的混合输入：

```text
# F5编码URL列表 - 注释行会被自动跳过
# 每行一个URL，支持以下格式:

# 完整格式（推荐）
https://f5server/f5-w-7777772e676f6f676c652e636f6d$$/path/to/resource

# 简单格式
f5-w-7777772e676f6f676c652e636f6d$$

# 复杂路径
https://proxy.company.com/f5-w-687474703a2f2f696e7465726e616c2e636f6d$$/admin/login.php

# 空行会被自动跳过

```

### 输出文件格式
解码结果文件包含详细信息：

```text
F5 URL批量解码结果
处理时间: 2024-01-20 15:30:45
总计: 100 条, 成功: 95 条, 失败: 5 条
==================================================

============================================================
第 1 条: ✅ 成功
============================================================
原始URL: https://f5server/f5-w-7777772e676f6f676c652e636f6d$$/admin
F5服务器: https://f5server
目标地址: www.google.com
附加路径: /admin
最终URL: www.google.com/admin
十六进制: 7777772e676f6f676c652e636f6d

...更多结果...
```

---

⭐ 如果这个项目对您有帮助，请给个星标支持！

☕️ 如果您觉得项目对你有帮助，可以请作者喝杯咖啡

![img.jpg](https://github.com/worlik/F5_BIG_IP_URL/blob/main/img.jpg?raw=true)


