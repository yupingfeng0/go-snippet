## Some Points of https://go.dev/doc/faq

1. runtime

> - 每一个Go程序都有一个runtime运行时库，实现了垃圾收集、并发、堆栈管理以及 Go语言的其他关键功能。
> - Go不包含虚拟机。它被编译成本地机器代码。
> - "runtime"只是对提供关键语言服务的库的称呼。

2. Unicode标识符

> - Go的规则--标识符必须是Unicode所定义的字母或数字。

3. X 特性

> - Go的设计着眼于编程的便利性、编译的速度、概念的正交性，以及支持并发和垃圾回收等功能的需要。
> - 你最喜欢的功能可能因为不合适而被遗漏，因为它影响了编译速度或设计的清晰度，或者因为它使基本的系统模型过于困难。

4. 泛型及其代价

> - Go 1.18 release加入了泛型。
> - 参见: https://go.dev/ref/spec
> - 多态编程在Go发布之初对该语言的目标并不重要，所以最初为了简化而被排除在外。
> - 泛型是很方便的，但它们的代价是类型系统和运行时间的复杂性。

5. Go的异常

> - Go采取了一种不同的方法。对于普通的错误处理，Go的多值返回使得报告错误很容易，而不需要重载返回值。
> - Go的几个内置函数`Defer`, `Panic`和 `Recover`，用来发出信号并从真正的特殊情况下恢复。
> - 参见: https://go.dev/blog/error-handling-and-go
> - 参见: https://go.dev/doc/articles/defer_panic_recover.html
> - 参见: https://blog.golang.org/errors-are-values
