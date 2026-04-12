# Element Plus 中后台产品 UI 设计规范

## 1. 设计原则

### 1.1 核心原则

- **一致性**：保持视觉和交互的一致性，降低用户学习成本
- **简洁性**：界面简洁清晰，去除多余元素，突出核心内容
- **可用性**：注重用户体验，确保组件易用、易理解
- **响应式**：适配多种设备和屏幕尺寸
- **可访问性**：支持键盘操作和屏幕阅读器

### 1.2 设计目标

- 提供统一的设计语言，确保产品视觉一致性
- 提高开发效率，减少重复工作
- 保证产品质量，提升用户体验
- 降低维护成本，便于迭代更新

***

## 2. 色彩系统

### 2.1 主色调

```css
--el-color-primary: #409EFF          /* 品牌主色 - 蓝色 */
--el-color-primary-light-3: #79bbff  /* 主色浅3 - 悬停态 */
--el-color-primary-light-5: #a0cfff  /* 主色浅5 - 禁用态 */
--el-color-primary-light-7: #c6e2ff  /* 主色浅7 - 背景 */
--el-color-primary-light-8: #d9ecff  /* 主色浅8 - 浅色背景 */
--el-color-primary-light-9: #ecf5ff  /* 主色浅9 - 最浅背景 */
--el-color-primary-dark-2: #337ecc   /* 主色深 - 点击态 */
```

### 2.2 功能色

```css
/* 成功 */
--el-color-success: #67C23A
--el-color-success-light-3: #95d475
--el-color-success-light-5: #b3e19d
--el-color-success-light-7: #d1edc4
--el-color-success-light-9: #f0f9eb
--el-color-success-dark-2: #529b2e

/* 警告 */
--el-color-warning: #E6A23C
--el-color-warning-light-3: #eebe77
--el-color-warning-light-5: #f3d19e
--el-color-warning-light-7: #f8e3c5
--el-color-warning-light-9: #fdf6ec
--el-color-warning-dark-2: #b88230

/* 危险 */
--el-color-danger: #F56C6C
--el-color-danger-light-3: #f89898
--el-color-danger-light-5: #fab6b6
--el-color-danger-light-7: #fcd3d3
--el-color-danger-light-9: #fef0f0
--el-color-danger-dark-2: #c45656

/* 信息 */
--el-color-info: #909399
--el-color-info-light-3: #b1b3b8
--el-color-info-light-5: #c8c9cc
--el-color-info-light-7: #dedfe0
--el-color-info-light-9: #f4f4f5
--el-color-info-dark-2: #73767a
```

### 2.3 中性色

```css
/* 主要文字 */
--el-text-color-primary: #303133     /* 主要文字 - 标题 */
--el-text-color-regular: #606266     /* 常规文字 - 正文 */
--el-text-color-secondary: #909399   /* 次要文字 - 辅助信息 */
--el-text-color-placeholder: #A8ABB2 /* 占位文字 */
--el-text-color-disabled: #C0C4CC    /* 禁用文字 */

/* 边框 */
--el-border-color: #DCDFE6           /* 一级边框 */
--el-border-color-light: #E4E7ED     /* 二级边框 */
--el-border-color-lighter: #EBEEF5   /* 三级边框 */
--el-border-color-extra-light: #F2F6FC /* 四级边框 */

/* 填充色 */
--el-fill-color: #F0F2F5             /* 基础填充 */
--el-fill-color-light: #F5F7FA       /* 浅填充 - 悬停背景 */
--el-fill-color-lighter: #FAFAFA     /* 更浅填充 */
--el-fill-color-extra-light: #FAFCFF /* 最浅填充 */
--el-fill-color-dark: #E6E8EB        /* 深填充 */
--el-fill-color-darker: #DEDFE0      /* 更深填充 */
--el-fill-color-blank: #FFFFFF       /* 空白填充 */

/* 背景色 */
--el-bg-color: #FFFFFF               /* 页面背景 */
--el-bg-color-page: #F2F3F5          /* 页面背景（灰） */
--el-bg-color-overlay: #FFFFFF       /* 浮层背景 */
```

***

## 3. 字体规范

### 3.1 字体族

```css
/* 中文优先 */
font-family: 'Helvetica Neue', Helvetica, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', '微软雅黑', Arial, sans-serif;

/* 等宽字体（代码） */
font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, Courier, monospace;
```

### 3.2 字号规范

```css
--el-font-size-extra-large: 20px     /* 大标题 */
--el-font-size-large: 18px           /* 标题 */
--el-font-size-medium: 16px          /* 小标题 */
--el-font-size-base: 14px            /* 正文（默认） */
--el-font-size-small: 13px           /* 小字 */
--el-font-size-extra-small: 12px     /* 辅助文字 */
```

### 3.3 字重规范

```css
--el-font-weight-primary: 500        /* 常规 */
--el-font-weight-secondary: 100      /* 细体 */
```

### 3.4 行高规范

```css
--el-font-line-height-primary: 24px  /* 主要行高 */
--el-font-line-height-secondary: 16px /* 次要行高 */
```

### 3.5 字体使用场景

| 场景    | 字号   | 字重  | 行高   | 用途      |
| ----- | ---- | --- | ---- | ------- |
| 页面大标题 | 20px | 500 | 28px | 页面主标题   |
| 卡片标题  | 16px | 500 | 24px | 卡片、区块标题 |
| 正文    | 14px | 400 | 24px | 正文内容    |
| 辅助文字  | 13px | 400 | 20px | 辅助说明    |
| 标签/徽章 | 12px | 400 | 18px | 标签、时间戳  |

***

## 4. 间距系统

### 4.1 基础间距

```css
--el-spacing-mini: 4px
--el-spacing-small: 8px
--el-spacing-base: 12px
--el-spacing-medium: 16px
--el-spacing-large: 20px
--el-spacing-extra-large: 24px
```

### 4.2 组件间距规范

| 场景     | 间距值  | 说明          |
| ------ | ---- | ----------- |
| 页面边距   | 20px | 页面内容区边距     |
| 卡片内边距  | 20px | 卡片内部padding |
| 表单元素间距 | 16px | 表单项之间       |
| 按钮间距   | 12px | 按钮之间        |
| 表格行高   | 48px | 表格默认行高      |
| 列表项间距  | 12px | 列表项之间       |

***

## 5. 圆角规范

```css
--el-border-radius-small: 2px        /* 小圆角 - 标签、徽章 */
--el-border-radius-base: 4px         /* 基础圆角 - 按钮、输入框 */
--el-border-radius-small: 2px        /* 小圆角 */
--el-border-radius-round: 20px       /* 圆角按钮 */
--el-border-radius-circle: 50%       /* 圆形 - 头像、图标按钮 */
```

### 5.1 圆角使用场景

| 组件   | 圆角值  | 说明     |
| ---- | ---- | ------ |
| 按钮   | 4px  | 默认按钮   |
| 圆角按钮 | 20px | pill形状 |
| 圆形按钮 | 50%  | 图标按钮   |
| 输入框  | 4px  | 默认输入框  |
| 卡片   | 4px  | 默认卡片   |
| 对话框  | 4px  | 弹窗     |
| 标签   | 4px  | 默认标签   |
| 徽章   | 10px | 圆角徽章   |

***

## 6. 阴影规范

```css
--el-box-shadow: 0px 12px 32px 4px rgba(0, 0, 0, 0.04), 0px 8px 20px rgba(0, 0, 0, 0.08)
--el-box-shadow-light: 0px 0px 12px rgba(0, 0, 0, 0.12)
--el-box-shadow-lighter: 0px 0px 6px rgba(0, 0, 0, 0.12)
--el-box-shadow-dark: 0px 16px 48px 16px rgba(0, 0, 0, 0.08), 0px 12px 32px rgba(0, 0, 0, 0.12), 0px 8px 16px -8px rgba(0, 0, 0, 0.16)
```

### 6.1 阴影使用场景

| 场景   | 阴影类型             | 说明   |
| ---- | ---------------- | ---- |
| 卡片默认 | 无                | 平面展示 |
| 卡片悬停 | box-shadow-light | 轻微浮起 |
| 下拉菜单 | box-shadow       | 明显浮层 |
| 对话框  | box-shadow       | 模态浮层 |
| 抽屉   | box-shadow       | 侧边浮层 |
| 通知   | box-shadow-light | 提示浮层 |

***

## 7. 断点系统（响应式）

```css
--el-breakpoint-xs: 0        /* 超小屏幕 - 手机 */
--el-breakpoint-sm: 768px    /* 小屏幕 - 平板 */
--el-breakpoint-md: 992px    /* 中屏幕 - 笔记本 */
--el-breakpoint-lg: 1200px   /* 大屏幕 - 桌面 */
--el-breakpoint-xl: 1920px   /* 超大屏幕 */
```

### 7.1 响应式规则

| 断点 | 宽度范围            | 布局调整            |
| -- | --------------- | --------------- |
| xs | < 768px         | 单列布局，侧边栏隐藏，汉堡菜单 |
| sm | 768px - 991px   | 双列布局，侧边栏可折叠     |
| md | 992px - 1199px  | 三列布局，完整侧边栏      |
| lg | 1200px - 1919px | 四列布局，完整侧边栏      |
| xl | ≥ 1920px        | 多列布局，完整侧边栏      |

### 7.2 中后台布局响应式

- **桌面端 (≥992px)**：侧边栏 220px 展开，可折叠为 64px
- **平板端 (768px-991px)**：侧边栏默认折叠，点击展开遮罩层
- **移动端 (<768px)**：侧边栏隐藏，通过汉堡菜单触发抽屉式导航

***

## 8. 组件状态规范

### 8.1 按钮状态

| 状态       | 背景色     | 边框色     | 文字色     |
| -------- | ------- | ------- | ------- |
| Default  | #ffffff | #dcdfe6 | #606266 |
| Hover    | #ecf5ff | #c6e2ff | #409eff |
| Active   | #409eff | #409eff | #ffffff |
| Focus    | #ecf5ff | #409eff | #409eff |
| Disabled | #f5f7fa | #e4e7ed | #a8abb2 |

### 8.2 表单状态

| 状态       | 边框色     | 阴影                                 |
| -------- | ------- | ---------------------------------- |
| Default  | #dcdfe6 | none                               |
| Hover    | #c0c4cc | none                               |
| Focus    | #409eff | 0 0 0 2px rgba(64, 158, 255, 0.2)  |
| Error    | #f56c6c | 0 0 0 2px rgba(245, 108, 108, 0.2) |
| Disabled | #e4e7ed | none                               |

### 8.3 反馈状态色

- **Info**: #909399
- **Success**: #67c23a
- **Warning**: #e6a23c
- **Error**: #f56c6c

***

## 9. 图标规范

### 9.1 图标尺寸

```css
--el-icon-size-small: 14px
--el-icon-size-base: 16px
--el-icon-size-medium: 18px
--el-icon-size-large: 20px
```

### 9.2 图标使用原则

- 使用 Element Plus 官方图标库
- 图标颜色跟随文字颜色或指定功能色
- 按钮内图标与文字间距 6px
- 导航菜单图标统一使用 18px

***

## 10. 布局规范

### 10.1 栅格系统

- 24列栅格
- 槽宽 (gutter)：20px
- 支持响应式断点

### 10.2 中后台布局结构

```
┌─────────────────────────────────────┐
│  Sidebar (220px)  │  Header (60px)   │
│                   ├──────────────────┤
│                   │  TagsView (40px) │
│                   ├──────────────────┤
│                   │                  │
│                   │  Main Content    │
│                   │                  │
└─────────────────────────────────────┘
```

### 10.3 布局尺寸

- 侧边栏宽度：220px（展开）/ 64px（折叠）
- 顶部导航高度：60px
- 标签页高度：40px
- 页面内容边距：20px

***

## 11. 命名规范

### 11.1 BEM 命名

```
Block: .el-button
Element: .el-button__icon
Modifier: .el-button--primary, .el-button--large
```

### 11.2 组件前缀

- Element Plus 组件：`el-`
- 业务组件：`app-` 或项目前缀

***

## 12. 无障碍设计

### 12.1 键盘导航

- 支持 Tab 键导航
- 支持 Enter/Space 激活
- 支持 Esc 关闭弹窗

### 12.2 对比度

- 正文对比度 ≥ 4.5:1
- 大文字对比度 ≥ 3:1
- 焦点状态清晰可见

### 12.3 ARIA 属性

- 表单元素使用正确的 label
- 动态内容使用 aria-live
- 图标按钮使用 aria-label

***

## 13. 动画规范

### 13.1 过渡时间

```css
--el-transition-duration: 0.3s
--el-transition-duration-fast: 0.2s
--el-transition-duration-slow: 0.4s
```

### 13.2 缓动函数

```css
--el-transition-function-ease-in-out-bezier: cubic-bezier(0.645, 0.045, 0.355, 1)
--el-transition-function-fast-bezier: cubic-bezier(0.23, 1, 0.32, 1)
```

### 13.3 动画使用场景

| 场景   | 动画类型              | 时长          |
| ---- | ----------------- | ----------- |
| 按钮悬停 | background-color  | 0.2s        |
| 菜单展开 | height/opacity    | 0.3s        |
| 弹窗出现 | transform/opacity | 0.3s        |
| 页面切换 | fade/slide        | 0.3s        |
| 加载状态 | rotate            | 1s infinite |

***

## 14. Z-Index 层级

```css
--el-index-normal: 1
--el-index-top: 1000
--el-index-popper: 2000
--el-index-mask: 3000
--el-index-message: 4000
```

### 14.1 层级使用

| 组件    | z-index | 说明   |
| ----- | ------- | ---- |
| 下拉菜单  | 2000    | 浮层基础 |
| 对话框遮罩 | 3000    | 模态遮罩 |
| 对话框   | 3100    | 模态内容 |
| 消息提示  | 4000    | 全局通知 |
| 加载层   | 5000    | 最高层级 |

***

## 15. 文件组织规范

```
admin/
├── index.html          # 主框架
├── login.html          # 登录页
├── register.html       # 注册页
├── pages/              # 功能页面
│   ├── user.html       # 用户管理
│   ├── role.html       # 角色管理
│   ├── dept.html       # 部门管理
│   ├── post.html       # 岗位管理
│   ├── menu.html       # 菜单管理
│   ├── operlog.html    # 操作日志
│   ├── loginlog.html   # 登录日志
│   ├── params.html     # 参数配置
│   ├── dict.html       # 字典管理
│   └── message.html    # 消息提醒
├── css/                # 样式文件
│   ├── variables.css   # CSS变量
│   ├── layout.css      # 布局样式
│   └── components.css  # 组件样式
└── js/                 # JS文件
    ├── utils.js        # 工具函数
    ├── api.js          # API接口
    └── components.js   # 公共组件
```

***

## 16. 代码规范

### 16.1 HTML 规范

- 使用语义化标签
- 属性使用双引号
- 自定义属性使用 data- 前缀

### 16.2 CSS 规范

- 使用 CSS 变量管理颜色和尺寸
- 类名使用小写，多单词用连字符
- 避免使用 !important

### 16.3 JS 规范

- 使用 ES6+ 语法
- 变量使用 const/let
- 函数使用箭头函数
- 使用 async/await 处理异步

***

## 17. 检查清单

### 17.1 色彩检查

- [ ] 主色调使用 #409EFF
- [ ] 功能色符合规范
- [ ] 文字对比度符合 WCAG 标准
- [ ] 禁用状态使用正确色值

### 17.2 字体检查

- [ ] 使用指定字体族
- [ ] 字号符合规范
- [ ] 行高适当
- [ ] 字重使用正确

### 17.3 布局检查

- [ ] 响应式适配正常
- [ ] 间距统一
- [ ] 圆角一致
- [ ] 阴影使用恰当

### 17.4 交互检查

- [ ] 悬停状态明显
- [ ] 点击反馈清晰
- [ ] 加载状态完整
- [ ] 错误提示明确

### 17.5 无障碍检查

- [ ] 支持键盘导航
- [ ] 焦点状态可见
- [ ] ARIA 属性正确
- [ ] 颜色不依赖信息传达

