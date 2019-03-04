# exit-status-ext

Rust trait for extending `std::process::ExitStatus`.

```rust
use exit_status_ext::ExitStatusExt;

Command::new("program-name")
    .status()
    .and_then(ExitStatusExt::as_result)?;
```
