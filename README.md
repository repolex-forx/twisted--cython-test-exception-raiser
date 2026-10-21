# Repolex Knowledge Graph of twisted/cython-test-exception-raiser

RDF knowledge graph data for [twisted/cython-test-exception-raiser](https://github.com/twisted/cython-test-exception-raiser), parsed by [repolex](https://repolex.ai).

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
rlex download twisted/cython-test-exception-raiser
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c0c28994d522a8eb650189fc6f9ce1d91a0bc268
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── c0c28994d522a8eb650189fc6f9ce1d91a0bc268
│           └── chunk-001.nq.gz
├── blob
│   ├── 0604c6c7fb5133f7ff134d239532636658fe9f01.nq.gz
│   ├── 2bdddf994b00769e093ce1ff173c71cc54c03db0.nq.gz
│   ├── 3bf688e76fc22680107055ccd0631a9b8c330ba9.nq.gz
│   ├── 56c9bf6143f8d5b7ecaaf40e8123487d01f3d36d.nq.gz
│   ├── 580084011b804f591883220c82da545ef4d0791d.nq.gz
│   ├── 5c44c970c821c153f84b60ac146673b5e6778a44.nq.gz
│   ├── 7f36245e6642b7535b65837b41520c3e32089755.nq.gz
│   ├── 86dc17d9dd587983ea8cfa55f0bb03159da18375.nq.gz
│   ├── b35069f7efff04f103a10b2874b0d29bf9c36490.nq.gz
│   ├── cc0af6aa7126a5a3e53cc9550ea965e28cafa11c.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f740060fa7649975a960471684a07192c46f78a9.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── c0c28994d522a8eb650189fc6f9ce1d91a0bc268.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 19 files
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

[twisted/cython-test-exception-raiser](https://github.com/twisted/cython-test-exception-raiser)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
