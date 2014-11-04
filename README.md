
# cargo-watch

```
Run a Cargo command (defaults to `run`) everytime a source file changes.

Usage:
    cargo watch [options] [<command>]

Options:
    -h        Display this message.
    -d DIR    Watch files in the given directory [default: src/].

Requirements:
    This command requires fswatch to be present on your system.
    Use your favorite package manager to install it (MacPorts, Homebrew, apt, etc).
```

## Installation

1. Install `fswatch` using your favorite package manager (MacPorts, Homebrew, apt, etc).

2. Copy `cargo-watch` somewhere in your `$PATH`. Eg. `$ cp cargo-watch ~/.bin/cargo-watch`

3. Then call the `watch` command as a normal `cargo` command. Eg. `$ cargo watch test`

## License

cargo-watch is released under the [MIT license](http://romac.mit-license.org).

