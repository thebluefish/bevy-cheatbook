# IntelliJ IDE setup

## Installation

1. Install your favorite IDE
   - Rust works best with [CLion][clion], [IDEA Ultimate][idea], [PyCharm Pro][pycharm], or [GoLand][goland] 
   - Please note [debugging support][intellij-dbg] varies by product
2. Install the [Rust][intellij-rust] plugin

## Add a debug configuration

1. `Run` menu
2. `Edit Configurations...`
3. Add new configuration (plus symbol) -> `Cargo`
4. If it's not already set, set your `Working directory` to your project
5. Add `CARGO_MANIFEST_DIR=<your working directory>` to `Environment variables`

With Bevy 0.5, the debugger is unable to find your `assets` folder by default. If you are getting asset errors while using the debugger, ensure that `CARGO_MANIFEST_DIR` is properly setup above.

## Enable "evaluate build scripts"

With Bevy 0.5, some code completion doesn't work - most notably with `Query`. We can fix this by enabling an experimental feature:

1. `Help` menu
2. `Find Action`
3. Find `Experimental features...`
4. Enable `org.rust.cargo.evaluate.build.scripts`
   - Additionally `org.rust.resolve.new.engine` may help code completion issues with other crates


[clion]: https://www.jetbrains.com/clion/
[idea]: https://www.jetbrains.com/idea/
[pycharm]: https://www.jetbrains.com/pycharm/
[goland]: https://www.jetbrains.com/go/
[intellij-rust]: https://intellij-rust.github.io/
[intellij-dbg]: https://plugins.jetbrains.com/plugin/8182-rust/docs/rust-debugging.html