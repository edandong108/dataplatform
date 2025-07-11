# 数据平台权限管理系统

## 项目概述

这是一个B端数据平台权限管理系统的HTML原型，采用现代化的UI设计和完整的权限管理功能。

## 功能模块

### 1. 项目管理
管理数据平台中的各个项目，包括项目信息、数据资源绑定和项目管理员分配。

**示例项目数据：**
- **客户数据中台**：整合全渠道客户数据，构建360度客户画像
- **营销效果分析平台**：实时监控营销活动效果，提供ROI分析
- **供应链数据治理**：建立供应链数据标准，监控数据质量
- **财务报表自动化**：自动化财务数据收集和报表生成
- **用户行为分析系统**：收集分析用户行为数据，优化用户体验

### 2. 角色管理
定义和管理系统中的各种角色及其权限。

**预设角色：**
- **平台管理员**：拥有所有平台管理权限
- **项目管理员**：管理分配的项目和项目内用户权限
- **数据分析师**：负责业务数据分析，制作报表和看板
- **数据开发工程师**：负责数据模型设计、ETL开发和数据质量管理
- **业务用户**：业务部门用户，主要查看相关业务数据
- **只读用户**：只能查看数据和报表，适用于外部合作伙伴

**权限类别：**
- 数据看板相关：查看、管理、导出
- 数据源相关：查看、管理、配置连接
- 数据模型相关：查看、管理、发布
- 查询任务相关：执行、管理、查看历史
- 任务调度相关：查看、管理、监控执行
- 数据质量相关：查看报告、管理规则、配置监控
- 系统管理相关：用户行为日志、系统配置、系统监控
- 平台管理相关：管理用户、角色、项目

### 3. 用户管理
管理平台用户账户，包括用户信息、状态和所属项目。

**示例用户数据：**
- **admin**：系统管理员账户
- **张伟**：数据平台负责人
- **李娜**：营销数据分析师
- **王强**：供应链数据工程师
- **刘敏**：财务数据分析师
- **陈杰**：已禁用用户
- **赵丽**：业务数据分析师
- **孙涛**：用户行为分析工程师

### 4. 项目用户分配
管理项目内的用户分配和角色权限。

**分配示例：**
- 客户数据中台：张伟(项目管理员)、李娜(数据分析师)、赵丽(数据工程师)
- 营销效果分析平台：李娜(项目管理员)、王强(数据分析师)、孙涛(业务用户)
- 供应链数据治理：王强(项目管理员)、刘敏(数据工程师)
- 财务报表自动化：刘敏(项目管理员)、赵丽(数据分析师)
- 用户行为分析系统：张伟(项目管理员)、孙涛(数据工程师)、李娜(业务用户)

## 技术特性

- **响应式设计**：采用现代化的科技蓝主题
- **数据持久化**：使用localStorage模拟数据存储
- **完整CRUD操作**：支持数据的增删改查
- **数据关联**：实现用户、项目、角色之间的关联关系
- **权限控制**：核心数据保护，防止误删除
- **数据验证**：完善的表单验证和数据完整性检查

## 使用说明

1. 打开 `index.html` 进入系统主页
2. 使用左侧导航菜单切换不同功能模块
3. 如需重置示例数据，可访问 `clear_data.html` 清理localStorage

## 数据重置

如果需要查看最新的示例数据，请：
1. 访问 `clear_data.html`
2. 点击"清理所有数据"按钮
3. 返回主页，系统将自动加载新的示例数据

## 文件结构

```
├── index.html                    # 主页面（左侧导航+iframe内容区）
├── project_management.html       # 项目管理模块
├── role_management.html          # 角色管理模块
├── user_management.html          # 用户管理模块
├── project_user_management.html  # 项目用户分配模块
├── clear_data.html              # 数据清理工具
└── README.md                    # 项目说明文档
```

## 设计理念

本系统采用现代化的B端产品设计理念：
- **简洁明了**：清晰的信息层级和操作流程
- **一致性**：统一的视觉风格和交互模式
- **易用性**：直观的操作界面和友好的错误提示
- **专业性**：符合企业级应用的设计标准 