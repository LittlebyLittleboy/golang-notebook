### Go语言的编码规范

---
- **<a href='#1'>1.注释方式</a>**
- **<a href='#2'>2.命名方式</a>**
- **<a href='#3'>3.控制结构</a>**
- **<a href='#4'>4.函数结构</a>**
- **<a href='#5'>5.错误处理</a>**
- **<a href='#6'>6.panic</a>**
- **<a href='#7'>7.import</a>**
- **<a href='#8'>8.缩写</a>**
- **<a href='#9'>9.参数传递</a>**
- **<a href='#10'>10.接受者</a>**
- **<a href='#11'>11.单行最长字符</a>**

---
**<a id='1'>1.注释方式</a>**
```
简介：用于注解说明程序的文字就是注释，注释提高代码的可阅读性，注释是一个程序员必须要具有的良好的编码习惯。
```
```
注释：行注释和块注释
①.行注释
基本语法：// 注释内容
代码实例：
// 定义主函数
func main(){
	// 打印内容
	fmt.Println("Hello,world.")
}

②.块注释
基本语法：/* 注释内容 */
代码实例：
/*
fmt.Println("hahahahaha")
fmt.Println("hehehehehe")
*/

细节：
①.对于行注释和块注释，注释部分不会被编译器执行。
②.注意事项：块注释不允许有块注释嵌套
```
**<a id='2'>2.命名方式</a>**
```
简介：
使用短命名，长名字并不会自动使得事物更易读，文档注释会比格外长的名字更有用。
```
```
包名：
包名应该为小写单词，不要使用下划线或者混合大小写。
```
```
接口名：
单个函数的接口名以"er"作为后缀，如Reader,Writer
```
```
接口的实现则去掉“er”
type Reader interface {
        Read(p []byte) (n int, err error)
}
```
```
两个函数的接口名综合两个函数名
type WriteFlusher interface {
    Write([]byte) (int, error)
    Flush() error
}
```
```
三个以上函数的接口名，类似于结构体名
type Car interface {
    Start([]byte)
    Stop() error
    Recover()
}
```
```
混合大小写
采用驼峰式命名
MixedCaps 大写开头，可导出
mixedCaps 小写开头，不可导出

变量
全局变量：驼峰式，结合是否可导出确定首字母大小写
参数传递：驼峰式，小写字母开头
局部变量：下划线形式
```
**<a id='3'>3.控制结构</a>**
```
if:if接受初始化语句，约定如下方式建立局部变量

if err := file.Chmod(0664); err != nil {
    return err
}
```
```
for:采用短声明建立局部变量

sum := 0
for i := 0; i < 10; i++ {
    sum += i
}
```
```
range:如果只需要第一项（key），就丢弃第二个：

for key := range m {
    if key.expired() {
        delete(m, key)
    }
}
如果只需要第二项，则把第一项置为下划线

sum := 0
for _, value := range array {
    sum += value
}
```
```
return:尽早return：一旦有错误发生，马上返回

f, err := os.Open(name)
if err != nil {
    return err
}
d, err := f.Stat()
if err != nil {
    f.Close()
    return err
}
codeUsing(f, d)
```

**<a id='4'>4.函数结构</a>**
```
函数采用命名的多值返回
传入变量和返回变量以小写字母开头
func nextInt(b []byte, pos int) (value, nextPos int) {
	......
}
```
**<a id='5'>5.错误处理</a>**
```
error作为函数的值返回,必须对error进行处理
错误描述如果是英文必须为小写，不需要标点结尾
```
```
采用独立的错误流进行处理
不要采用这种方式

    if err != nil {
        // error handling
    } else {
        // normal code
    }
而要采用下面的方式

    if err != nil {
        // error handling
        return // or continue, etc.
    }
    // normal code
如果返回值需要初始化，则采用下面的方式

x, err := f()
if err != nil {
    // error handling
    return
}
// use x
```
**<a id='6'>6.panic</a>**
```
尽量不要使用panic，除非你知道你在做什么
```
**<a id='7'>7.import</a>**
```
对import的包进行分组管理，而且标准库作为第一组

package main

import (
    "fmt"
    "hash/adler32"
    "os"

    "appengine/user"
    "appengine/foo"

    "code.google.com/p/x/y"
    "github.com/foo/bar"
)
```
**<a id='8'>8.缩写</a>**
```
采用全部大写或者全部小写来表示缩写单词
比如对于url这个单词，不要使UrlPony
而要使用urlPony 或者 URLPony
```
**<a id='9'>9.参数传递</a>**
```
对于少量数据，不要传递指针
对于大量数据的struct可以考虑使用指针
传入参数是map，slice，chan不要传递指针
因为map，slice，chan是引用类型，不需要传递指针的指针
```
**<a id='10'>10.接受者</a>**
```
名称:
统一采用单字母'p'而不是this，me或者self

    type T struct{} 

    func (p *T)Get(){}
```
```
类型
对于go初学者，接受者的类型如果不清楚，统一采用指针型

func (p *T)Get(){}
而不是

func (p T)Get(){}
```
```
在某些情况下，出于性能的考虑，或者类型本来就是引用类型，有一些特例

如果接收者是map,slice或者chan，不要用指针传递
//Map
package main

import (
    "fmt"
)

type mp map[string]string

func (m mp) Set(k, v string) {
    m[k] = v
}

func main() {
    m := make(mp)
    m.Set("k", "v")
    fmt.Println(m)
}
//Channel
package main

import (
    "fmt"
)

type ch chan interface{}

func (c ch) Push(i interface{}) {
    c <- i
}

func (c ch) Pop() interface{} {
    return <-c
}

func main() {
    c := make(ch, 1)
    c.Push("i")
    fmt.Println(c.Pop())
}


<pre><code><br /></code></pre>

如果需要对slice进行修改，通过返回值的方式重新赋值
//Slice
package main

import (
    "fmt"
)

type slice []byte

func main() {
    s := make(slice, 0)
    s = s.addOne(42)
    fmt.Println(s)
}

func (s slice) addOne(b byte) []byte {
    return append(s, b)
}

<pre><code><br /></code></pre>

如果接收者是含有sync.Mutex或者类似同步字段的结构体，必须使用指针传递避免复制
package main

import (
    "sync"
)

type T struct {
    m sync.Mutex
}

func (t *T) lock() {
    t.m.Lock()
}

/*
Wrong !!!
func (t T) lock() {
    t.m.Lock()
}
*/

func main() {
    t := new(T)
    t.lock()
}

<pre><code><br /></code></pre>

如果接收者是大的结构体或者数组，使用指针传递会更有效率。

package main

import (
    "fmt"
)

type T struct {
    data [1024]byte
}

func (t *T) Get() byte {
    return t.data[0]
}

func main() {
    t := new(T)
    fmt.Println(t.Get())
}
```

**<a id='11'>11.单行最长字符</a>**
```
一行最长不超过80个字符，超过的请使用换行展示，尽量保持格式优雅。
```

---
**参考网络文章**
[**Go语言编码规范**](https://segmentfault.com/a/1190000000464394#item-2)
[**Go语言官方教程**](https://go-zh.org/)

---
**作者：张电永**
**时间：2020-02-07 23:59:56 星期五**