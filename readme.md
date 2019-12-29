### 基于FreeMarker、mysql的代码生成器

> 注意：这里的FreeMarker模板是作者个人的模板，继承类和忽略属性都是作者的习惯，请自行修改

> 

#### 使用方式：
    
**Generate main方法启动**，需配置参数如下

- 包名：packageName
- 模块名：moduleName
- 类名：className
- 模块功能名称：functionName （用于类备注以及文本描述）
- 类作者：classAuthor
- 数据库连接串：dbCoon
- 数据库名：dbName (数据库名理论上可以从连接串中截取，但懒得做)
- 数据库用户名：user
- 数据库连接驱动：driver
- 表名：tableName
- 代码输出路径：filePath
 

#### 模板位置
> **resources/freemakerTpl**，配置位置在**core/FreeMarkerTemplateUtils/static**

#### 模板生成方法
> FreemarkerInit具体生成代码中，作者忽略了BaseEntity内的字段，具体详见 **FreemarkerInit.getDataMap**
