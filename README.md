# 相关信息
1. 本项目使用了Backbone.js的知识。
2. 源代码在[这里](https://github.com/udacity/ud989-todo-app)，源码中需要的css已经给出
3. 课程在[这里](https://classroom.udacity.com/nanodegrees/nd001/parts/00113454014/modules/271165859175461/lessons/3525509902/concepts/35747685650923#)， 答案在课程中都已经给出，关键是思考的过程。

# 代码结构
## model
1. 数据：设置初始值，这里有priority，completed以及titile
2. 逻辑： 转换、验证、计算属性和访问控制，这里只涉及到了转换逻辑

## view
创建自定义的视图类，构建重载 render 函数，声明 events， 以及通过 tagName, className, 或 id 为视图指定根元素。

# 任务以及解决方案
## 任务完后在任务的末尾加上“it is done”字符串
在index文件上增加选择条件
## 增加编辑按钮
由于这是按钮，具有view的属性，所以需要在views的js代码中找，在todu-view.js中有dom events的集合，所以需要在那里实现编辑功能，在这里编辑功能的具体函数已经给出，调用就好。
最后不要忘了通过类名（edit-btn）在index.html上加上按钮
## 增加重要程度按钮：点击按钮文字变红
1. 在index上通过类名加上重要程度的按钮；
2. 在view的events集合内声明根元素以连接按钮以及需要编写的函数togglePriority；
3. 在view中的函数需要连接至model上；
4. 在model.js中仿照toggle函数写出自己的togglePriority函数并且设置好初始值；
5. 在todu-view.js的render--重载函数中仿照completed设置priority的初始值。
