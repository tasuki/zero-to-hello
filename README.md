# Zero to Hello (World)

| Language | Version | Confusion | Setup MB | Hot run  |
| -------- | ------- | --------: | -------: | -------: |
| Python   | 3.13.5  | 🙂        | 108 MB   | 0.0      |
| Scala    | 3.7.1   | 😕        | 260 MB   | 0.6      |
| Haskell  | 3.5.1   | 😐        | 200 MB   | 0.4      |
| Idris2   | 0.7.0   | 😐        | 125 MB   | 0.1      |
| Gleam    | 1.11.1  | 😐        | 200 MB   | 0.2      |
| F#       | 8       | 😐        | 577 MB   | 1.6      |

- **Python**: No dependencies! Run: `python hello/hello.py`
- **Scala**: Excl system `default-jdk`. Run: `scala-cli hello/hello.scala`
- **Haskell**: Run: `stack hello/hello.hs`
- **Idris2**: Run: `idris2 hello/hello.idr && build/exec/hello`
- **Gleam**: But I had to download lots more, also needed Erlang. Run: `cd hello/gleam/ && gleam run`
- **F#**: DotNet is big and F# is slow. Run: `cd hello/fsharp/ && dotnet run`
