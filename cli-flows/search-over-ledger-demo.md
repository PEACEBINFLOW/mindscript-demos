# 3.4-search-over-ledger-demo.md  
## Demo: Search Over Ledger with mindscript-search

Once ledger entries exist:

1. Point `mindscript-search` config to your ledger directory.
2. Run indexing:

```bash
python 5-cli/5.1-search_cli.py reindex ledger
Then search:

bash
Copy code
python 5-cli/5.1-search_cli.py find "multi-stage essay"
Observe which ledger entries and threads are returned.
