# Repolex Knowledge Graph of block/apple-codesign-action-example

RDF knowledge graph data for [block/apple-codesign-action-example](https://github.com/block/apple-codesign-action-example), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download block/apple-codesign-action-example
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8349e37cd6735d00c39a6818f0fea9c8c007754f
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 8349e37cd6735d00c39a6818f0fea9c8c007754f.nq.gz
│   └── repolex
│       └── 8349e37cd6735d00c39a6818f0fea9c8c007754f
│           └── chunk-001.nq.gz
├── blob
│   ├── 0819e1664cf11514be6bdcaaba174d5083e721f1.nq.gz
│   ├── 097e8bf10c02ce7b030393e999d1baf292d2f972.nq.gz
│   ├── 1c627d309725cdc4cec7755566b5121e22159fbc.nq.gz
│   ├── 2349addd6d5c2fe881f3a5d5d577c97a0698c68d.nq.gz
│   ├── 38c1d7aa08c172c094533aa6b06ff2d1ddb0a028.nq.gz
│   ├── 39778ae97e0dd1e93c72ba83dd5b126e3aa5d9b7.nq.gz
│   ├── 4fa50aef5c623db117eafef96c288f51cf7e122e.nq.gz
│   ├── 534f088ce881059fe23552624e8518f1e633ffd4.nq.gz
│   ├── 6bccf43368fd7c96d9c659562a5142b8b8cb98a1.nq.gz
│   ├── 71cc9cc9ea766dbfcda7e031b3136f95d35c8fbf.nq.gz
│   ├── 795580e6c475a3d7d48cd0d704a7dd76dd150345.nq.gz
│   ├── 862ee3c28647e7a58801a75236855c269c1448ae.nq.gz
│   ├── 89f8686e94e90a526c4f5c288b43d07db16a70a8.nq.gz
│   ├── 90dd9ced1dffd7b626efa9a14bd83386a222f74c.nq.gz
│   ├── 919434a6254f0e9651f402737811be6634a03e9c.nq.gz
│   ├── 9582fc588754f78d9875691a3bd5e674295436b3.nq.gz
│   ├── 9a048e8ffaebeb1b07902f081e2b635cbfc13cea.nq.gz
│   ├── 9b43153981089cca86fc92fed446433d07c4f323.nq.gz
│   ├── 9b6d43054a413c1f658e39a86999c2faf8f2d287.nq.gz
│   ├── 9d534f4f4bfe3379bc4113606e1db74c8e32896c.nq.gz
│   ├── aa1070e7f8e703220bf4157a922d30441a3cfe1a.nq.gz
│   ├── bf68079e7da2992c60140c794d5cb04a88c8c078.nq.gz
│   ├── c13ab98aaf76772c8397837ede6472e79267c6cd.nq.gz
│   ├── cedfbd120b75f047fcd5cf9dfc0d124be3267760.nq.gz
│   ├── d6914d2b75a611b0be5fda1b44b3698fa92dca89.nq.gz
│   ├── dbaa5bbcca5cc738680b33f0231777d281e01646.nq.gz
│   └── dff25db22d156d008d129835b953db35addc0439.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 8349e37cd6735d00c39a6818f0fea9c8c007754f.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 36 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[block/apple-codesign-action-example](https://github.com/block/apple-codesign-action-example)

---
*Parsed on 2026-10-02 by [repolex](https://repolex.ai)*
