#聚课盒子 
[传送门](http://www.gkrbox.com)
聚课盒子是一个课程搜索网站，现已完成对慕课网，极客学院，腾讯课堂等多家在线教育平台课程信息的积累和搜索服务。
由于敏感原因，该项目暂不开源。


####version 1.0
#####php版本(已暂停维护)
 * 前端使用jquery+vue+bootstrap+grunt。
 * 后端使用smarty模板引擎进行渲染。
 * 移动端使用zepto+vue,并采用了fastclick解决点击延迟问题。


####version 2.1
#####使用node.js重写后端，新增node.js版本
 * 使用node.js中的主流框架express，所有业务全部实现异步处理。
 * 使用ejs模板引擎进行渲染。
 * 经初步测试，在现有学生版ubuntu云服务器的环境下，可承受的并发量与页面处理速度均优于php（其中对相同并发量的处理效果约为php的5倍），而数据传输速率低于php。
 
 
####version 3.0
#####该版本主要对移动端进行了重构
 * 使用ionic框架重构移动端前端，去掉了ejs模板引擎，全部改用angular+ajax。
 * 添加了内联iframe显示跳转的课程页面（极客学院由于设置了S-Iframe-Options:SAMEORIGIN,无法在iframe中显示，其他均正常）
 
####version 3.1
#####主要对搜索功能做了优化
 * 新增了中文分词模块 [Segment](https://github.com/leizongmin/node-segment)。
 * 添加”删除重复项“逻辑。
 * 更换了网站Logo
 
####version 3.2
#####主要对PC端代码进行了重构
 * 使用express.router，新增moment模块。
 * 前端用vue.js作组件化
 * 使用Webpack进行模块化及自动化构建。
 
####version 3.3
#####主要对移动端代码进行了重构
 * 使用angular.directive 组件化
 * 去掉部分jquery函数，采用angular原生写法。（进行中）