# minigrep

It's a command line tool to searches for the text within the desired file and returns the entire line that contains the desired text. 📟🦀

## Screenshots 📷

![Minigrep Screenshot](assets/minigrep_printscreem.png)

## Prerequisites 📋

To build and run the project, ensure you have the following installed:

- [Rust](https://www.rust-lang.org/) (latest stable version recommended)
- Cargo (Rust's package manager, included with Rust)

## Getting started 🚀

### 1. Clone the Repository

```bash
$ git clone https://github.com/vilsonfcastilho/minigrep.git
$ cd minigrep
```

### 2. Run the project

To execute the project you need to execute the `cargo run` followed by two parameters `query` and `file_path`;<br />
Follow the example bellow:

```bash
$ cargo run -- text example.txt
```

By default the program will execute the command as case sensitive;<br />
If you want to change that you need to set a environment variable named `IGNORE_CASE` as true;<br />
Follow the example bellow:

```bash
$ IGNORE_CASE=1 cargo run -- text example.txt
```

If you're using PowerShell:<br />

```bash
PS> $Env:IGNORE_CASE=1; cargo run -- text example.txt
```

```bash
PS> Remove-Item Env:IGNORE_CASE
```

And if you want to redirect the output response to other file we need to add `>` and a second `file_path`;<br />
Follow the example bellow:

```bash
$ cargo run -- text example.txt > output.txt
```

I created an `examples` folder with a `poem.txt` file that you can use to do some tests.

## Contact 📧

For any inquiries or feedback, feel free to reach out via GitHub or email.

---

Made with ♥ by Vilson Castilho
