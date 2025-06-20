# Zero to Hello (World)

Install `mise`, perhaps version `2025.4.1`.

What a hello world takes, starting from Debian and using mise:

| Language | Confusion | Setup MB | Setup time | First run | Hot run |
| -------- | --------: | -------: | ---------: | --------: | ------: |
| Python   |        😊 |   108 MB |       15 s |       0 s |   0.0 s |
| Scala    |        😕 |   260 MB |       60 s |      60 s |   0.6 s |
| Haskell  |        🙂 |  2800 MB |        5 s |     220 s |   0.4 s |
| Idris2   |        😏 |   125 MB |      666 s |       1 s |   0.1 s |
| Gleam    |        😅 |   190 MB |      120 s |       1 s |   0.2 s |
| F#       |        😐 |   577 MB |       35 s |       3 s |   1.3 s |
| Roc      |        😕 |   105 MB |       20 s |       1 s |   0.2 s |

- **Python**: No dependencies! Run: `python hello/hello.py`
- **Scala**: Excl system `default-jdk`. Confusion: scala-cli, coursier, bloop. Run: `scala-cli hello/hello.scala`
- **Haskell**: Run: `stack hello/hello.hs`
- **Idris2**: Cons: builds everything from scratch. Pros: builds everything from scratch. Run: `idris2 hello/hello.idr && build/exec/hello`
- **Gleam**: Confusion: needs Erlang. Run: `cd hello/gleam/ && gleam run`
- **F#**: DotNet is big and F# is slow. Run: `cd hello/fsharp/ && dotnet run`
- **Roc**: `mise plugins add roc https://github.com/dkuku/asdf-roc.git`. Run: `roc/hello.roc`
