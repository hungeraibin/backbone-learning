# backbone-learning
Backbone.js学习之旅

1.Hello World
- Model
1. 定义一个模型World，等待View层new World创建

- Collection
1. initialize绑定方法 - add remove reset sort 参数model
2. initialize参数：models options
3. 在View层new Worlds(models, optinos)传入

- View 
1. initialize实例化Collection，传入参数models, options与上面相对应
2. events绑定DOM事件
3. 在方法中new Model，通过Collection.add(model)联系
4. 集合add方法，回调参数为模型Model

2.Model
1. initialize绑定方法 - change change:[attribute] destory invalid
2. invalid回调参数 - model error
3. validate参数attributes指模型对象，返回error
4. save - POST发送到服务器，触发验证
5. fetch - GET从服务器上要数据
6. success参数 - model response options
7. url和urlRoot

3.Collecton
1. add添加模型，each方法循环遍历模型
2. fetch获取数据，sucess参数 - collection response options
3. 集合绑定reset方法，fetch设置 reset: true
4. create发送数据，触发add sync事件

4.Router
1. routes设置 ":"代表对应路径，"*"代表所有路径，传入函数参数
2. history.start 监控 hashchange 事件并分配路由
3. app_router.navigate 手动触发router

5.View
1. 模板引擎 <% %> <%= %>
2. initialize 主要执行this.render,传递模板所需参数
3. render 参数context，传递给模板template参数
4. template编译模板，接受参数是所需编译的模板
5. events 绑定DOM，传递参数为event