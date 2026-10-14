# Public metadata redaction

Local home/workspace prefixes, recorded host names, working directories and process identities were removed or replaced with stable public placeholders. Bytecode caches were omitted because they can embed local source paths. Experimental run IDs, block IDs, controller/source revisions, numeric observations, tolerances, expected verdicts and negative findings are retained.

SANITIZATION_MANIFEST.csv distinguishes original-before-redaction and distributed hashes. The private reverse identity mapping is not distributed. The ND2410 transport cache and two pilot native executable snapshots remain omitted as separately documented. This derivative is not byte-identical to the original reviewer archive. Original frozen local files are unchanged.

RELEASE_STATIC_MANIFEST.csv and RELEASE_LOCATOR_INDEX.csv describe the distributed bytes. Historical original-byte ledgers are retained as evidence but cannot validate metadata-redacted files. Accordingly the public replay entry checks distributed integrity and does not run the old original-byte-only integrity stage. The historical driver is preserved under historical/. No numeric checker or reference predicate was replaced, no experimental truth or verdict was edited, and no controller/test/replay was executed to prepare this edition.

The publisher's static numeric-preservation inspection is not an independent semantic audit or non-author reproduction. Public access, DOI, author AI disclosure, licensing scope and independent replication remain separately reported.
