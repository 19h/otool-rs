<h1 align="center">otool</h1>

<h5 align="center">A pure Rust-implementation of 'otool' for the Mach-O File Format.</h5>

<div align="center">
  <a href="https://crates.io/crates/otool">
    crates.io
  </a>
  —
  <a href="https://github.com/19h/otool">
    Github
  </a>
  -
  <a href="https://github.com/19h/otool-rs/releases">
    Releases (prebuilt binaries)
  </a>
</div>

<br />

```shell script
$ cargo install otool
$ otool -a binary.o
```

#### Trivia

<h5>otool is based on rust-macho, more specifically on its <a href="https://github.com/flier/rust-macho/blob/94bafced83cad602f37e31cc387c021bd2db47c2/examples/otool.rs">otool example</a>. This is a distribution (with minor changes).</h5>

#### Usage

```yaml
otool 0.1.0
object file displaying tool

USAGE:
    otool [FLAGS] [OPTIONS] [--] [files]...

FLAGS:
        --help       Prints help information
    -a               Print the archive headers
        --bind       Print the mach-o binding info
    -d               Print the data section
        --export     Print the mach-o exported symbols
    -f               Print the fat headers
    -X               Print no leading addresses or headers
        --lazy       Print the mach-o lazy binding info
    -S               Print the table of contents of a library
    -l               Print the load commands
    -h               Print the mach header
        --rebase     Print the mach-o rebasing info
    -L               Print shared libraries used
    -D               Print shared library id name
    -n               Print the symbol table
    -t               Print the text section
    -v               Print verbosely (symbolically) when possible
        --version    Print the version of program
        --weak       Print the mach-o weak binding info

OPTIONS:
        --arch <cpu-type>             Specifies the architecture
    -s <segname[:sectname]>...        Print contents of section

ARGS:
    <files>...    The object files
```

#### Notes

`cargo` requires a rust installation.
