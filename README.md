
# cargo-watch

Run a Cargo command (defaults to `run`) everytime a source file changes.

This should work on any POSIX environment where [`fswatch`](https://github.com/emcrisostomo/fswatch) is available.

I quickly threw this together because [passcod/cargo-watch](https://github.com/passcod/cargo-watch) doesn't support Mac OS X, and I was tired of running `cargo build` by hand everytime I updated a source file.

The plan is not to improve this script, but to add support for FSEvents to [passcod/cargo-watch](https://github.com/passcod/cargo-watch) and then deprecate this project.

## Usage

```
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

3. Make it executable. Eg. `$ chmod +x ~/.bin/cargo-watch`

4. Then call the `watch` command as a normal `cargo` command. Eg. `$ cargo watch test`

## TODO

- <del>Reach feature-parity with https://github.com/passcod/cargo-watch.</del>
- Add support for FSEvents to [passcod/cargo-watch](https://github.com/passcod/cargo-watch) and deprecate this project.

## License

cargo-watch is released under the [MIT license](http://romac.mit-license.org).

