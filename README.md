# excel_export_import
## 简介
### 为什么开发
* 做系统的时候，经常需要对文件导出以及excel的导入。我们最熟悉的是便是poi。但是poi本身只是提供了对excel的处理，并没有一些组件可以对其进一步的封装
* 我们使用的时候，当导出时，比如字段A，B,就需要写个代码处理AB，下次业务说换成B，又要修改大量代码，或者说不要导出excel，导出csv，也让开发觉得繁琐。
* excel的导入就更麻烦了，excel的导入涉及到两个方面问题。
** 同导出一样，经常字段更改
** 无法控制excel的输入格式，就算你跟用户强调了输入框必需什么格式，实际操作仍然有不同格式，就需要开发进行代码对不同格式进行操作
### 功能
* 使用xml进行数据类型，数据key，数据开始行，进行配置，方便维护，同时写更少的代码
* 导出，调用方法，把自己产生list or map 转化成 对应的excel或者csv 
* 读取excel，转换成相应的map或者其他内容(其他内容暂时还未开发)。目前只有map