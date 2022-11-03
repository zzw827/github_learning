# React For Redux Mbox Exercise

本项目用于练习 Redux 和 Mbox with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

React中的状态如何进行管理的呢？

1.组件内部私有状态  2.通过 Mobx redux 这种 进行共享state

使用 redux Mbox 这种东西  主要是 实现数据共享 以及 (对共享数据的规范处理)


不使用Context的时候 那么就每层传递props 一层一层传递下去

使用Context的时候就可以直接再第一层 声明 然后每层都可以使用

### `认识Redux`
1.Redux 是什么？
使用action 的事件来管理和更新应用状态的工具库,它以集中式Store的方式进行管理 共享数据 
一个公共状态的管理工具

2.我们的应用程序是否需要redux?
 
 1.用户的使用方式比较复杂
 2.与服务器大量交互的
 3.多个用户之间可以协作的

 如果你不知道 是否需要 那就是不需要
 如果你在想有没有  一个 存放共享数据的地方 那你就需要redux

### `Redux核心思想`
Store 存放公共state 
View中的 state 从Store中获取
View通过 Action 触发 
Action携带 type类型和 数据 
Reducer 处理Action  Store再更换 new State 
之后自动重新渲染
### `redux-thunk`

1.1个redux的中间件
2.让 dispatch 参数支持 Function
3.一定程度上优化了应用中的异步处理逻辑

其实 还是想把 异步逻辑 与 视图层 给分离开来
直接可以return 一个 function 进行处理




## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
