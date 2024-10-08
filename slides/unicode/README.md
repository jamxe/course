# Unicode 是什么

## 字符集

字符集：从 字符 到 整数 的映射

Unicode 为每个字符都对应了一个整数。

计算机存储字符时，实际上是存储了那个对应的整数。

一段文字（字符串）实际上就是所有字符对应整数的数组。

这些整数就被称为 *码点 (code point)*。

## 字符编码

Unicode 字符集只是指定了整数，没有规定整数如何在内存中存在。

字符编码：规定抽象的 整数 如何序列化为计算机可直接存储的 字节。

- UTF-32：每个 Unicode 字符 都用 1 个 `uint32_t` 存储。
- UTF-16：每个 Unicode 字符 都用 1 至 2 个 `uint16_t` 存储。
- UTF-8：每个 Unicode 字符 都用 1 至 4 个 `uint8_t` 存储。

# C/C++ 中的字符类型
