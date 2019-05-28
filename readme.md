# rust-lang/rustlings [![explain]][source] [![translate-svg]][translate-list]

<!-- [![size-img]][size] -->

[explain]: http://llever.com/explain.svg
[source]: https://github.com/chinanf-boy/Source-Explain
[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list
[size-img]: https://packagephobia.now.sh/badge?p=Name
[size]: https://packagephobia.now.sh/result?p=Name

「 desc 」

[中文](./readme.md) | [english](https://github.com/rust-lang/rustlings)

---

## 校对 🀄️

<!-- doc-templite START generated -->
<!-- repo = 'rust-lang/rustlings' -->
<!-- commit = '41170ce3411b2029d8906dcee16548f00d90ca24' -->
<!-- time = '2019-05-26' -->

| 翻译的原文 | 与日期        | 最新更新 | 更多                       |
| ---------- | ------------- | -------- | -------------------------- |
| [commit]   | ⏰ 2019-05-26 | ![last]  | [中文翻译][translate-list] |

[last]: https://img.shields.io/github/last-commit/rust-lang/rustlings.svg
[commit]: https://github.com/rust-lang/rustlings/tree/41170ce3411b2029d8906dcee16548f00d90ca24

<!-- doc-templite END generated -->

### 贡献

欢迎 👏 勘误/校对/更新贡献 😊 [具体贡献请看](https://github.com/chinanf-boy/chinese-translate-list#贡献)

## 生活

[hIf help, **buy** me coffee —— 营养跟不上了，给我来瓶营养快线吧! 💰](https://github.com/chinanf-boy/live-need-money)

---

![crab pet](http://i.imgur.com/LbZJgmm.gif)

# 沙沙 🦀❤️

问候和欢迎`rustlings`。这个项目包含一些小练习，让你习惯于阅读和编写 Rust 代码。这包括读取和响应编译器消息！

_...寻找旧的，基于网络的 Rustlings 版本？尝试[这里](https://github.com/rust-lang/rustlings/tree/rustlings-1)_

或者，对于第一次 Rust 学习者，还有其他几种资源：

- [the book](https://doc.rust-lang.org/book/index.html)- 学习 Rust 最全面的资源，但有时候有点理论。你将和 Rustlings 一起使用它！
- [Rust 示例](https://doc.rust-lang.org/rust-by-example/index.html)- 通过解决小练习来学习 Rust！这几乎就像`rustlings`，但在线

## 入门

_注意：如果您使用的是 MacOS，请确保已通过键入来安装 Xcode 及其开发人员工具`xcode-select --install`。_

_注意：如果您安装了 Xcode 10+，则还需要安装找到的软件包文件`/Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg`。_

您需要安装 Rust。你可以通过访问获得它<https://rustup.rs>。这也将安装 Cargo，Rust 包裹/项目经理。

## MacOS / Linux

赶紧跑：

```bash
curl -L https://git.io/rustlings | bash
# Or if you want it to be installed to a different path:
curl -L https://git.io/rustlings | bash -s mypath/
```

这将安装 Rustlings 并允许您访问`rustlings`命令。运行它开始！

## 在 Windows /手动

基本上：克隆存储库，签出到最新标签，运行`cargo install`。

```bash
git clone https://github.com/rust-lang/rustlings
cd rustlings
git checkout tags/1.0.0 # or whatever the latest version is (find out at https://github.com/rust-lang/rustlings/releases/latest)
cargo install --force --path .
```

与上面相同，运行`rustlings`开始。

## 做练习

练习按主题排序，可以在子目录中找到`rustlings/exercises/<topic>`。对于每个主题，都有一个附加的 README 文件，其中包含一些资源，可帮助您开始使用该主题。我们真的建议您在开始之前先看看它们。

任务很简单。大多数练习包含一个错误，使其无法编译，并由你来解决它！有些练习也是作为测试运行的，但是沙沙作为处理它们都是一样的。要按建议的顺序运行练习，请执行：

```bash
rustlings verify
```

这将尝试按预定顺序验证每项练习的完成情况（我们认为最适合新手的）。如果你不想重新运行`verify`每次更改文件时，都可以运行：

```bash
rustlings watch
```

这将与验证相同，但在运行后不会退出，而是在您更改文件后立即自动重新运行`exercises/`目录。

如果您想通过自己的订单，或者只想验证一个练习，您可以运行：

```bash
rustlings run exercises/path/to/exercise.rs
```

如果你遇到困难，每次练习的底部通常会有一个暗示。

## 测试自己

在每两个部分之后，将会有一个测试，它会立即测试你对一堆部分的知识。这些测试见于`exercises/testN.rs`。

## 完成

生锈没有做;有几个部分是非常实验性的，没有适当的文档。这些包括：

- 错误（`exercises/errors/`）
- 选项 （`exercises/option/`）
- 结果（`exercises/result/`）
- 移动语义（仍然可以改进，`exercises/move_semantics/`）

另外，我们可以在几个主题上使用练习：

- 结构
- 更好的所有权
- `impl`
- ???可能更多

如果您有兴趣改进或添加新的，请随时贡献！继续读以获取更多信息 ：）

## 特约

### 添加练习

第一步是添加练习！叫它`exercises/yourTopic/yourTopicN.rs`，请务必添加一些有用的链接，并链接到本书的各个部分`exercises/yourTopic/README.md`。

接下来，您要确保它在使用时运行`rustlings`。所有练习都存储在`info.toml`， 在下面`exercises`阵列。他们按照他们使用时的命令排序`rustlings verify`。

您想确保在文件中添加练习的位置。如果您不确定，请将其添加到底部并在拉取请求中询问。要添加练习，请按以下方式编辑文件：

```diff
  ...
+ [[exercises]]
+ path = "exercises/yourTopic/yourTopicN.rs"
+ mode = "compile"
  ...
```

该`mode`属性决定 Rustlings 是否只编译练习，或者编译和测试它。如果您在练习中有要验证的测试，请选择`test`， 除此以外`compile`。

就这样！随意提出拉动请求。

### 处理源代码

`rustlings`基本上是一个美化`rustc`包装。因此，源代码并不是那么复杂，因为大部分工作都是通过完成的`rustc`。`src/main.rs`包含一个简单的`clap`从中加载的 CLI`src/verify.rs`和`src/run.rs`。

## 积分

`rustlings`最初是由[颂歌](https://github.com/carols10cents)！
