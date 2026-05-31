# 随机点名器（纯前端版）

一个基于 HTML + CSS + JavaScript 的纯前端随机点名应用，无需后端服务器，数据保存在浏览器本地存储（localStorage）中。

## 功能特性

- ✅ 创建、重命名、删除名单
- ✅ 批量添加名字（支持逗号、中文逗号、换行分隔）
- ✅ 单独删除名单中的某个名字
- ✅ 自动去重
- ✅ 随机点名（支持指定人数）
- ✅ 点名统计（总点名次数 + 每人被点名次数，可视化柱状图）
- ✅ 支持重置统计数据
- ✅ 数据持久化保存（localStorage）
- ✅ 响应式设计，支持手机和电脑

## 使用方法

### 方式一：直接打开
双击 `index.html` 文件，在浏览器中打开即可使用。

### 方式二：使用本地服务器（推荐）
```bash
# Python 3
python -m http.server 8080

# 或 Node.js
npx serve .

# 然后浏览器访问 http://localhost:8080
```

## 数据存储

所有数据保存在浏览器的 **localStorage** 中：
- 名单名称、成员列表
- 点名统计数据（总次数、每人次数）
- 数据不会随页面关闭而丢失
- 清除浏览器数据会导致名单丢失

## 项目结构

```
roll_call_web/
├── index.html      # 主文件（包含 HTML + CSS + JS）
└── README.md       # 使用说明
```

## 浏览器兼容性

- Chrome / Edge / Firefox / Safari 等现代浏览器
- 支持移动端浏览器
- 需要浏览器启用 JavaScript 和 localStorage
