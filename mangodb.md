MongoDB 是一款非关系型数据库，以灵活的类 JSON 文档存储数据，
核心特点是无固定模式（同一集合中文档字段可不同），
其数据结构层级为 “数据库→集合→文档→字段”，与关系型数据库（RDBMS）的 
“数据库→表→行→列” 形成对应；文档支持字符串、整数、布尔值等多种数据类型，
还可包含数组和嵌套文档，且 MongoDB 会自动为每个文档分配唯一
ObjectId（也支持自定义 ID，如 ISBN），适配需灵活调整数据结构的场景。


就是简单的极少一下mangodb
如何往mangodb里面输入内容


4. 文档唯一标识（_id 字段）
自动生成：默认情况下，MongoDB 会为每个新增文档分配唯一的 12 字节 ObjectId，作为文档的唯一标识。
自定义支持：允许手动指定 _id 字段的值（如用书籍的 ISBN 作为唯一 ID），增强 ID 的业务关联性。




## mangodb creation
本文详细介绍了 MongoDB 中文档创建（插入）的核心方法，包括插入单个文档的insertOne()（支持指定或自动生成_id，自动生成时为唯一 ObjectId）、批量插入多个文档的insertMany()（默认有序插入，出错则停止；可通过ordered: false设为无序插入，出错仍继续），同时提及已弃用的 insert () 方法（兼容性差，推荐用前两者）；还以 “大学管理数据库” 为例，演示了在Departments“Instructors”“Courses”“Students”“Enrollments” 5 个集合中用insertMany()插入数据的具体操作，最后给出了新增院系、讲师等数据的实验任务。

1,insert 
insertMany的区别






use  mangodb campass

## 疑惑点
1.数据库里面的database name和collection name有什么区别


