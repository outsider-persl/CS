> move 是接口，需要自己实现move constructor

> 栈上分配的对象，无法手动释放

> `delete this` 只能操作使用 new 分配的对象（即在heap上的对象）

## 右值引用
> 左值引用和右值引用是C++11中引入的新特性，它们的主要区别在于引用的类型和绑定的对象。

> 左值引用是指对一个左值（可以取地址、有名字的变量或者对象、表达式或函数返回值）进行的引用，它的类型为T&，可以对其进行修改或者取地址等操作。

> 右值引用是指对一个右值（不能取地址、没有名字的临时对象或者表达式）进行的引用，它的类型为T&&，通常用于移动语义和完美转发等场景。右值引用的一个重要作用是支持移动语义，即通过将右值引用参数移动到目标对象中，避免了昂贵的内存拷贝操作，提高了程序的效率。

> 右值引用的意义在于提供了一种新的引用类型，使得我们可以更加高效地处理临时对象和表达式，同时也支持了新的语言特性，比如移动语义和完美转发等。右值引用还可以用于实现移动构造函数和移动赋值运算符等操作，从而提高程序的效率和性能。
