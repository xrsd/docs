---
sourcePath: en/ydb/ydb-docs-core/en/core/reference/ydb-sdk/example/_includes/steps/03_write_queries.md
---
## Adding data {#write-queries}

Adding data to the created tables using an [`UPSERT`](../../../../../yql/reference/syntax/upsert_into.md) statement of [YQL](../../../../../yql/reference/index.md). A data update request is sent within a single request to the server with transaction auto-commit mode enabled.

