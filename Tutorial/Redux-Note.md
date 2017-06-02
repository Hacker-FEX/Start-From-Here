# 一些你可能需要的文章：

1. [官方例子（吐血推荐，必看）](http://redux.js.org/docs/basics/)
2. [Redux 入门教程（一）：基本用法-阮一峰](http://www.ruanyifeng.com/blog/2016/09/redux_tutorial_part_one_basic_usages.html);

# 一些需要注意的点：

1. state保存在store里面，store的设计要扁平化，避免嵌套；

    > 官方建议：We suggest that you keep your state as normalized as possible, without any nesting. Keep every entity in an object stored with an ID as a key, and use IDs to reference it from other entities, or lists. Think of the app's state as a database.
    
2. reducer 为什么叫 reducer：It's called a reducer because it's the type of function you would pass to Array.prototype.reduce(reducer, ?initialValue). It's very important that the reducer stays pure. 
3. Reducer 里面不能改变参数state，而要返回一个新的state；
