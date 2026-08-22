# Publication manifest contract

`.publish/manifest.json` is reserved for the latest successful exporter run.
Only the exporter may replace it, together with generated files under
`content/wiki/`. No exporter may modify content outside that managed subtree.

The final manifest must record schema and policy versions, source and target
repositories, the managed subtree, each exported file's path/byte count/SHA-256,
and the canonical manifest SHA-256. This directory is outside `content/` and is
therefore not Quartz-published content.
