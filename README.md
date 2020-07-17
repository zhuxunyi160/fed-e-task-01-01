# fed-e-task-01-01

##1、下面关于虚拟 DOM 的说法正确的是：
A. 使用虚拟 DOM 不需要手动操作 DOM，可以极大的提高程序的性能。

B. 使用虚拟 DOM 不需要手动操作 DOM，可以极大的提高开发效率。

C. 虚拟 DOM 可以维护程序的状态，通过对比两次状态的差异更新真实 DOM。

D. 虚拟 DOM 本质上是 JavaScript 对象，可以跨平台，例如服务器渲染、Weex 开发等。

答案 :  C


##2、下面关于 Snabbdom 库的描述错误的是：
A. Snabbdom 库是一个高效的虚拟 DOM 库，Vue.js 的虚拟 DOM 借鉴了 Snabbdom 库。

B. 使用 h() 函数创建 VNode 对象，描述真实 DOM 结构。

C. Snabbdom 库本身可以处理 DOM 的属性、事件、样式等操作。

D. 使用 patch(oldVnode, null) 可以清空页面元素

答案 :  D

简答题
1、请简述 patchVnode 函数的执行过程。
执行prepatch钩子函数
判断是否和老vnode相同
执行update函数

判断vnode.text 是否定义
如果未定义
判断判断新老节点是否有children
都有的话，使用diff更新子节点，
如果新的有children 老的没有children
如果老节点有text,清空dom元素

如果定义了
老节点有children 移除
设置textcontnete为vnode.text

z最后执行postpatch


