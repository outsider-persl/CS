# use c/cpp in vscode

*简单项目创建默认配置文件，修改一下target目录即可*
```cpp
# tasks.json
# args: 将调试文件整合到当前目录的上级目录target中
"${fileDirname}/../target/${fileBasenameNoExtension}"
```
*复杂的项目建议使用cmake*
# 移动语义与 std::move

## 1. 移动语义概述
- **移动语义** 允许资源的所有权在对象之间转移，避免不必要的复制。
- `std::move` 是一种将左值转换为右值的工具，通常用于启用移动构造函数和移动赋值操作符。

## 2. `std::move` 的作用
- 调用 `std::move(obj)` 会将 `obj` 转换为右值引用，使其可以被移动构造函数或移动赋值操作符接收。
- `std::move` 不会进行任何实际的移动，只是进行类型转换。

## 3. 移动构造函数
- 在移动构造函数中，资源的所有权从源对象转移到新对象。
- 源对象的指针应被置为 `nullptr`，以防止双重释放。

### 示例
```cpp
MyClass(MyClass&& other) noexcept : data(other.data) {
    other.data = nullptr;  // 使源对象的指针为空
}
```
> 总结
`std::move` 实现了资源的转移，但如果不在移动构造函数或移动赋值运算符中显式释放原对象的资源，就只是避免了复制，而没有真正转移所有权。因此，需要手动管理资源以防止内存泄漏或悬挂指针。