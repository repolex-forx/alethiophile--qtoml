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
│   │   ├── 00b881f07d3957d9599797528e92fdc84cc0f465.nq.gz
│   │   ├── 1b33c9a3e2180619e48c5adabe96797e7af78590.nq.gz
│   │   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   │   ├── 71ff8049a8ab34e34ada3d6406cd918873032f8b.nq.gz
│   │   ├── a0ae43709d0f7890dba32ca2503e794af2fb31c7.nq.gz
│   │   ├── a953edcfb93cbb613076122f8d90a33f448be8d6.nq.gz
│   │   ├── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│   │   └── f249ee5590719bc00b054ac2cb93f9295d073141.nq.gz
│   ├── lsp
│   │   ├── 00b881f07d3957d9599797528e92fdc84cc0f465.nq.gz
│   │   ├── 1b33c9a3e2180619e48c5adabe96797e7af78590.nq.gz
│   │   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   │   ├── 71ff8049a8ab34e34ada3d6406cd918873032f8b.nq.gz
│   │   ├── a0ae43709d0f7890dba32ca2503e794af2fb31c7.nq.gz
│   │   ├── a953edcfb93cbb613076122f8d90a33f448be8d6.nq.gz
│   │   ├── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│   │   └── f249ee5590719bc00b054ac2cb93f9295d073141.nq.gz
│   └── repolex
│       ├── 00b881f07d3957d9599797528e92fdc84cc0f465.nq.gz
│       ├── 1b33c9a3e2180619e48c5adabe96797e7af78590.nq.gz
│       ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│       ├── 71ff8049a8ab34e34ada3d6406cd918873032f8b.nq.gz
│       ├── a0ae43709d0f7890dba32ca2503e794af2fb31c7.nq.gz
│       ├── a953edcfb93cbb613076122f8d90a33f448be8d6.nq.gz
│       ├── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│       └── f249ee5590719bc00b054ac2cb93f9295d073141.nq.gz
├── blob
│   ├── 0681fa2d2ca51fa85c155774b9d4ecac17525ea3.nq.gz
│   ├── 09adb940b24322d84fe80bbdcc8ef52b92536746.nq.gz
│   ├── 0d400b13e6f8ba741af19a3aeb7f527c20231a4f.nq.gz
│   ├── 10662a2deaff6696e03d92e36f6372aba8ac6199.nq.gz
│   ├── 15a41a746cb1178b0a19c5959b4845d93aae720a.nq.gz
│   ├── 1c06aef57aea1cb1caf412ff9c9200f1cb09af1d.nq.gz
│   ├── 1c811a8d38d0c34e2ea16deb36e6a8da494de3e5.nq.gz
│   ├── 1df44754a802ac676b89029ed7e0999bd0693e64.nq.gz
│   ├── 24992c1d0c64e43f3f99e2145603b85030170b70.nq.gz
│   ├── 36283fc13b66abff2f4e342e2e6d8ad71e3f9186.nq.gz
│   ├── 38326c840d44247de3fad5919f6ead1744668afe.nq.gz
│   ├── 393571704701870b7550232c29b9eeebe317f953.nq.gz
│   ├── 472a1d42314e1f36db5ade0212cd7af42cc702a2.nq.gz
│   ├── 5157eef71338379d5b1888970bb98d097ec7995f.nq.gz
│   ├── 56fbde34ab30aba2f1051c2ebc01f867bb6870d1.nq.gz
│   ├── 59b6be503dcfe2e95cda5c434164b47fe4adb2a4.nq.gz
│   ├── 6390b2a75e2fba928f8e5c4a243d6e4b1f6f2b64.nq.gz
│   ├── 66eef123d290198504c9744934ed9aa04fd9a715.nq.gz
│   ├── 69937956a8b3c7d9ce47a20d04274202c01fdea7.nq.gz
│   ├── 716cc0773315b3807e35dab3a8fc7fa94c80c764.nq.gz
│   ├── 74ea4a498db30cf40efe3f34c747f2d584252b91.nq.gz
│   ├── 8534bebbe86b24d4923fe1eefe59956c66c93f6d.nq.gz
│   ├── 890be30b7dac0b6ff2a7462087c2cc8bf70801aa.nq.gz
│   ├── 91f72fcdb9586de9c802aa2eb2f0426744f0f2dc.nq.gz
│   ├── 924486f8a1b69ae99a103570b799718f79cc535e.nq.gz
│   ├── 92a5f7f7cd3ddd1b786b1998940fa79d8f6df0db.nq.gz
│   ├── 932b16858b28212b44d1ac4b3537ad7779287ed3.nq.gz
│   ├── 936940730c95599b953dec24ea5d678585f2cfa4.nq.gz
│   ├── 9f0231111dc3cc14a7e79d3c0ecd4496324fc5d3.nq.gz
│   ├── a205cd3c8f4d1f09d8eac3a0fc2c755761d92be8.nq.gz
│   ├── a7f5ad372e989701e50f5c46661ba4b1c25f92e8.nq.gz
│   ├── ae83c5147cad2bb15794d23879b120f9acffae7a.nq.gz
│   ├── c500c7687290a2d88a125da2b434b2ce7662619a.nq.gz
│   ├── c535d0eeaa0f21d74b36e2ecce4bdad2aa271ac1.nq.gz
│   ├── c8cb9d68a5a9d635966eff37e4acfe7b2f16ac81.nq.gz
│   ├── c918ac71bf7ae21eeeec6e467b61bce51bf43918.nq.gz
│   ├── cc2df672a3b37cfd0bd43a82cfefe3401bf59718.nq.gz
│   ├── ccf25ef51e95761fe1cce59af481703356468c37.nq.gz
│   ├── d36d6da9da01e068d5a5b18db726b27a3fe4fc96.nq.gz
│   ├── d63f269bd9f3a181e8e941ba4960c12edeb494a6.nq.gz
│   ├── deb756af737db33d2d7ae48022a4d657c72c8905.nq.gz
│   ├── e4c23282d9f5d95dbbc6362ca027dd35b9fe77b8.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── eac58f948c05ce3efa7cf13eed67b9e44fd1cfe4.nq.gz
│   ├── f2136d548847e34e0206526fbe8dce25618e7547.nq.gz
│   ├── f7af855bf529b0eecd576e7ac3e2a85db808ec06.nq.gz
│   ├── f901f0d27c58f7fcc228f34dc54278caeddf4910.nq.gz
│   ├── fb63eb7dda8dadd6ceaf303ece558c26bdad9405.nq.gz
│   ├── fbf7bb32bc2e0938c45f2be93214513fc3e28c48.nq.gz
│   └── fbfa7301d853c3fe8d1c7dcc2495fbbdf8984c76.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 00b881f07d3957d9599797528e92fdc84cc0f465.nq.gz
│   ├── 1b33c9a3e2180619e48c5adabe96797e7af78590.nq.gz
│   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   ├── 71ff8049a8ab34e34ada3d6406cd918873032f8b.nq.gz
│   ├── a0ae43709d0f7890dba32ca2503e794af2fb31c7.nq.gz
│   ├── a953edcfb93cbb613076122f8d90a33f448be8d6.nq.gz
│   ├── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│   └── f249ee5590719bc00b054ac2cb93f9295d073141.nq.gz
├── filetree
│   ├── 00b881f07d3957d9599797528e92fdc84cc0f465.nq.gz
│   ├── 1b33c9a3e2180619e48c5adabe96797e7af78590.nq.gz
│   ├── 328d1ff3c5c231c29a9d997f5869ee2272a561db.nq.gz
│   ├── 71ff8049a8ab34e34ada3d6406cd918873032f8b.nq.gz
│   ├── a0ae43709d0f7890dba32ca2503e794af2fb31c7.nq.gz
│   ├── a953edcfb93cbb613076122f8d90a33f448be8d6.nq.gz
│   ├── cb997e7d364b008fd12978ee4b30da1dd7a2c9be.nq.gz
│   ├── ed150abae170d7faa5bbf321d8e0b23129fcfe19.nq.gz
│   └── f249ee5590719bc00b054ac2cb93f9295d073141.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 96 files
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
