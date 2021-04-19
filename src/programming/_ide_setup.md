# IDE Setup

This subchapter will cover recommendations and tips for working in your favorite IDE.

<!-- TODO: Is this too opinionated? -->

Currently the following IDEs appear to work best for Rust:

- [VSCode][vscode] with the [rust-analyzer][rust-analyzer] plugin
- IntelliJ [CLion][clion], [IDEA Ultimate][idea], [PyCharm Pro][pycharm], or [GoLand][goland] with the [Rust][intellij-rust] plugin
  - [Debugging support varies between products][intellij-dbg]

These IDEs need some tweaking to get the most out of Rust and Bevy. We will cover these in the following sub-chapters.

If you are using a different IDE, here are some general tips:

- Set `CARGO_MANIFEST_DIR` to your root directory, where the `assets` folder can be found.

[vscode]: https://code.visualstudio.com/
[rust-analyzer]: https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer
[clion]: https://www.jetbrains.com/clion/
[idea]: https://www.jetbrains.com/idea/
[pycharm]: https://www.jetbrains.com/pycharm/
[goland]: https://www.jetbrains.com/go/
[intellij-rust]: https://intellij-rust.github.io/
[intellij-dbg]: https://plugins.jetbrains.com/plugin/8182-rust/docs/rust-debugging.html