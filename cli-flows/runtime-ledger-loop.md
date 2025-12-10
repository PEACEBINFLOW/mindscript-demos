# 3.3-runtime-ledger-loop.md  
## Demo: Runtime + Ledger Loop

Goal:
- Execute a MindScript file.
- Log each stage into MindScript Ledger.

High-level idea:

1. Modify `mindscript-runtime` to emit a JSON entry per stage into `mindscript-ledger`.
2. Use a helper script to:
   - run the program
   - write entries into `/ledger/entries/`
3. Use `mindscript-ledger` to inspect the stored entries.

This doc describes the **conceptual loop**; implementation details live in the other repos.
