# 院校匹配系统

一个基于 Next.js 的智能化院校和专业匹配推荐平台。

## 项目特性

- 🎯 **分步流程设计** - 包含五个关键步骤的完整匹配流程
- 🔒 **步骤控制机制** - 只有完成前一步才能进入下一步
- 🎨 **现代化UI设计** - 使用Tailwind CSS构建的美观界面
- 📱 **响应式设计** - 适配各种设备尺寸
- ⚡ **组件化架构** - 清晰的组件分离和复用

## 系统流程

系统包含以下五个步骤：

1. **院校匹配** - 根据用户需求匹配合适的院校
2. **专业需求匹配** - 分析用户的专业需求和偏好
3. **专业背景匹配** - 评估用户的专业背景和能力
4. **生成推荐报告** - 基于前面的分析生成个性化推荐报告
5. **案例库校准** - 通过历史案例进行结果校准和优化

## 技术栈

- **框架**: Next.js 15+ (App Router)
- **语言**: TypeScript
- **样式**: Tailwind CSS
- **UI组件**: 自定义React组件
- **状态管理**: React Hooks (useState)

## 项目结构

```
src/
├── app/
│   ├── page.tsx          # 主页面
│   ├── layout.tsx        # 布局组件
│   └── globals.css       # 全局样式
└── components/
    ├── StepNavigation.tsx           # 步骤导航组件
    ├── SchoolMatching.tsx           # 院校匹配组件
    ├── MajorRequirementMatching.tsx # 专业需求匹配组件
    ├── MajorBackgroundMatching.tsx  # 专业背景匹配组件
    ├── GenerateReport.tsx           # 生成推荐报告组件
    ├── CaseCalibration.tsx          # 案例库校准组件
    └── index.ts                     # 组件导出索引
```

## 快速开始

### 安装依赖

```bash
npm install
```

### 启动开发服务器

```bash
npm run dev
```

在浏览器中打开 [http://localhost:3000](http://localhost:3000) 查看应用。

### 构建生产版本

```bash
npm run build
```

### 启动生产服务器

```bash
npm start
```

## 组件说明

### StepNavigation
步骤导航组件，负责：
- 显示五个步骤的导航栏
- 控制步骤的可点击状态
- 显示步骤完成状态

### 各步骤组件
每个步骤组件都包含：
- 标题和描述
- 占位内容区域（待实现具体功能）
- 完成按钮

## 状态管理

- `currentStep`: 当前激活的步骤
- `completedSteps`: 已完成的步骤数组
- 步骤控制逻辑：只有完成前一步才能进入下一步

## 样式设计

- 使用 Tailwind CSS 实现现代化设计
- 支持暗色模式
- 响应式布局
- 平滑过渡动画
- 自定义滚动条样式

## 后续开发

各个步骤组件目前为占位状态，可以根据业务需求添加具体功能：

1. **院校匹配**: 添加院校数据库和匹配算法
2. **专业需求匹配**: 添加需求分析表单和匹配逻辑
3. **专业背景匹配**: 添加背景评估功能
4. **生成推荐报告**: 添加报告生成和导出功能
5. **案例库校准**: 添加案例数据库和校准算法

## 许可证

MIT License

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
#   m a t c h S c h o o l  
 