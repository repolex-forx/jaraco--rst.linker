# Repolex Knowledge Graph of jaraco/rst.linker

RDF knowledge graph data for [jaraco/rst.linker](https://github.com/jaraco/rst.linker), parsed by [repolex](https://repolex.ai).

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
rlex download jaraco/rst.linker
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 6faaaa3faed8a38bbcb3cb9ba5cfd2b3814c3a71
│   │   │   └── chunk-001.nq.gz
│   │   └── c41cef52d5ac348a8108a33ad2abc8c890ff3b71
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 6faaaa3faed8a38bbcb3cb9ba5cfd2b3814c3a71.nq.gz
│   └── repolex
│       ├── 6faaaa3faed8a38bbcb3cb9ba5cfd2b3814c3a71
│       │   └── chunk-001.nq.gz
│       └── c41cef52d5ac348a8108a33ad2abc8c890ff3b71
│           └── chunk-001.nq.gz
├── blob
│   ├── 0d76d0a298ad9ce6d20e3844d1e41b708d2f519a.nq.gz
│   ├── 10d412f406891b9683f832fcbc134c9bdf4f916e.nq.gz
│   ├── 1bb5a44356f00884a71ceeefd24ded6caaba2418.nq.gz
│   ├── 1be442dde94dfe54b7bf5f1e7b6ee3c8533add2c.nq.gz
│   ├── 1f2aa7533b0423a8eb943f6f4ec02498e39581a0.nq.gz
│   ├── 2344853a22cd6597920a8a2bfc9dc34f7d84e5fc.nq.gz
│   ├── 240329c3604d8ead4c10aa8c88352caa8e4ce7b2.nq.gz
│   ├── 2e3f4dd791a6372b427d618eb0baa8c4dc58e5f0.nq.gz
│   ├── 304196f81e11a168c9894f966e4a617ebf4ed53c.nq.gz
│   ├── 32150488de655c2c2ef3b26c0a8519e7365584b3.nq.gz
│   ├── 35b98b1df96093e99fea65bec2187baff3c12514.nq.gz
│   ├── 39c013aac9a0da79c256cd6633d4eeaf1629389a.nq.gz
│   ├── 3d091d14655daf79ab375de30d8778b6ee840ba8.nq.gz
│   ├── 4c39a5b139c5c24eed2c8fe1f67116ef681ad39b.nq.gz
│   ├── 54c9000ec94341dd65c2053251b85b124017b9b5.nq.gz
│   ├── 54cc8303b22089e12053e552d4e6cb852a865b8a.nq.gz
│   ├── 577e87a793a20e413f7321f4f17ec1eba2ea1962.nq.gz
│   ├── 5991e93963c284834736a51353462e544ee53adc.nq.gz
│   ├── 5a4a7e9166ec3143f71b5e3875860802048554f3.nq.gz
│   ├── 5bdc232005af9be104a00437ae9bc64417a4c1cc.nq.gz
│   ├── 6fa480e44f38768722368d7a986607adacf41d99.nq.gz
│   ├── 700235be57c1b2872455c0be5333f59cf568e252.nq.gz
│   ├── 70612985a7a6f8ae0e29777e7ed3df05e5a717dc.nq.gz
│   ├── 724370638fc188317bbc7dc868f1a571995fd796.nq.gz
│   ├── 85dfea9d42d16274b4e8a4892bf6986d131f4241.nq.gz
│   ├── 870b551e72a61d60a5ac6efdbd3cdc6dd4a04058.nq.gz
│   ├── 89ff33961ba3d6f9cda89322a1fdbf1ac2e35513.nq.gz
│   ├── 9a0f3bce1395ae3819030b822e5d9076c85068ea.nq.gz
│   ├── 9c8bd953fc7a68919d3411ea4b3f4a8b112bb55d.nq.gz
│   ├── a993c0d67feea414fba328ca28b85353f98fb142.nq.gz
│   ├── ac0ff69e22507b430cfb9a91d98e2451a3de52d9.nq.gz
│   ├── b6f972769e61a5e65f9f45015b363cc362487e55.nq.gz
│   ├── b9faca4bfa7b5ce62335fed7f2d35323296f9a36.nq.gz
│   ├── e05a3d4a2ab888e32952006d8cd380864368db5f.nq.gz
│   └── efcb8cbc2043faa7caf4f92fc7488bd6914c934c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 6faaaa3faed8a38bbcb3cb9ba5cfd2b3814c3a71.nq.gz
├── filetree
│   ├── 6faaaa3faed8a38bbcb3cb9ba5cfd2b3814c3a71.nq.gz
│   └── c41cef52d5ac348a8108a33ad2abc8c890ff3b71.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

17 directories, 48 files
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

[jaraco/rst.linker](https://github.com/jaraco/rst.linker)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
