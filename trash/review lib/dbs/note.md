## 数据模型
概念模型：E-R图
逻辑模型：（网状、层次、关系）

## 三级模式
外模式：                        **视图**（面向用户）
模式（or 逻辑模式 or 概念模式）：   **表** （面向开发者）
内模式：                        **索引**（面向dba）

## 二级映射
| **功能**     | **映像层级**      | **数据独立性类型** |
| ------------ | ----------------- | ------------------ |
| 外部映像功能 | 外模式 ↔ 概念模式 | 逻辑数据独立性     |
| 内部映像功能 | 概念模式 ↔ 内模式 | 物理数据独立性     |

## 数据库安全性（数据库用户管理）

> 数据库用户，权限等，略

## 数据库完整性（约束）
> 也就是约束，foreignkey check,not null check 等

## 数据库设计的步骤

[查看详细步骤(选填题知识点.pdf)](./选填题知识点.pdf)

## 数据库设计过程总结

### 1. 需求分析
- 确定业务需求，理解数据和操作的需求。
- 与用户沟通，收集数据项、功能要求及性能目标。
- 定义系统需要管理的信息及其处理方式。

### 2. 概念结构设计
- 使用实体-关系（E-R）模型来抽象表示数据及其关系。
- 定义实体、属性和实体间的关系。
- 创建概念设计图（E-R图），以便更清晰地理解数据的结构和逻辑。

### 3. 逻辑结构设计
- 将概念设计中的实体转化为关系模型（表结构）。
- 确定表中的字段、数据类型，并定义主键、外键及其他约束。
- 对表进行规范化处理，确保数据一致性和减少冗余。

### 4. 物理结构设计
- 将逻辑设计映射到实际的数据库管理系统（DBMS）。
- 选择合适的数据类型、索引、存储方案等优化数据库性能。
- 设定分区、存储引擎等，以适应大数据量和高并发的需求。

### 5. 数据库实施
- 在数据库管理系统中创建数据库和表结构。
- 插入初始数据并进行初步测试，确保数据库结构正确实现。
- 配置权限、备份策略以及其他数据库管理操作。

### 6. 数据库运行和维护
- 监控数据库的运行状态，进行性能调优。
- 定期备份数据并检查数据库健康状态。
- 根据业务需求变化，进行数据库升级、优化或调整。

> 1   调研
> 2-4 设计
> 5   设计转数据
> 6   运行、维护

## 数据库编程

## 数据库恢复技术（事务）

[查看详细步骤(选填题知识点.pdf)](./选填题知识点.pdf)
