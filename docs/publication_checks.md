# Publication checks

Checked on 9 October 2026 for this upload.

- Source: `Nobel-Corpus-Package.zip` supplied by the user.
- All 20 supplied files match the ZIP byte for byte. Its README is preserved as `ORIGINAL_README.md` at the repository root so its relative links still work.
- The new `README.md` explains the collection in simple Canadian English for a grown-up to read with a young child.
- Python 3.12.4 on Windows: `python -m unittest discover -s tests -v` passed all 18 existing tests, with zero failures or errors. This includes a byte-for-byte corpus rebuild.
- `python corpus.py audit data/processed/corpus.jsonl` completed successfully: 47 records, 46 distinct normalised original texts, eight editorial edits, one reported stream, and zero approved translation pairs.
- All Japanese-source fields remain empty and all current records remain ineligible for training.
- The new README's local links were checked against files in this repository.

These checks confirm file preservation and the tested program behaviours. They do not fact-check the submitted Nobel Prize or scientific statements, review the translations against Japanese audio, verify the supplied research/release snapshots, or train or evaluate a model. `docs/verification.json` is preserved from the attachment and is separate from this run's results.

Source ZIP SHA-256: `359638178a2bff54a4c434e8ca5eec4330161c9019d0702b0bc05bdd8cbb811b`
