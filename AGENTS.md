# lib-result

`result` — Result type for Handl (pure handl).

## Layout

| path | role |
| --- | --- |
| `src/index.hnl` | the library |
| `src/result.test.hnl` | the .hnl test suite |
| `pkg.hnl` | package manifest — `modules: ["result"]` |
| `scripts/hnl-gate.sh`, `workflows/gate.yaml` | the gate / bupha entry |

## Contract

- Pure `.hnl` Result type (ok/err records); no Rust crate. `lib-test`
  assertion helpers return this shape.

## Verification

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.

<!-- myco:agent-awareness -->

## Agent awareness

- Session start / any work discussion: run `myco status --prompt`
  before proposing next steps — know the board first.
- User describes new work → offer to capture it (`myco todo add`,
  `issue new`, `proposal new`). Don't wait to be asked.
- Picking up a task: `myco resume <ID>` is the briefing.
- Wrapping up: `myco handoff <ID>` anything resumable; keep statuses
  honest (claimed → in-progress → blocked/done).

<!-- /myco:agent-awareness -->
