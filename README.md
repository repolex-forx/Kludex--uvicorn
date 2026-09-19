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
│   │   ├── 0e3b18c39959ad4ec8bfe6cb7e11c82664aaa702
│   │   │   └── chunk-001.nq.gz
│   │   ├── 137f88ea3224b8134fc58ed1243881642382d31b
│   │   │   └── chunk-001.nq.gz
│   │   ├── 1dfb0bd885bbb0c466c19eee8bb2001bed59ca8c
│   │   │   └── chunk-001.nq.gz
│   │   ├── 3850ad6520cafb290bd4174fa9c4ca5d33440c82
│   │   │   └── chunk-001.nq.gz
│   │   ├── 4098bcac97aa0fbda2f4e73278fbbe3b128be940
│   │   │   └── chunk-001.nq.gz
│   │   ├── 4f40b8495772eb3a1ab3613ffd7be5156f8e1389
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5279296e620fad6c6839263c279ff23b4be8df32
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5e33d430f13622c8363fe74d97963ab37f3df3c2
│   │   │   └── chunk-001.nq.gz
│   │   ├── 695820ae9bf6b3867f3634bc0776681a7ddf9dd7
│   │   │   └── chunk-001.nq.gz
│   │   ├── 7983c1ae9c2276b94cd85217f7aa58bb248847c4
│   │   │   └── chunk-001.nq.gz
│   │   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c
│   │   │   └── chunk-001.nq.gz
│   │   ├── a50051308509600388ed170fdedacfb673757de4
│   │   │   └── chunk-001.nq.gz
│   │   ├── a50753268a9033dcdc57d6dee45f3829cdedf8f0
│   │   │   └── chunk-001.nq.gz
│   │   ├── bdf95fd3e71f5f904dc6f7f1194a5fe23d1c3f2f
│   │   │   └── chunk-001.nq.gz
│   │   ├── daecb45327702efe8f702f46fb0870c2d6357837
│   │   │   └── chunk-001.nq.gz
│   │   ├── edb54c43c0321c0b41eee1473f3f4cf145e8927f
│   │   │   └── chunk-001.nq.gz
│   │   └── fe3910083e3990695bc19c2ef671dd447262ae18
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea.nq.gz
│   │   ├── 0e3b18c39959ad4ec8bfe6cb7e11c82664aaa702.nq.gz
│   │   ├── 137f88ea3224b8134fc58ed1243881642382d31b.nq.gz
│   │   ├── 1dfb0bd885bbb0c466c19eee8bb2001bed59ca8c.nq.gz
│   │   ├── 3850ad6520cafb290bd4174fa9c4ca5d33440c82.nq.gz
│   │   ├── 4098bcac97aa0fbda2f4e73278fbbe3b128be940.nq.gz
│   │   ├── 4f40b8495772eb3a1ab3613ffd7be5156f8e1389.nq.gz
│   │   ├── 5279296e620fad6c6839263c279ff23b4be8df32.nq.gz
│   │   ├── 5e33d430f13622c8363fe74d97963ab37f3df3c2.nq.gz
│   │   ├── 695820ae9bf6b3867f3634bc0776681a7ddf9dd7.nq.gz
│   │   ├── 7983c1ae9c2276b94cd85217f7aa58bb248847c4.nq.gz
│   │   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf.nq.gz
│   │   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2.nq.gz
│   │   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c.nq.gz
│   │   ├── a50051308509600388ed170fdedacfb673757de4.nq.gz
│   │   ├── a50753268a9033dcdc57d6dee45f3829cdedf8f0.nq.gz
│   │   ├── bdf95fd3e71f5f904dc6f7f1194a5fe23d1c3f2f.nq.gz
│   │   ├── daecb45327702efe8f702f46fb0870c2d6357837.nq.gz
│   │   ├── edb54c43c0321c0b41eee1473f3f4cf145e8927f.nq.gz
│   │   └── fe3910083e3990695bc19c2ef671dd447262ae18.nq.gz
│   └── repolex
│       ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea
│       │   └── chunk-001.nq.gz
│       ├── 0e3b18c39959ad4ec8bfe6cb7e11c82664aaa702
│       │   └── chunk-001.nq.gz
│       ├── 137f88ea3224b8134fc58ed1243881642382d31b
│       │   └── chunk-001.nq.gz
│       ├── 1dfb0bd885bbb0c466c19eee8bb2001bed59ca8c
│       │   └── chunk-001.nq.gz
│       ├── 3850ad6520cafb290bd4174fa9c4ca5d33440c82
│       │   └── chunk-001.nq.gz
│       ├── 4098bcac97aa0fbda2f4e73278fbbe3b128be940
│       │   └── chunk-001.nq.gz
│       ├── 4f40b8495772eb3a1ab3613ffd7be5156f8e1389
│       │   └── chunk-001.nq.gz
│       ├── 5279296e620fad6c6839263c279ff23b4be8df32
│       │   └── chunk-001.nq.gz
│       ├── 5e33d430f13622c8363fe74d97963ab37f3df3c2
│       │   └── chunk-001.nq.gz
│       ├── 695820ae9bf6b3867f3634bc0776681a7ddf9dd7
│       │   └── chunk-001.nq.gz
│       ├── 7983c1ae9c2276b94cd85217f7aa58bb248847c4
│       │   └── chunk-001.nq.gz
│       ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf
│       │   └── chunk-001.nq.gz
│       ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2
│       │   └── chunk-001.nq.gz
│       ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c
│       │   └── chunk-001.nq.gz
│       ├── a50051308509600388ed170fdedacfb673757de4
│       │   └── chunk-001.nq.gz
│       ├── a50753268a9033dcdc57d6dee45f3829cdedf8f0
│       │   └── chunk-001.nq.gz
│       ├── bdf95fd3e71f5f904dc6f7f1194a5fe23d1c3f2f
│       │   └── chunk-001.nq.gz
│       ├── daecb45327702efe8f702f46fb0870c2d6357837
│       │   └── chunk-001.nq.gz
│       ├── edb54c43c0321c0b41eee1473f3f4cf145e8927f
│       │   └── chunk-001.nq.gz
│       └── fe3910083e3990695bc19c2ef671dd447262ae18
│           └── chunk-001.nq.gz
└── blob
    ├── 001c08df7cebe63fcbb0edafe57b641f040e8160.nq.gz
    ├── 00dab39b6a23e9d85b82af733900443390fd8c6e.nq.gz
    ├── 00f1fb720756628fb1daf30cab68624a598e09a6.nq.gz
    ├── 0165256254142b24c49d29e346eb97de1cae40de.nq.gz
    ├── 0174bcce6d48de946214d59bcae5543d38d89c3a.nq.gz
    ├── 017ae769f81a89149b92c97ee3c0c3af6a2bd408.nq.gz
    ├── 02544382040cd438717a91d57820bfb6a45f80a0.nq.gz
    ├── 02f455d8eefd53ef88da5424315589610bf7edd7.nq.gz
    ├── 039b554df7304f7987536637e11466f0c4cc8b36.nq.gz
    ├── 0492cc33e934a75b14a2f1765c5a208785e2b48e.nq.gz
    ├── 061805b6c31f8b086c64e3e2a9339f058c09169e.nq.gz
    ├── 069d63923ec8b95bbbb5fef3b5dc3bd92a8781bd.nq.gz
    ├── 06fdf295eeb6ae0a513f145077bf57c3bde3a9a3.nq.gz
    ├── 072dec942d7c1358b1d78787b0451ff020955b98.nq.gz
    ├── 074c01d0339a46835196be6e8a9672b8b103e7f5.nq.gz
    ├── 075ec2401621e039f9a353e2f080d27544f1693a.nq.gz
    ├── 078de1af01579e2020303ad1ee65481f84db0c84.nq.gz
    ├── 08fd13678a1c4dffe3e126acf0167c17d62c2ed8.nq.gz
    ├── 091004a238069f51c6b7704153932361d23fd945.nq.gz
    ├── 0950d5276aeaf133999e7c320ea2605d4ef871c6.nq.gz
    ├── 09df984ea1b184c0af9666c98d0709364de024c5.nq.gz
    ├── 09e24071e8f9ab620662505e6b69d720dfcb0e77.nq.gz
    ├── 09e863e40e68d456f5d5ef0455ccff21d3dce578.nq.gz
    ├── 0a8996666f28fb71654b29e63aee616da663f1df.nq.gz
    ├── 0a8f431f4e1663852304160f6835d2036c7c7802.nq.gz
    ├── 0ade97450a1056c2aaf0c391418789dd2b14820e.nq.gz
    ├── 0ba903e5ef8ead9f1a9866cf267372673926220d.nq.gz
    ├── 0c3ef1fa50c39751a1ea51cea137f43953713b17.nq.gz
    ├── 0c9c20f1c819b5525c3e76a6f18102b3cd796c57.nq.gz
    ├── 0ccd3592a7aebf34b6fde2830f30ca53e94cd74d.nq.gz
    ├── 0d3b9b77e611d2d861fdaaa2940a78b03aee8a91.nq.gz
    ├── 0e2fd1eb05efc526f660bcf10e865d2fe781a239.nq.gz
    ├── 0e8f4b2be991fd10687d1ed1e29f98d6b1da0369.nq.gz
    ├── 10e422cbf6da104ad200f15f771e55020f5c6528.nq.gz
    ├── 118a19ac0c43e518a24cf1108bfbb9dde507bd0c.nq.gz
    ├── 12262c39f59c48cd2147df1100b573c14cedad98.nq.gz
    ├── 129b38b63c89a5d5f48846c0ea9339c64035a4f0.nq.gz
    ├── 1404ba8e92964b6a4126aa565f0683dd9625efda.nq.gz
    ├── 14f5011080190f3dc7171dea26624af792614923.nq.gz
    ├── 15748a4e82f649f892b1b8424661f857655b6421.nq.gz
    ├── 15ccfdd7d31269f40e9b20450f3258bbdfeae6d8.nq.gz
    ├── 15fdd860756b148c68d12074ade5ad6ad8c916cb.nq.gz
    ├── 16188c91d34743ec196308ec0f16ad47353f5300.nq.gz
    ├── 1691edd7f61ecfbef3d720375b35890debc36845.nq.gz
    ├── 16b47cd0ec15c702d8d15ea858f93cb2693b3f44.nq.gz
    ├── 1721e4c4610689b08d7ceda62016750e9a33a007.nq.gz
    ├── 17ee643c5b84b75993b3f95b386a4fcad05e0d7f.nq.gz
    ├── 1811b43972b186729e104165e37c3ef93de25e6e.nq.gz
    ├── 190839905566f0c0e59c6119604887c326078115.nq.gz
    ├── 194ce8347af95e02330d568675c6460ffdd03be8.nq.gz
    ├── 194fc18c7832e80bc9b8700abd9d3c3c3a386ad6.nq.gz
    ├── 19c11d65aaac4e58940f9082f6abe5ffa1a4daea.nq.gz
    ├── 1ae45f40dd1d670ca0b2c29dbdae14b6fb02e9e5.nq.gz
    ├── 1b04d208e3f80d4050690cfc9c4956506c5c813d.nq.gz
    ├── 1b0c0e84e54842ac7e13edabc43ca33978cad2f7.nq.gz
    ├── 1bb447fc4a4c6fb59000751d33d782aac232877d.nq.gz
    ├── 1bead4a061cc0989ffcd999ffeb0a7279ec25b4f.nq.gz
    ├── 1c06844de5f1e1fa06394e42d11259c65555cd14.nq.gz
    ├── 1cfa88672eccefd45f490a4ae32684937fd0c982.nq.gz
    ├── 1d240c7e405c6c10c4a02b1a4ed3fb3ded80380e.nq.gz
    ├── 1d8cd4a51f74c05a70734cb9383ce487a93ce859.nq.gz
    ├── 1e873f649981948ec292348e0095c8736524b918.nq.gz
    ├── 1e895cd493f81dc4a83b81321410a7317487fff0.nq.gz
    ├── 1eff6b930a3f33fb8b70662048b47f6d784862dc.nq.gz
    ├── 1f79b37868f0ef832c32b1a2d7c0d93b7ff8d421.nq.gz
    ├── 1fb6804a361bf40faaa9e2512ad391b99ca53ff1.nq.gz
    ├── 2193e81945c2955a6b6559b3c91f758e6d137ccc.nq.gz
    ├── 21f95d5d6d9985a06e41eb90d152471382f9c492.nq.gz
    ├── 222f13e64ab68875d77c86feccee926fc5dc644b.nq.gz
    ├── 2285457bf181d31d36b74ba6c368eac604178645.nq.gz
    ├── 2302648eadbe315e060c4c9dbadaed5d1ec4fe13.nq.gz
    ├── 23fdd9ceff218374929f05bf3b1cd14a2948fc93.nq.gz
    ├── 23fe61784c7104d61ad78c2bdb4d05f039b86c99.nq.gz
    ├── 24a3feb5115a3d6866665eae300e391396443222.nq.gz
    ├── 2562143106038ede63de00a2e4766d26d35bec96.nq.gz
    ├── 2869183d9bffdca7c4da8bb8551e1fa743f286ec.nq.gz
    ├── 28693f9cc6d14ed8ea98518a78162e8c84f51c72.nq.gz
    ├── 29914a5ee3df6854715bf570a6ad41a8a54792d6.nq.gz
    ├── 2a3725f6fd07deed4ff30234e8d5fbb7b7db63e0.nq.gz
    ├── 2ad140c8b5464f68771a7e9620b37bfcb92c2344.nq.gz
    ├── 2b18f8e89c8047915df7fb83a2d1699ed464072a.nq.gz
    ├── 2b87e6d8ad9217cfafa96ab7b0f00bfabbdec5f2.nq.gz
    ├── 2d1b5fa2d3366fd6584181a26c8569a0207900cc.nq.gz
    ├── 2d6ea60ee6aa7a3e620d0e8f20314013dd82fa5f.nq.gz
    ├── 2e0830f0d7b99c8c06fff4e0fa248f893214ca40.nq.gz
    ├── 2e1a33ad0c528ce06b2a98ec1c96e2707ca5c66e.nq.gz
    ├── 2e5813738009b79ca30ceffd6b6ec1402f46cb47.nq.gz
    ├── 2e94ba178a2efd56e62158d2cf5ef585254385be.nq.gz
    ├── 2f87d94ca10327497ac0f4c0093930826ff76642.nq.gz
    ├── 303ae6feb52ec9f03d0bf6c446fb3a9ba197960f.nq.gz
    ├── 30eea2321e82be074828e00434c7d3519a0c214d.nq.gz
    ├── 312bd56756860ff4a6f541fcf48bd857482f57d5.nq.gz
    ├── 32e98cd447e2b0f4e755a46c71b95e3e8a6b8c91.nq.gz
    ├── 3424aadb63bccca3093da45dfd2c4c9388b09906.nq.gz
    ├── 3438ddf80e47543a48c6ed9a6454e6cd9d84467d.nq.gz
    ├── 34ad2c75ceb711d0861eee90864693a3417d6bc0.nq.gz
    ├── 35266f5a38458e21cecb23d75ef583567798ce67.nq.gz
    ├── 363f4ba37214346f61f4fd97fc036d19f4a7c8d9.nq.gz
    ├── 371fdcaf992afee5d4be1edab7ec1b65e0c232a7.nq.gz
    ├── 3764845548829bec468942b64f3de958828f00b8.nq.gz
    ├── 37f6c9300c70784846b2cde20540efc03fdca579.nq.gz
    ├── 385a8b76ca8aeb0a4cc535297105f227f6eca511.nq.gz
    ├── 39bb27944aa72b5e0924ef11db32544c96d62c62.nq.gz
    ├── 39e81fa7a2e1f2cf2d3a98794ea966739ace310d.nq.gz
    ├── 3ad98afab2bd5f6d6d729b7d3ad7c50ed5c6b941.nq.gz
    ├── 3be0c6e39e9c2fe0c656f8b79aabd39cf1e8a2fe.nq.gz
    ├── 3c839899807beb537128aba05e0923461f3e06bd.nq.gz
    ├── 3d52a24ede1ef8d9caaae9e944be84c4d495b3f3.nq.gz
    ├── 3e6c2abbe0ed69857903fa7288b97a5a5adaa826.nq.gz
    ├── 3ece31f8813760aab9f6b3b982f65a8661135223.nq.gz
    ├── 3f2e9a64d0eb61304678019e0cdcd43a24f8244a.nq.gz
    ├── 402b723d0e7575df62c0236d8e3b1cca7ea4724b.nq.gz
    ├── 417f29df7e90c453178a98fedcf15d8a97ab997c.nq.gz
    ├── 423c0d3600b6ff462f23141d9bc628c0deb37c00.nq.gz
    ├── 4380cbd94146d18c9f0e325d33686af0dea71f8d.nq.gz
    ├── 43956622db68f2de8200b33b740a68114233fc55.nq.gz
    ├── 44eb9970b1c37633142d95b40dfe4734864d3b5b.nq.gz
    ├── 45f33bef83d8b4a1aef7e91213746ff7297fc60f.nq.gz
    ├── 46832413fd36be95f1094e3e3b52f38e88e1977b.nq.gz
    ├── 48236d9ed84a966634f40d62f4ae997fc8093d56.nq.gz
    ├── 49195978c01a0aa30f24240e24f77929674fcacd.nq.gz
    ├── 4c43a32fe4757c60b8cd9ff47472ef73b4df8f45.nq.gz
    ├── 4c6f62fb125e0038ad2e49fa59773fc94fe39c5d.nq.gz
    ├── 4d70addbad8afc7a5a8220bf2f7475ce6e4f9395.nq.gz
    ├── 4da2ae1f4a56e6850b3aee14ec90c4252c981cc1.nq.gz
    ├── 4df50af33f804651539767cc9f041aa21331908e.nq.gz
    ├── 4e15d1599bab04ac38f56cf271d2ff9b1b9984c8.nq.gz
    ├── 4f75dbdedb4bf6eb33d351e1aa9d4b0659dcedac.nq.gz
    ├── 4f7feba6eb97d88e2d060888d00ad338d5aef9d3.nq.gz
    ├── 5120d2a041309cb9ffbf0d2e3c745e15abf1e4b5.nq.gz
    ├── 5207cfb7d425977ed0d66047ba5c8f7888d95610.nq.gz
    ├── 52198239e052f2f0dca32ec2852cd4f8c0a966ab.nq.gz
    ├── 52666bca6359f0e5bf8f193e27d6ed42b6dfed3c.nq.gz
    ├── 52ac03e332825206d25fe6630158b7f7194f8242.nq.gz
    ├── 5488cf242f232e4c32f3168517653a0d5376e96f.nq.gz
    ├── 56362f20f0ae9c11d6107d97f80ce6b60bd27c44.nq.gz
    ├── 57804e799c9603eb2b6c930d04ce9043a6b409f1.nq.gz
    ├── 57e71b88405515bed30a9af5fcd140177a355982.nq.gz
    ├── 59655bdafed24a7ba5e95e5f950f21b5af79852a.nq.gz
    └── 598c83ba34a3035aa00e62b2e5351a24cd05f042.nq.gz

46 directories, 200 files
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
