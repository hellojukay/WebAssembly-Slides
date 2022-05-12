---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# WebAssembly 生态介绍

BBFE--WuHan 李聪

---

## How Javascript works?
```javascript
sum(1,3)

function sum(a,b) {
    return a + b
}
```

Read more about [How javascript works?](https://coralogix.com/blog/how-js-works-behind-the-scenes%E2%80%8A-%E2%80%8Athe-engine/)

---

<img src="/js_compile.png"/>

---

### Performance
因为 Javascript 的运行机制限制，Javascript 在运行速度上很难又较大的突破了。

--- 

<img src="/node_benchmark.png"/>

---

# ASM.js
- ASM 是 Javascript 的严格的子集，执行速度更快
- ASM.js 有 emscripten 编译器将其他静态语言编译而成
- https://zh.m.wikipedia.org/zh-hans/Asm.js
- https://github.com/emscripten-core/emscripten

---

<img src="/asmjs_benchmark.png" />

---

# WebAssembly是什么

WebAssembly 本身并不是一种编程语言,是一种高效的字节码标准，可以在现代的网络浏览器中运行 。JAVA 能运行在哪里，取决于 JVM 虚拟机能运行在哪里，同样的 WebAssembly 虚拟机能在哪里运行，WebAssembly 就能在哪里运行。

---

<img src="/JVM.png" />

---

# WASI
WASI 全称是 WebAssembly System Interface。

- javascript 通过 DOM 和 BOM 和浏览器交互, 通过 Node.js 接口访问操作系统接口
- WebAssembly 通过 WASI 访问操作系统接口，走出了浏览器的局限

---

# 现状
- 各种编程语言都能编译成 WebAssembly 字节码，C/C++, C#, Rust, GO, Python 等
- https://www.assemblyscript.org/ (typescript转WebAssembly)
- https://wasi.dev/ (WebAssembly System Interface)
- https://wapm.io/ (WebAssembly的包管理中心)

---
layout: center
class: text-center
---

# Go 与 WebAssembly
- https://github.com/hellojukay/WebAssembly-Demo

---

# Learn More

[Documentations](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev) · [Showcases](https://sli.dev/showcases.html)
