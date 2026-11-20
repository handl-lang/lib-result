# lib-result

`result` — Result type for Handl (pure handl).

## Layout

```text
src/index.hnl         the library
src/result.test.hnl   the .hnl test suite
pkg.hnl               package manifest — modules, deps, description, license
ci.sh                 bupha entry → scripts/hnl-gate.sh
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.
