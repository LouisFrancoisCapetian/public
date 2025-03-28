# 影视论坛系统

基于 SpringBoot 3 + Vue 3 的前后端分离影视论坛系统。

## 技术栈

### 后端
- SpringBoot 3.0.2
- MyBatis
- MySQL 5.7
- Redis (缓存)
- JWT (认证)
- Spring Security (权限)

### 前端
- Vue 3.5.13
- Element Plus
- Axios
- Vue Router
- Pinia

## 项目结构

```
com.example/
├── config/        # 配置类
│   ├── SecurityConfig.java     # Spring Security配置
│   ├── JwtConfig.java         # JWT配置
│   └── RedisConfig.java       # Redis配置
│
├── controller/    # 控制器层，处理HTTP请求
│   ├── AuthController.java    # 认证相关接口
│   ├── UserController.java    # 用户相关接口
│   └── PostController.java    # 帖子相关接口
│
├── service/       # 服务层，业务逻辑
│   ├── impl/     # 服务实现类
│   ├── UserService.java       # 用户服务接口
│   └── PostService.java       # 帖子服务接口
│
├── mapper/        # MyBatis映射接口
│   ├── UserMapper.java        # 用户数据访问
│   └── PostMapper.java        # 帖子数据访问
│
├── entity/        # 实体类，与数据库表对应
│   ├── User.java             # 用户实体
│   └── Post.java             # 帖子实体
│
├── dto/           # 数据传输对象，接收前端请求参数
│   ├── LoginDTO.java         # 登录参数
│   └── RegisterDTO.java      # 注册参数
│
├── vo/            # 视图对象，返回给前端的数据
│   ├── UserVO.java           # 用户信息
│   └── PostVO.java           # 帖子信息
│
├── common/        # 公共组件
│   ├── Result.java           # 统一响应格式
│   ├── ResultCode.java       # 响应状态码
│   └── GlobalExceptionHandler.java  # 全局异常处理
│
├── utils/         # 工具类
│   ├── JwtUtils.java         # JWT工具类
│   └── RedisUtils.java       # Redis工具类
│
└── SpringbootApplication.java # 启动类

```

## 功能模块

### 1. 用户认证
- 用户注册
- 用户登录
- 用户登出
- JWT认证
- 权限控制

### 2. 用户管理
- 用户信息管理
- 用户状态管理
- 用户活跃度统计

### 3. 影视资源
- 影视信息展示
- 分类筛选
- 评分系统
- 资源上传
- 资源审核

### 4. 社区互动
- 发布帖子
- 评论互动
- 点赞收藏
- 举报管理

### 5. 个人中心
- 基本信息修改
- 收藏管理
- 发布历史
- 浏览历史

### 6. 管理后台
- 用户管理
- 内容审核
- 数据统计
- 系统配置

## 开发环境
- JDK 21(IDEA使用java17)
- Maven 3.9.9
- Node.js v20.15.1
- MySQL 5.7.39
- IDEA 2023.3.8
