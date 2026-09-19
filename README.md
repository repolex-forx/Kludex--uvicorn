# Repolex Knowledge Graph of Kludex/uvicorn

RDF knowledge graph data for [Kludex/uvicorn](https://github.com/Kludex/uvicorn), parsed by [repolex](https://repolex.ai).

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
lexq download Kludex/uvicorn
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea
│   │   │   └── chunk-001.nq.gz
│   │   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c
│   │   │   └── chunk-001.nq.gz
│   │   └── edb54c43c0321c0b41eee1473f3f4cf145e8927f
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea.nq.gz
│   │   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf.nq.gz
│   │   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2.nq.gz
│   │   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c.nq.gz
│   │   └── edb54c43c0321c0b41eee1473f3f4cf145e8927f.nq.gz
│   └── repolex
│       ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea
│       │   └── chunk-001.nq.gz
│       ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf
│       │   └── chunk-001.nq.gz
│       ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2
│       │   └── chunk-001.nq.gz
│       ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c
│       │   └── chunk-001.nq.gz
│       └── edb54c43c0321c0b41eee1473f3f4cf145e8927f
│           └── chunk-001.nq.gz
├── blob
│   ├── 001c08df7cebe63fcbb0edafe57b641f040e8160.nq.gz
│   ├── 00dab39b6a23e9d85b82af733900443390fd8c6e.nq.gz
│   ├── 0165256254142b24c49d29e346eb97de1cae40de.nq.gz
│   ├── 0174bcce6d48de946214d59bcae5543d38d89c3a.nq.gz
│   ├── 02f455d8eefd53ef88da5424315589610bf7edd7.nq.gz
│   ├── 039b554df7304f7987536637e11466f0c4cc8b36.nq.gz
│   ├── 0492cc33e934a75b14a2f1765c5a208785e2b48e.nq.gz
│   ├── 075ec2401621e039f9a353e2f080d27544f1693a.nq.gz
│   ├── 091004a238069f51c6b7704153932361d23fd945.nq.gz
│   ├── 0950d5276aeaf133999e7c320ea2605d4ef871c6.nq.gz
│   ├── 0c9c20f1c819b5525c3e76a6f18102b3cd796c57.nq.gz
│   ├── 118a19ac0c43e518a24cf1108bfbb9dde507bd0c.nq.gz
│   ├── 129b38b63c89a5d5f48846c0ea9339c64035a4f0.nq.gz
│   ├── 16188c91d34743ec196308ec0f16ad47353f5300.nq.gz
│   ├── 1691edd7f61ecfbef3d720375b35890debc36845.nq.gz
│   ├── 16b47cd0ec15c702d8d15ea858f93cb2693b3f44.nq.gz
│   ├── 1721e4c4610689b08d7ceda62016750e9a33a007.nq.gz
│   ├── 1811b43972b186729e104165e37c3ef93de25e6e.nq.gz
│   ├── 190839905566f0c0e59c6119604887c326078115.nq.gz
│   ├── 194fc18c7832e80bc9b8700abd9d3c3c3a386ad6.nq.gz
│   ├── 1ae45f40dd1d670ca0b2c29dbdae14b6fb02e9e5.nq.gz
│   ├── 1bb447fc4a4c6fb59000751d33d782aac232877d.nq.gz
│   ├── 1d8cd4a51f74c05a70734cb9383ce487a93ce859.nq.gz
│   ├── 1e873f649981948ec292348e0095c8736524b918.nq.gz
│   ├── 1fb6804a361bf40faaa9e2512ad391b99ca53ff1.nq.gz
│   ├── 21f95d5d6d9985a06e41eb90d152471382f9c492.nq.gz
│   ├── 2302648eadbe315e060c4c9dbadaed5d1ec4fe13.nq.gz
│   ├── 23fdd9ceff218374929f05bf3b1cd14a2948fc93.nq.gz
│   ├── 24a3feb5115a3d6866665eae300e391396443222.nq.gz
│   ├── 28693f9cc6d14ed8ea98518a78162e8c84f51c72.nq.gz
│   ├── 2a3725f6fd07deed4ff30234e8d5fbb7b7db63e0.nq.gz
│   ├── 2ad140c8b5464f68771a7e9620b37bfcb92c2344.nq.gz
│   ├── 2b18f8e89c8047915df7fb83a2d1699ed464072a.nq.gz
│   ├── 2b87e6d8ad9217cfafa96ab7b0f00bfabbdec5f2.nq.gz
│   ├── 2d1b5fa2d3366fd6584181a26c8569a0207900cc.nq.gz
│   ├── 2e94ba178a2efd56e62158d2cf5ef585254385be.nq.gz
│   ├── 312bd56756860ff4a6f541fcf48bd857482f57d5.nq.gz
│   ├── 34ad2c75ceb711d0861eee90864693a3417d6bc0.nq.gz
│   ├── 371fdcaf992afee5d4be1edab7ec1b65e0c232a7.nq.gz
│   ├── 3764845548829bec468942b64f3de958828f00b8.nq.gz
│   ├── 37f6c9300c70784846b2cde20540efc03fdca579.nq.gz
│   ├── 39bb27944aa72b5e0924ef11db32544c96d62c62.nq.gz
│   ├── 39e81fa7a2e1f2cf2d3a98794ea966739ace310d.nq.gz
│   ├── 3ad98afab2bd5f6d6d729b7d3ad7c50ed5c6b941.nq.gz
│   ├── 3be0c6e39e9c2fe0c656f8b79aabd39cf1e8a2fe.nq.gz
│   ├── 3d52a24ede1ef8d9caaae9e944be84c4d495b3f3.nq.gz
│   ├── 423c0d3600b6ff462f23141d9bc628c0deb37c00.nq.gz
│   ├── 45f33bef83d8b4a1aef7e91213746ff7297fc60f.nq.gz
│   ├── 46832413fd36be95f1094e3e3b52f38e88e1977b.nq.gz
│   ├── 49195978c01a0aa30f24240e24f77929674fcacd.nq.gz
│   ├── 4c43a32fe4757c60b8cd9ff47472ef73b4df8f45.nq.gz
│   ├── 4c6f62fb125e0038ad2e49fa59773fc94fe39c5d.nq.gz
│   ├── 4da2ae1f4a56e6850b3aee14ec90c4252c981cc1.nq.gz
│   ├── 4e15d1599bab04ac38f56cf271d2ff9b1b9984c8.nq.gz
│   ├── 4f75dbdedb4bf6eb33d351e1aa9d4b0659dcedac.nq.gz
│   ├── 4f7feba6eb97d88e2d060888d00ad338d5aef9d3.nq.gz
│   ├── 5207cfb7d425977ed0d66047ba5c8f7888d95610.nq.gz
│   ├── 52666bca6359f0e5bf8f193e27d6ed42b6dfed3c.nq.gz
│   ├── 57e71b88405515bed30a9af5fcd140177a355982.nq.gz
│   ├── 598c83ba34a3035aa00e62b2e5351a24cd05f042.nq.gz
│   ├── 5da02c2eaa248ec3538ecf1374263c16613fa9bb.nq.gz
│   ├── 600990595274dbc649176247c0c15840e59e0105.nq.gz
│   ├── 6097cd5729cd39b376886a9f926d8b1ed9f70919.nq.gz
│   ├── 66e34f53ffe62df65284d914bbf7d44a268b4917.nq.gz
│   ├── 6c2ccbdcc424988b67245a751e7ee40694a51a7c.nq.gz
│   ├── 6c61844c247ef00d8eb3a25639a9cfb830a8f066.nq.gz
│   ├── 6efbd54413f021a3a706881ffad41fce211d02fa.nq.gz
│   ├── 6f593e9716aeb3ec85aa64f2e7d8d283c7744db0.nq.gz
│   ├── 7061a143bf56c4951ea03e198fe67402a29ae6aa.nq.gz
│   ├── 70807e1fe2a1f730fb3ea66f1970e2bb32a937c2.nq.gz
│   ├── 717091604a929acb58a557611c1c690e7c112cd9.nq.gz
│   ├── 7180ad39788c6fb14e15ae3fda379aba01c332f8.nq.gz
│   ├── 71ac39472e9e07025f25c62b074b1d44df39cf8e.nq.gz
│   ├── 74554b1e2a149c37131168fbe283f3e2476a8f75.nq.gz
│   ├── 766790a39e88947b2a98485505777b7c8b457681.nq.gz
│   ├── 7cb6f6e22371151f592e6ff1720146756255c017.nq.gz
│   ├── 7e070c684b8dd90acc9e6125e525ca90dd02771a.nq.gz
│   ├── 80578a59de72487c2041d14db3a36c957cd123d2.nq.gz
│   ├── 80671396ba940ec2403d4c64ef996c2a88929269.nq.gz
│   ├── 8145a2bd28b9d2f7442999fc807ac9677903b410.nq.gz
│   ├── 822445a7b58bb5b0726a9be205e8855a958dcdcf.nq.gz
│   ├── 827d091c0f1693a43ae030b55e6ff79f7a552192.nq.gz
│   ├── 880982afacd8115105d0c156585873bf43ad3f9f.nq.gz
│   ├── 89368fa98131b053625adbfd0208cd124d7b1aa1.nq.gz
│   ├── 8a1dc979a39e36ce81e987843391479f125d73f3.nq.gz
│   ├── 8acce68002c927614f5b8abb3e7c950db3580b86.nq.gz
│   ├── 8b137891791fe96927ad78e64b0aad7bded08bdc.nq.gz
│   ├── 8b26fb17a54086f60e72f48a0307cbe193f67119.nq.gz
│   ├── 8be916c9ad6f2ce67ddeb84490a6c5212123739f.nq.gz
│   ├── 8c4ecf00db5dac56c5f7d5c1d57b5901edaed160.nq.gz
│   ├── 8c9ab8e889cb852c515655ebc8404481b82adbf4.nq.gz
│   ├── 90a9c910eb144b8c064deb96991b02a555591fbb.nq.gz
│   ├── 90c47a8b2c6117c5a8e23995c2730451bd4225f7.nq.gz
│   ├── 91704e36beba57b8f47549a23caf9b7fb396abe8.nq.gz
│   ├── 93191bacbf1b56470b11601dc683c111d12f33e7.nq.gz
│   ├── 938a6aaa905035fdd0b4af66133a89cefacd73f5.nq.gz
│   ├── 93c85cb7661015e40a1ed568d692c8741a6faacb.nq.gz
│   ├── 94508f55fec5b4a21a11efae7787a4bcd51b939f.nq.gz
│   ├── 95ea617d41e1fd6d88198818be55503a09c0f8a6.nq.gz
│   ├── 96c63c55a227cc4e46b0a092ad010f886515eb8d.nq.gz
│   ├── 9727bdab93cf821e2017cfb2d0c32bf9b8b21d94.nq.gz
│   ├── 972fb7caab3cb5eaebdf15164b7e0791ace50c6f.nq.gz
│   ├── 99ee455a06a43e5e6376d0e93735ddf609a0b09b.nq.gz
│   ├── 9dfcbe8f492c8773f1ae9b5fca65100bd1c8235d.nq.gz
│   ├── 9ee622e0d43ac0810a97620a67217835fcf9b5e8.nq.gz
│   ├── 9f024e93a79665e92da8055e12d3273e9a754ebf.nq.gz
│   ├── a02baff3a0c7f6490db663430eb8e1d48d594bcd.nq.gz
│   ├── a14bec144a97a5e3718a768abe3b6a9e7e93d2c1.nq.gz
│   ├── a23c2fb63ef887c2c64aada8d8977148a5f39950.nq.gz
│   ├── a252a87f6ff1b155a3d27bbb30ba4190de22f8d3.nq.gz
│   ├── a2720c574c99861e748a3347c97301ed43a2250e.nq.gz
│   ├── a36b83672673d87b618d0cc3e36a551f2908ae80.nq.gz
│   ├── a604862d6648da286eeac287f85edd301f677890.nq.gz
│   ├── a69aa937f95bbbbe1f66f7ca21d4123988eeff9d.nq.gz
│   ├── a6bba14552c7673a7db57a5750ddb06508264273.nq.gz
│   ├── a9a89065c70d7a7905d4b44bc3c385a492cc0d70.nq.gz
│   ├── aa3b0e733b60e0ea9ae15c8371f2d283ebc63e32.nq.gz
│   ├── aa8097a5b5da188f0a83eed7d0db658c4e885e8c.nq.gz
│   ├── ab767f6602ce90fd29b917799aef3cbccdb37391.nq.gz
│   ├── ac4896b8c85198930d55fae40449e8b7876e2abe.nq.gz
│   ├── ad6121ee086b0c3b2fc2cb8dd378134725c1edf6.nq.gz
│   ├── af5309ee923c061093533ea7921aeae75cc7d85d.nq.gz
│   ├── b2109c4062d3ce3e285555e0ac66d191709d4c76.nq.gz
│   ├── b2e3cb77d421085947741430e8b5451821eb66c7.nq.gz
│   ├── b47a7e94d5ab93d3e52a8d92657afef6b9302f12.nq.gz
│   ├── b4d4143bd1d74fd2b396b2e326fe2f773b27486c.nq.gz
│   ├── b73958624876a7c03f1b2f11c7943ee6e207e1a7.nq.gz
│   ├── b9ee14a6c760840e01b62f6bd91685e77a2ef271.nq.gz
│   ├── ba49c4bfb293b2c7835f344f6adad09660539421.nq.gz
│   ├── bb0afe9d58c61873335c41ded59034b43fe00ecc.nq.gz
│   ├── bc9e1f016afca2ae14c2e93dc07a00da7024c36b.nq.gz
│   ├── bd16115311a2c4deb4f5de0131d5cdfb14049980.nq.gz
│   ├── bdcfdea214e8a671d81dec45afd74156e48d1f70.nq.gz
│   ├── bec869a05d6af96ad7a7a5a661ed3bc64f9d4a89.nq.gz
│   ├── bf78d169a1dff854f5ce03b216bbfcaf6b621953.nq.gz
│   ├── c084ec90b6a16c9e4824808d22283642e2757ded.nq.gz
│   ├── c14513ba97085f9130bea614c7e56a1724a98331.nq.gz
│   ├── c329c281683b4f45f8cfcca2a956b23ac888058f.nq.gz
│   ├── c6692c58f5c63501b2ad0f3d3c1d6b2336d88aad.nq.gz
│   ├── c67d04aaf7e786aecb325e5900aa9f7cf7366fa3.nq.gz
│   ├── c88fdf53bbb1126c617a516e5829e139219a9c06.nq.gz
│   ├── c9c0d64cebc87d4360a585f6b2b16bf97bae30ff.nq.gz
│   ├── cd3d701bb9f78888fa433a9d36ec937069f1baf8.nq.gz
│   ├── cfceb6b94ce36dad006b1f81b816d45ce70ab3d6.nq.gz
│   ├── d09efad8301cf20c505ac9656261589a7c162be9.nq.gz
│   ├── d53a8b06d933ef4bbc43b4149d0ebe61b7433eb1.nq.gz
│   ├── d70ba642b258ce804fe2646f77728e6e27700e37.nq.gz
│   ├── d7e3688885b617da9abd80ec0af157aa210c65d7.nq.gz
│   ├── da58a9c30efa873c2c25971a78b146bfc00fa206.nq.gz
│   ├── da60bb8ddb8bb6e575910d47b8429af34b478e05.nq.gz
│   ├── de5b237597ac87e55cdf2ac58ae878b93860c615.nq.gz
│   ├── dfba2c20c5284a2afee462d00d9ed08df278e570.nq.gz
│   ├── dfca3c55bdcb4a783ba7c954279a147f10c83a03.nq.gz
│   ├── dfd7ce7eab627564cf80648e641f45ffeedc8d6f.nq.gz
│   ├── e05140c779c2cfad18edb077bc90a46a48f2a6fa.nq.gz
│   ├── e4139391a2d199e2f2d1f67c232693774875f57a.nq.gz
│   ├── e4b055e13bf54873a40b100f0c52ae33d93461d7.nq.gz
│   ├── e601afbb07b7014faac0c8680b06cf1e3882ac71.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ed257a1eef6107ee578b918c54e00b1d522f6d80.nq.gz
│   ├── ed8bcf67eaa964e2be223be9f4ee068de58a10b8.nq.gz
│   ├── f0c2f8aa2231a966594908ce69edeff6be9a746c.nq.gz
│   ├── f656a8813cf050d78f98237911dd9e5dbd14c709.nq.gz
│   ├── f77520ee106deeedee30a48005479806ff9a19e2.nq.gz
│   ├── f9995e59b859a3914564d537baaccdd36bb02c5a.nq.gz
│   ├── fa1f5f432a69660abccc212ef287e2c232aa8fdc.nq.gz
│   ├── fb41547ba214b164b20082f05f6a267c48d9bf5f.nq.gz
│   ├── fbbd20f1ec0b33dc9523637f1548d0fc828042df.nq.gz
│   └── fe90d09e9a5d75e7dffdb182c42bb93a1e1e63a2.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea.nq.gz
│   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf.nq.gz
│   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2.nq.gz
│   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c.nq.gz
│   └── edb54c43c0321c0b41eee1473f3f4cf145e8927f.nq.gz
├── filetree
│   ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea.nq.gz
│   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf.nq.gz
│   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2.nq.gz
│   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c.nq.gz
│   └── edb54c43c0321c0b41eee1473f3f4cf145e8927f.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

23 directories, 199 files
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

[Kludex/uvicorn](https://github.com/Kludex/uvicorn)

---
*Parsed on 2026-09-19 by [repolex](https://repolex.ai)*
