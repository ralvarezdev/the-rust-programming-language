# the-rust-programming-language

Notes and exercises while following [*The Rust Programming Language*](https://doc.rust-lang.org/book/). Each top-level folder is named after a chapter and holds the Cargo project written for it. Only chapters 1, 2 and 12 are present so far.

## Contents

- **`01-getting-started/hello_world`** — hello-world program.
- **`02-programming-a-guessing-game/guessing_game`** — number guessing game; reads guesses from stdin and picks a secret number from 1 to 100 with the `rand` crate (0.9.3).
- **`12-io-project/minigrep`** — command-line search tool with a library (`search`, `search_case_insensitive`) and a binary.

All packages use Rust edition 2024, so you need a recent toolchain (install with [rustup](https://rustup.rs/)).

## Running

```bash
cd 01-getting-started/hello_world && cargo run
cd 02-programming-a-guessing-game/guessing_game && cargo run
cd 12-io-project/minigrep && cargo run -- <query> poem.txt
```

`minigrep` prints the lines of the given file that match (a sample `poem.txt` is included). Set `IGNORE_CASE` (any value) for case-insensitive search, e.g. `IGNORE_CASE=1 cargo run -- to poem.txt`.

## License

GNU General Public License v3.0. See [LICENSE](LICENSE).
