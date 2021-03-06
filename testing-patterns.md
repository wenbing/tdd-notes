# Testing Patterns

## Mock Object

如果在测试中需要用到一个昂贵且复杂的资源对象，那么创建它一定不是一个好主意，除非它就是要测试的对象。
这里的解决方法通常是 Mock。广义的 Mock 有 3 类。

1. 为所有未实现的接口和方法提供空实现，事实上什么也不做，且全部返回类似null的结构，被称为Stub(存根实现)。

2. 为所有未实现的接口和方法提供写死的返回值，比如一个或多个常量，或将参数毫无变化地返回出去，被称为Fake(伪实现)。

3. 利用某种运行时工具动态地生成一个对象，使其实现预定的接口和方法，当该方法被调用时，这种运行时工具会将调用信息保存下来供测试用例检验，
或触发其他的测试代码，这种方式依赖于所使用的语言是否提供了这样的机制。这一类又被称为狭义的Mock。

# Log String

编写日志便于了解代码的执行序列

## Crash Test Dummy

编写一个空的测试用例，只做抛出异常这一件事，看看错误处理系统是如何工作的

## Broken Test

提交前请务必保证自己所有的测试用例都能通过

## Clean Check-in

提交前确定下其他人的测试都可以跑通

