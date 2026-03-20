# Repolex Knowledge Graph of alethiophile/qtoml

RDF knowledge graph data for [alethiophile/qtoml](https://github.com/alethiophile/qtoml), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download alethiophile/qtoml
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   │   └── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│   ├── lsp
│   │   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   │   └── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│   └── repolex
│       ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│       └── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
├── blob
│   ├── 0681fa2d2ca51fa85c155774b9d4ecac17525ea3.nq.gz
│   ├── 10662a2deaff6696e03d92e36f6372aba8ac6199.nq.gz
│   ├── 15a41a746cb1178b0a19c5959b4845d93aae720a.nq.gz
│   ├── 1c811a8d38d0c34e2ea16deb36e6a8da494de3e5.nq.gz
│   ├── 56fbde34ab30aba2f1051c2ebc01f867bb6870d1.nq.gz
│   ├── 6390b2a75e2fba928f8e5c4a243d6e4b1f6f2b64.nq.gz
│   ├── 69937956a8b3c7d9ce47a20d04274202c01fdea7.nq.gz
│   ├── 716cc0773315b3807e35dab3a8fc7fa94c80c764.nq.gz
│   ├── 74ea4a498db30cf40efe3f34c747f2d584252b91.nq.gz
│   ├── 8534bebbe86b24d4923fe1eefe59956c66c93f6d.nq.gz
│   ├── 91f72fcdb9586de9c802aa2eb2f0426744f0f2dc.nq.gz
│   ├── 924486f8a1b69ae99a103570b799718f79cc535e.nq.gz
│   ├── 932b16858b28212b44d1ac4b3537ad7779287ed3.nq.gz
│   ├── 936940730c95599b953dec24ea5d678585f2cfa4.nq.gz
│   ├── 9f0231111dc3cc14a7e79d3c0ecd4496324fc5d3.nq.gz
│   ├── a205cd3c8f4d1f09d8eac3a0fc2c755761d92be8.nq.gz
│   ├── ae83c5147cad2bb15794d23879b120f9acffae7a.nq.gz
│   ├── c535d0eeaa0f21d74b36e2ecce4bdad2aa271ac1.nq.gz
│   ├── c8cb9d68a5a9d635966eff37e4acfe7b2f16ac81.nq.gz
│   ├── d36d6da9da01e068d5a5b18db726b27a3fe4fc96.nq.gz
│   ├── deb756af737db33d2d7ae48022a4d657c72c8905.nq.gz
│   ├── e4c23282d9f5d95dbbc6362ca027dd35b9fe77b8.nq.gz
│   ├── f2136d548847e34e0206526fbe8dce25618e7547.nq.gz
│   ├── f901f0d27c58f7fcc228f34dc54278caeddf4910.nq.gz
│   └── fbf7bb32bc2e0938c45f2be93214513fc3e28c48.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   └── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
├── filetree
│   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   ├── a953edcfb93cbb613076122f8d90a33f448be8d6.nq.gz
│   └── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 41 files
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

## Source repository

[alethiophile/qtoml](https://github.com/alethiophile/qtoml)

---
*Parsed on 2026-03-20 by [repolex](https://repolex.ai)*
