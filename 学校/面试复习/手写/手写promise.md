## 流程

1. 首先promise内部包含三种状态，并且定义了处理函数
2. 定义构造器会执行传入的函数同时传入定义的回调函数
3. 当resolve回调完成后会修改状态同时执行微任务队列
4. then方法会接收onfulfilled和onrejected方法，同时返回一个promise对象，方法接收resolve和reject方法并且将传入的方法放入执行队列之后调用执行函数，执行函数会调用process.nextTick异步执行处理
5. 注意传入的执行器会接收返回的参数 value

> 1. 构造函数传入成功和失败回调
> 2. resolve调用执行队列
> 3. reject调用后执行异步队列
> 4. then传入方法到异步队列中执行
