# Repolex Knowledge Graph of NousResearch/Hermes-Function-Calling

RDF knowledge graph data for [NousResearch/Hermes-Function-Calling](https://github.com/NousResearch/Hermes-Function-Calling), parsed by [repolex](https://repolex.ai).

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
rlex download NousResearch/Hermes-Function-Calling
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ea3c4723e4cefdac760d483ccac6c8a428c95ab8
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── ea3c4723e4cefdac760d483ccac6c8a428c95ab8.nq.gz
│   └── repolex
│       └── ea3c4723e4cefdac760d483ccac6c8a428c95ab8
│           └── chunk-001.nq.gz
├── blob
│   ├── 0783c70bdf10a29c3d971db4fdac806983eb2a22.nq.gz
│   ├── 0a6dc9bf22a667fda4daf9416621f00fdeebd5b1.nq.gz
│   ├── 0cc6d66ecf742679d3d254a06356ac23bf310388.nq.gz
│   ├── 10294c010ee4da1f50128dd97d4fcec04216e507.nq.gz
│   ├── 13d69902fbeaae23a982dbdec8f526a2e6ce6fb6.nq.gz
│   ├── 1458c31571187c63e48002be5c6052042ccb4db4.nq.gz
│   ├── 16fd9d20c39d9790acf132fbd5ab9767557fa706.nq.gz
│   ├── 199d03f689e3686e96ba07ba89c3796dad756cab.nq.gz
│   ├── 2a65925d58f91be0c0681b9a36bbed114e7f7ee9.nq.gz
│   ├── 2c10e89eba59a4e9573fdcbba855fd33ca4afa2e.nq.gz
│   ├── 357c7eaa53611eb06fe6cb0a925f0b82cb217309.nq.gz
│   ├── 374579be59eb03e3bd89c2278c1d1a11f9405325.nq.gz
│   ├── 406a736ba98f506143ba46d4dfa2eb9213922fc3.nq.gz
│   ├── 42aa8a1ae92369e6b504f93402f43a97abae087a.nq.gz
│   ├── 4a569e52936159334de091cf994831ec2b45e068.nq.gz
│   ├── 520df8c4107495a6403d1c74d4804761765803ae.nq.gz
│   ├── 579e5c9bd4d32560ed84589a975a36a62d15115d.nq.gz
│   ├── 5dd32abdc7b8c956705494078b03e540b6f3f21b.nq.gz
│   ├── 6bc58a11a0f8e5cd8c931364c239a7bdb2fcdbaf.nq.gz
│   ├── 7204db73d3743ee76e34e424487f636c2bbf156a.nq.gz
│   ├── 74acdddfa081cb262e2f0547708a2a1c51d05682.nq.gz
│   ├── 7568abd1e410b45c1fd1fecfa17114872c255ac8.nq.gz
│   ├── 794627ad5b01e486baccfcea4c9ad71866550dad.nq.gz
│   ├── 7d0d54495e2c822f18239eb8f2becc122fefdbb5.nq.gz
│   ├── 80d5a1e94272de458f2a1087ce275f4c8a44c716.nq.gz
│   ├── 853743bc9d54eac008c66ef9d962380c24fd8fb3.nq.gz
│   ├── a06423eebff9a1dcd1b66e30df1aa26c2909b28d.nq.gz
│   ├── a73efc2e8c3f0899417c023a4e291bdde3735bd2.nq.gz
│   ├── abd915402f2ab5fdfa049a28da8259308a8c4191.nq.gz
│   ├── c70eabe61fd660b918cca12a6bfaf57d5a6b7f07.nq.gz
│   ├── c9f137984f9b43b644dc7ff6281e1b43c860ec74.nq.gz
│   ├── ccde790d0d89bc1c2edf3210faf4300ef956fbf6.nq.gz
│   ├── dac1363f3cd89fdcb42474122c61cc6a7f09438b.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── edf2acb5fa8020ea28f5a3278a7ead7c0060874d.nq.gz
│   ├── ee9ec8ff42da543bf30a54be622c56baef5ca84e.nq.gz
│   ├── eece5b7a99563d9242e28c0b628336d3b71633be.nq.gz
│   ├── ef5717137b2da17b335ce054c60db898a3ef605d.nq.gz
│   └── f3a7ef38941b46810d566277753d069b17e3a20a.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── ea3c4723e4cefdac760d483ccac6c8a428c95ab8.nq.gz
├── filetree
│   └── ea3c4723e4cefdac760d483ccac6c8a428c95ab8.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 49 files
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

[NousResearch/Hermes-Function-Calling](https://github.com/NousResearch/Hermes-Function-Calling)

---
*Parsed on 2026-10-01 by [repolex](https://repolex.ai)*
