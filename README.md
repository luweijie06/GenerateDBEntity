# Java 数据库实体生成器

这个 IntelliJ IDEA 插件简化了从数据库表生成 Java 实体类的过程。它提供了一个用户友好的界面，用于连接数据库、自定义实体生成设置，并创建带有适当注解的 Java 类。

## 功能特性

- 连接到 MySQL 数据库
- 从数据库表生成 Java 实体类
- 自定义 SQL 类型到 Java 类型的映射
- 选择 JPA、MyBatis-Plus 或无注解
- 可选使用 Lombok 以减少样板代码
- 从实体生成中排除特定字段
- 为所有生成的实体指定基类
- 选择生成实体的目标包

## 安装

1. 打开 IntelliJ IDEA
2. 转到 `File > Settings > Plugins`
3. 点击 `Marketplace`
4. 搜索 "GenerateDBEntity"
5. 点击 `Install`
6. 重启 IntelliJ IDEA

## 使用方法

1. 转到 `Tools > Database Configuration` 设置数据库连接和实体生成偏好。
2. 配置以下设置：
    - 数据库连接详情（主机、端口、数据库名、用户名、密码）
    - 注解风格（无注解、JPA 或 MyBatis-Plus）
    - 实体的基类
    - 生成实体的目标包
    - 自定义类型映射
    - 需要从生成中排除的字段
3. 点击 `Apply` 保存设置。
4. 要生成实体，右键点击您的项目或特定包，选择 `Generate Entity from Database`。
5. 选择您想要生成实体的表。
6. 生成的实体类将在指定的包中创建。

## 配置选项

### 数据库连接
- **主机**：MySQL 服务器的主机名
- **端口**：MySQL 服务器的端口号（默认为 3306）
- **数据库**：要连接的数据库名称
- **用户名**：MySQL 用户名
- **密码**：MySQL 密码

### 实体生成
- **注解选项**：选择无注解、JPA 注解或 MyBatis-Plus 注解
- **基类**：为所有生成的实体指定基类（可选）
- **包**：选择生成实体的目标包
- **使用 Lombok**：勾选此项使用 Lombok 注解以减少样板代码

### 类型映射
自定义 SQL 类型到 Java 类型的映射。您可以根据需要添加、修改或删除映射。

### 排除字段
指定要从所有生成的实体中排除的常见字段。这对于 'id'、'created_at'、'updated_at' 等字段很有用，如果这些字段由基类处理或者您不想在实体中包含它们。

## 系统要求

- IntelliJ IDEA 2023.1 或更高版本
## 贡献

欢迎贡献！请随时提交 Pull Request。

## 许可证

本项目采用 Apache-2.0  许可证 - 详情请见 [LICENSE](LICENSE) 文件。

## 支持

如果您遇到任何问题或有任何建议，请在 GitHub 仓库上开一个 issue。
