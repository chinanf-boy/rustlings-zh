# rust-lang/rustlings [![explain]][source] [![translate-svg]][translate-list]

<!-- [![size-img]][size] -->

[explain]: http://llever.com/explain.svg
[source]: https://github.com/chinanf-boy/Source-Explain
[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list
[size-img]: https://packagephobia.now.sh/badge?p=Name
[size]: https://packagephobia.now.sh/result?p=Name

「 rustlings ：记得初次骑单车时，帮你扶住的那双手吗，嗯，这就是帮你扶住 Rust 的那双 」

[中文](./readme.md) | [english](https://github.com/rust-lang/rustlings)

---

## 校对 ✅

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

# rustlings 🦀❤️

欢迎来到`rustlings`。这个项目包含一些小练习，让你能对 Rust 代码产生习惯性，能够阅读和编写它们。还包括了解和响应编译器消息！

_...寻找旧的，基于网络的 Rustlings 版本？尝试[这里](https://github.com/rust-lang/rustlings/tree/rustlings-1)_

或者，对于 Rust 萌新，还有其他些资源可供参考：

- [the book](https://doc.rust-lang.org/book/index.html)- 学习 Rust 最全面的资源，但有时候有点理论。和 Rustlings 一起，学习它！
- [Rust 示例](https://doc.rust-lang.org/rust-by-example/index.html)- 通过解决小练习，来学习 Rust！这几乎就像`rustlings`，但为在线版本。

> 译者：rustlings 更为细腻，可能是女性所编写的练习，在新手关怀度上，不是我们这些大老粗能比，即便你看完了官方的语言书，了解了主要编程思想，但实际编写时，还是会畏首畏尾的。究其原因，(居然，rustlings 让我醒悟)是对那些编写(小)细节的不熟悉，甚至会有种陌生感。这种感觉上的膈膜，是迟迟没法在语言编写进一步的阻碍。谢谢作者 🦀️。

## 入门

_注意：如果您使用的是 MacOS，请确保已通过执行`xcode-select --install`，来安装 Xcode 及其开发工具。_

_注意：如果您安装了 Xcode 10+，则还需要找到`/Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg`安装软件包文件。_

若您需要安装 Rust。你可以通过访问<https://rustup.rs>获得它。这也将安装 Cargo —— Rust 包/项目管理器。

## MacOS / Linux

简单运行：

```bash
curl -L https://git.io/rustlings | bash
# 或是想安装在不同的位置
curl -L https://git.io/rustlings | bash -s mypath/
```

这将安装 Rustlings，并让您能够使用`rustlings`命令。运行它开始！

## Windows /手动安装

基本上：克隆存储库，签出到最新标签，运行`cargo install`。

```bash
git clone https://github.com/rust-lang/rustlings
cd rustlings
git checkout tags/1.2.2 # 或其他最新版本（最新版本在 https://github.com/rust-lang/rustlings/releases/latest)
cargo install --force --path .
```

与上面相同，运行`rustlings`开始。

## 做练习

练习按主题排序，可以在`rustlings/exercises/<topic>`子目录中找到。对于每个主题，都有一个附加的 README 文件，其中包含一些资源，可帮助您开始使用该主题。我们真的建议您在开始之前，先看看它们。

任务很简单。大多数练习包含一个错误，使其无法编译，而你的斗争，就是要解决它！有些练习还有些测试会运行，但是 `rustlings`命令会处理好。要按建议的顺序运行练习，请执行：

```bash
rustlings verify
```

这将尝试按预定顺序，验证(verify)每项练习的完成情况（我们认为最适合新手的）。如果你不想每次更改文件，都要重新运行一次`verify`，可以运行：

```bash
rustlings watch
```

这将与 verify 相同，但在运行后不会退出，而是您更改`exercises/`目录文件后，立即自动重新运行。

如果您想走自己的顺序，或者只想验证一个练习，您可以运行：

```bash
rustlings run exercises/path/to/exercise.rs
```

如果你遇到困难，每次练习(文件)的底部，通常会有一个暗示。

## 测试自己

在每两个部分之后，将会有一个测试，它会立即测试你对一堆的章节知识。这些测试见于`exercises/testN.rs`。

## 完成

Rustlings 其实还没有做完；有几个部分是非常实验性的，没有适当的文档。这些包括：

- Errors（`exercises/errors/`）
- Option（`exercises/option/`）
- Result（`exercises/result/`）
- Move 语义（仍然可以改进，`exercises/move_semantics/`）

另外，我们可以在几个主题上，使用练习：

- Structs
- 更好的所有权
- `impl`
- ??? 可能更多

如果您有兴趣改进或添加新的(练习)，请随时贡献！继续读以获取更多信息 ：）

## 帮助

### 添加练习

第一步是添加练习！它命名模式`exercises/yourTopic/yourTopicN.rs`，请务必添加一些有用的链接，并在`exercises/yourTopic/README.md`链接到本书章节。

接下来，您要确保它，在运行`rustlings`，能够执行(失败)。所有练习都存储在`info.toml`中，`exercises`数组以下。`rustlings verify`时，会按照使用时的命令排序。

您想确保在文件中，添加练习的位置。如果您不确定，请将其添加到底部，并在 PR 中询问。要添加练习，请按以下方式编辑文件：

```diff
  ...
+ [[exercises]]
+ path = "exercises/yourTopic/yourTopicN.rs"
+ mode = "compile"
  ...
```

该`mode`属性决定 Rustlings 是否只编译练习，或者编译和测试它。如果您在练习中，有要验证的测试，请选择`test`， 除此以外，都是`compile`。

就这样！随意提出 PR。

### 源代码的工作

`rustlings`基本上是一个美化的`rustc`包装器。因此，源代码并不是那么复杂，因为大部分工作都是通过`rustc`完成的。`src/main.rs`包含一个简单的`clap`CLI，会从`src/verify.rs`和`src/run.rs`中加载而来。

## 荣誉

`rustlings`最初是由[Carol](https://github.com/carols10cents)编写！
