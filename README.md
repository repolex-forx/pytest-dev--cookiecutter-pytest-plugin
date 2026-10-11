# Repolex Knowledge Graph of pytest-dev/cookiecutter-pytest-plugin

RDF knowledge graph data for [pytest-dev/cookiecutter-pytest-plugin](https://github.com/pytest-dev/cookiecutter-pytest-plugin), parsed by [repolex](https://repolex.ai).

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
rlex download pytest-dev/cookiecutter-pytest-plugin
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8f38e95b344f07071c1adada1fe209137c7effab
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 8f38e95b344f07071c1adada1fe209137c7effab
│           └── chunk-001.nq.gz
├── blob
│   ├── 15e44f5812fbd07edf8f8071823054bf16f9e0ef.nq.gz
│   ├── 16003680f859f84059a551bec73c171f0337f16e.nq.gz
│   ├── 1903e064f801693bae322800c834db6e7cf789ee.nq.gz
│   ├── 197fd9654cfbda0a6e889c2c3303e65534228428.nq.gz
│   ├── 19d93be3fa9b99a12741b5a7d2105bebcdbc5a4b.nq.gz
│   ├── 283d67eb04566b02bc383ce51e30e1998994ec12.nq.gz
│   ├── 2a7a0711bf15eadffc06a9274b78264c14326109.nq.gz
│   ├── 3536192220b9dcd3757e59e8481b6b63428d6f7f.nq.gz
│   ├── 48bce20822b3ead89a8acbd4641b8c5367b77d1b.nq.gz
│   ├── 4ad5cb22235f2c7e5638b8b037bf8970207760d1.nq.gz
│   ├── 4cb65f7ef60c6d4e40eab1c6fb42855efc549bef.nq.gz
│   ├── 4ea17e5420ce808affef453006aba809e527b905.nq.gz
│   ├── 55fb6a13bd47d82d2d0ee41e050d59a9c5dee2d2.nq.gz
│   ├── 59024da24cb83c6c2833d801c8e8556a880b02b9.nq.gz
│   ├── 61cbb8e8fbb205e2aeee20f6d594f4f52e35ad08.nq.gz
│   ├── 6b5d37714ec8c5ef4a3e794ebee2b4b376aa98ae.nq.gz
│   ├── 6c5886e04363a482ba04555c612e8520b3af7d33.nq.gz
│   ├── 6ff01b23d41c23558d00612cc0ad8c1aac4039e0.nq.gz
│   ├── 7571586bae454672bc10f45c92c89a1ea4426dc5.nq.gz
│   ├── 7900805540af568571aa93594c9e404fc03906fd.nq.gz
│   ├── 79034ac0efea26e7080bd0472f478cff282a62b5.nq.gz
│   ├── 7b968accbe4fe2552061e13b77f83e336558d7c1.nq.gz
│   ├── 88f74c2cfd5c4bac59341599ab64316124c50307.nq.gz
│   ├── 896a94fe25e154ef483bf04633c45dabe99e1b56.nq.gz
│   ├── 98cf330ae58b448ee14ca6b56c47caee8ac05338.nq.gz
│   ├── 9a09d45447728da4a5970f43dc6e3f08b8188b40.nq.gz
│   ├── 9b1fd6b0c103791150fc708cfcfaae27436253d4.nq.gz
│   ├── 9cb536d75900d3b18f9f7b5b8a8fe9a99c8439a2.nq.gz
│   ├── 9dea6b2e4d7fc962122415cd4f0d5a56773b99a7.nq.gz
│   ├── b3483857f05bef2a9b09028133e1fdbce9ae8985.nq.gz
│   ├── b4888607281e88d4d9fb8363f6e47e8c3e68c3f4.nq.gz
│   ├── bc711e55fefdd729816958fa0ce1563b55217c29.nq.gz
│   ├── c63d87600e0576065876b8ea24297f9115b10c81.nq.gz
│   ├── ca77b5f8eb72d43cf365191cd6b092a425571c83.nq.gz
│   ├── cc387546bd085936b05b97705b3320954f014df6.nq.gz
│   ├── dd63b197e61ae4848333bf90db45ec18b8118999.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e93cf0c59fa1dd05aa53327a0e3f586975559f94.nq.gz
│   ├── f14f32010f7265ced6702dd045c8691ccf9b121b.nq.gz
│   └── fb37258c2a01846f2a7812e7bdb57b1fb0c73dce.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 8f38e95b344f07071c1adada1fe209137c7effab.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
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

[pytest-dev/cookiecutter-pytest-plugin](https://github.com/pytest-dev/cookiecutter-pytest-plugin)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
