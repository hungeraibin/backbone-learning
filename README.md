# backbone-learning
Backbone.js学习之旅

1.Hello World
- Model
1. 定义一个模型World，等待View层new World创建

- Collection
1. initialize绑定方法 - add remove reset sort
2. initialize参数：models options
3. 在View层new Worlds(models, optinos)传入

- View 
1. initialize实例化Collection，传入参数models, options与上面相对应
2. events绑定DOM事件
3. 在方法中new Model，通过Collection.add(model)联系
4. 方法参数为模型Model




