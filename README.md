# RustyGrep

RustyGrep is a command-line tool written in Rust that allows users to search for patterns in files. It is a modern implementation of the classic `grep` command found on Unix systems.

## Features

RustyGrep offers the following features:

- Search for patterns in one or multiple files

- Search recursively through directories and subdirectories

- Case-sensitive or case-insensitive searching

- Display line numbers for matching lines

- Display context around matching lines

- Support for regular expressions

- Fast and efficient searching, thanks to Rust's performance and memory safety guarantees

## Installation

To use RustyGrep, you must have Rust installed on your system. You can download Rust from the official website: https://www.rust-lang.org/tools/install.

Once Rust is installed, you can install RustyGrep using Cargo, Rust's package manager:

```
cargo install rusty-grep
```

## Usage

**NOTICE: RustyGrep is still under active development and will soon be available.**

The basic syntax for RustyGrep is:

```
rusty-grep [options] pattern [file ...]
```

Here are some examples:

Search for the word "hello" in a single file:

```
rusty-grep hello file.txt
```

Search for the word "world" in all `.txt` files in the current directory, displaying line numbers for matching lines:

```
rusty-grep -n world *.txt
```

Search for the word "foo" in all `.rs` files in the `src` directory and its subdirectories, displaying two lines of context around each matching line:

```
rusty-grep -C 2 foo src/**/*.rs
```

For more information about RustyGrep's options and usage, please refer to the built-in help:

```
rusty-grep --help
```

## Contributing

Contributions to RustyGrep are welcome! If you have any suggestions or questions, please open an issue or pull request on GitHub.

## License

RustyGrep is distributed under the MIT License. Please refer to the [LICENSE](https://github.com/sunray-ley/rusty-grep/blob/main/LICENSE) file for more information.
