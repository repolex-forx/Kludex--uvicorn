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
│   │   ├── 11d28e208504436e7e06603a941c01b76f54346f
│   │   │   └── chunk-001.nq.gz
│   │   ├── 137f88ea3224b8134fc58ed1243881642382d31b
│   │   │   └── chunk-001.nq.gz
│   │   ├── 1c20f546574cc905a8b28a5390c3f815e27a84ab
│   │   │   └── chunk-001.nq.gz
│   │   ├── 1dfb0bd885bbb0c466c19eee8bb2001bed59ca8c
│   │   │   └── chunk-001.nq.gz
│   │   ├── 2f22bca659cdcaea6ed37e5c9aa128bf99150eb6
│   │   │   └── chunk-001.nq.gz
│   │   ├── 3850ad6520cafb290bd4174fa9c4ca5d33440c82
│   │   │   └── chunk-001.nq.gz
│   │   ├── 4098bcac97aa0fbda2f4e73278fbbe3b128be940
│   │   │   └── chunk-001.nq.gz
│   │   ├── 41e339dd953a00d071c8bb5704f4671564f9f6e1
│   │   │   └── chunk-001.nq.gz
│   │   ├── 448be75222093041561d136f9f2f5577d6e361ee
│   │   │   └── chunk-001.nq.gz
│   │   ├── 44a3071654d6bfb4449da46aa885769820c4f0da
│   │   │   └── chunk-001.nq.gz
│   │   ├── 4adff7b5f85d388904e5ec53bf76334d773331b1
│   │   │   └── chunk-001.nq.gz
│   │   ├── 4f40b8495772eb3a1ab3613ffd7be5156f8e1389
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5279296e620fad6c6839263c279ff23b4be8df32
│   │   │   └── chunk-001.nq.gz
│   │   ├── 59eeae66e926a7c6c1b6fd1a6d8fbe31719ab1c3
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5bf788f0eb0fc771f5c4eed8f282c7ec256565d2
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5e33d430f13622c8363fe74d97963ab37f3df3c2
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5ee093b37cb410a462bdeec4ade365298d82bd30
│   │   │   └── chunk-001.nq.gz
│   │   ├── 5f142a884ed52790a38b8e34df7060a0c3c6c760
│   │   │   └── chunk-001.nq.gz
│   │   ├── 65ec8d132c37a8338a2f495fa1be9f14bd4368d9
│   │   │   └── chunk-001.nq.gz
│   │   ├── 695820ae9bf6b3867f3634bc0776681a7ddf9dd7
│   │   │   └── chunk-001.nq.gz
│   │   ├── 71043a9c8fb6436a63110179650e32bcae4a6cbf
│   │   │   └── chunk-001.nq.gz
│   │   ├── 73b7bcdcaa663dd9d74a9fcadea0ce3ec1761f2f
│   │   │   └── chunk-001.nq.gz
│   │   ├── 7983c1ae9c2276b94cd85217f7aa58bb248847c4
│   │   │   └── chunk-001.nq.gz
│   │   ├── 7dc027d5fb980c7bd52ab4611f3109a796cec974
│   │   │   └── chunk-001.nq.gz
│   │   ├── 83986d822686739dc033495494ebdc88c4e266e8
│   │   │   └── chunk-001.nq.gz
│   │   ├── 892c7888ec613c49dd5ff826c58acc6c7e349955
│   │   │   └── chunk-001.nq.gz
│   │   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf
│   │   │   └── chunk-001.nq.gz
│   │   ├── 8efa41c7da41f26c893204ff3fd65c0d06aa74ce
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2
│   │   │   └── chunk-001.nq.gz
│   │   ├── 99fafb3c3b15e32dbaa504993161cb0c6898227f
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9a6b3a8249df6e38f3683c457df8297fb1319d80
│   │   │   └── chunk-001.nq.gz
│   │   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c
│   │   │   └── chunk-001.nq.gz
│   │   ├── a05ae6426cc8f224f4f1a995f46a901ab0f5644b
│   │   │   └── chunk-001.nq.gz
│   │   ├── a50051308509600388ed170fdedacfb673757de4
│   │   │   └── chunk-001.nq.gz
│   │   ├── a50753268a9033dcdc57d6dee45f3829cdedf8f0
│   │   │   └── chunk-001.nq.gz
│   │   ├── b06cc6376dfc566637a79607d5755d9519b3d6c6
│   │   │   └── chunk-001.nq.gz
│   │   ├── b52f3f97842dfa59cbef2e1e6f6606d8ea21e4c2
│   │   │   └── chunk-001.nq.gz
│   │   ├── b6b783bb8d2148355b644ab5d143e94a958e511d
│   │   │   └── chunk-001.nq.gz
│   │   ├── bd552df8f95716d53eb6fdea80b8d6d34cbc1968
│   │   │   └── chunk-001.nq.gz
│   │   ├── bdf95fd3e71f5f904dc6f7f1194a5fe23d1c3f2f
│   │   │   └── chunk-001.nq.gz
│   │   ├── bf04afb292fd8704f8b5f24ae113ba74eab3c2e4
│   │   │   └── chunk-001.nq.gz
│   │   ├── bf8f52bec7af4cf391dcabade49213213c5ac84b
│   │   │   └── chunk-001.nq.gz
│   │   ├── c4591651e2488e7ec303dffe387345ca22b940c6
│   │   │   └── chunk-001.nq.gz
│   │   ├── ca24e1b52ca21e2dbe9c94824e042524fc06b831
│   │   │   └── chunk-001.nq.gz
│   │   ├── ccd1aae48e49dd8c9365600fd79e886efe88be1d
│   │   │   └── chunk-001.nq.gz
│   │   ├── cd18c3b14aa810a4a6ebb264b9a297d6f8afb9ac
│   │   │   └── chunk-001.nq.gz
│   │   ├── daecb45327702efe8f702f46fb0870c2d6357837
│   │   │   └── chunk-001.nq.gz
│   │   ├── e659cf5d87c2aaf9ca8863625be436d7694471a4
│   │   │   └── chunk-001.nq.gz
│   │   ├── e674b96c4f9e20c2f6501b0c9e292d386931f9d0
│   │   │   └── chunk-001.nq.gz
│   │   ├── edb54c43c0321c0b41eee1473f3f4cf145e8927f
│   │   │   └── chunk-001.nq.gz
│   │   ├── f3040fba6a9c628c95fd510bcd9714367a0f4f4e
│   │   │   └── chunk-001.nq.gz
│   │   ├── f39933c8501dd6bc2e8e0f5be45819d3ba2caad0
│   │   │   └── chunk-001.nq.gz
│   │   ├── f73b8beeb1499ca5fcec3067cf89dad5326a0984
│   │   │   └── chunk-001.nq.gz
│   │   ├── fe3910083e3990695bc19c2ef671dd447262ae18
│   │   │   └── chunk-001.nq.gz
│   │   ├── fe85206c5c79be52910ff1b7049591adbab72e4d
│   │   │   └── chunk-001.nq.gz
│   │   └── ff54b029b15adc5259cfbbfa2749778179c48d37
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea.nq.gz
│   │   ├── 0e3b18c39959ad4ec8bfe6cb7e11c82664aaa702.nq.gz
│   │   ├── 11d28e208504436e7e06603a941c01b76f54346f.nq.gz
│   │   ├── 137f88ea3224b8134fc58ed1243881642382d31b.nq.gz
│   │   ├── 1c20f546574cc905a8b28a5390c3f815e27a84ab.nq.gz
│   │   ├── 1dfb0bd885bbb0c466c19eee8bb2001bed59ca8c.nq.gz
│   │   ├── 2f22bca659cdcaea6ed37e5c9aa128bf99150eb6.nq.gz
│   │   ├── 3850ad6520cafb290bd4174fa9c4ca5d33440c82.nq.gz
│   │   ├── 4098bcac97aa0fbda2f4e73278fbbe3b128be940.nq.gz
│   │   ├── 41e339dd953a00d071c8bb5704f4671564f9f6e1.nq.gz
│   │   ├── 448be75222093041561d136f9f2f5577d6e361ee.nq.gz
│   │   ├── 44a3071654d6bfb4449da46aa885769820c4f0da.nq.gz
│   │   ├── 4adff7b5f85d388904e5ec53bf76334d773331b1.nq.gz
│   │   ├── 4f40b8495772eb3a1ab3613ffd7be5156f8e1389.nq.gz
│   │   ├── 5279296e620fad6c6839263c279ff23b4be8df32.nq.gz
│   │   ├── 59eeae66e926a7c6c1b6fd1a6d8fbe31719ab1c3.nq.gz
│   │   ├── 5bf788f0eb0fc771f5c4eed8f282c7ec256565d2.nq.gz
│   │   ├── 5e33d430f13622c8363fe74d97963ab37f3df3c2.nq.gz
│   │   ├── 5ee093b37cb410a462bdeec4ade365298d82bd30.nq.gz
│   │   ├── 5f142a884ed52790a38b8e34df7060a0c3c6c760.nq.gz
│   │   ├── 65ec8d132c37a8338a2f495fa1be9f14bd4368d9.nq.gz
│   │   ├── 695820ae9bf6b3867f3634bc0776681a7ddf9dd7.nq.gz
│   │   ├── 71043a9c8fb6436a63110179650e32bcae4a6cbf.nq.gz
│   │   ├── 73b7bcdcaa663dd9d74a9fcadea0ce3ec1761f2f.nq.gz
│   │   ├── 7983c1ae9c2276b94cd85217f7aa58bb248847c4.nq.gz
│   │   ├── 7dc027d5fb980c7bd52ab4611f3109a796cec974.nq.gz
│   │   ├── 83986d822686739dc033495494ebdc88c4e266e8.nq.gz
│   │   ├── 892c7888ec613c49dd5ff826c58acc6c7e349955.nq.gz
│   │   ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf.nq.gz
│   │   ├── 8efa41c7da41f26c893204ff3fd65c0d06aa74ce.nq.gz
│   │   ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2.nq.gz
│   │   ├── 99fafb3c3b15e32dbaa504993161cb0c6898227f.nq.gz
│   │   ├── 9a6b3a8249df6e38f3683c457df8297fb1319d80.nq.gz
│   │   ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c.nq.gz
│   │   ├── a05ae6426cc8f224f4f1a995f46a901ab0f5644b.nq.gz
│   │   ├── a50051308509600388ed170fdedacfb673757de4.nq.gz
│   │   ├── a50753268a9033dcdc57d6dee45f3829cdedf8f0.nq.gz
│   │   ├── b06cc6376dfc566637a79607d5755d9519b3d6c6.nq.gz
│   │   ├── b52f3f97842dfa59cbef2e1e6f6606d8ea21e4c2.nq.gz
│   │   ├── b6b783bb8d2148355b644ab5d143e94a958e511d.nq.gz
│   │   ├── bd552df8f95716d53eb6fdea80b8d6d34cbc1968.nq.gz
│   │   ├── bdf95fd3e71f5f904dc6f7f1194a5fe23d1c3f2f.nq.gz
│   │   ├── bf04afb292fd8704f8b5f24ae113ba74eab3c2e4.nq.gz
│   │   ├── bf8f52bec7af4cf391dcabade49213213c5ac84b.nq.gz
│   │   ├── c4591651e2488e7ec303dffe387345ca22b940c6.nq.gz
│   │   ├── ca24e1b52ca21e2dbe9c94824e042524fc06b831.nq.gz
│   │   ├── ccd1aae48e49dd8c9365600fd79e886efe88be1d.nq.gz
│   │   ├── cd18c3b14aa810a4a6ebb264b9a297d6f8afb9ac.nq.gz
│   │   ├── daecb45327702efe8f702f46fb0870c2d6357837.nq.gz
│   │   ├── e659cf5d87c2aaf9ca8863625be436d7694471a4.nq.gz
│   │   ├── e674b96c4f9e20c2f6501b0c9e292d386931f9d0.nq.gz
│   │   ├── edb54c43c0321c0b41eee1473f3f4cf145e8927f.nq.gz
│   │   ├── f3040fba6a9c628c95fd510bcd9714367a0f4f4e.nq.gz
│   │   ├── f39933c8501dd6bc2e8e0f5be45819d3ba2caad0.nq.gz
│   │   ├── f73b8beeb1499ca5fcec3067cf89dad5326a0984.nq.gz
│   │   ├── fe3910083e3990695bc19c2ef671dd447262ae18.nq.gz
│   │   ├── fe85206c5c79be52910ff1b7049591adbab72e4d.nq.gz
│   │   └── ff54b029b15adc5259cfbbfa2749778179c48d37.nq.gz
│   └── repolex
│       ├── 02bed6f8c38e74f684bb0e572977a9bfdc1f6fea
│       │   └── chunk-001.nq.gz
│       ├── 0e3b18c39959ad4ec8bfe6cb7e11c82664aaa702
│       │   └── chunk-001.nq.gz
│       ├── 11d28e208504436e7e06603a941c01b76f54346f
│       │   └── chunk-001.nq.gz
│       ├── 137f88ea3224b8134fc58ed1243881642382d31b
│       │   └── chunk-001.nq.gz
│       ├── 1c20f546574cc905a8b28a5390c3f815e27a84ab
│       │   └── chunk-001.nq.gz
│       ├── 1dfb0bd885bbb0c466c19eee8bb2001bed59ca8c
│       │   └── chunk-001.nq.gz
│       ├── 2f22bca659cdcaea6ed37e5c9aa128bf99150eb6
│       │   └── chunk-001.nq.gz
│       ├── 3850ad6520cafb290bd4174fa9c4ca5d33440c82
│       │   └── chunk-001.nq.gz
│       ├── 4098bcac97aa0fbda2f4e73278fbbe3b128be940
│       │   └── chunk-001.nq.gz
│       ├── 41e339dd953a00d071c8bb5704f4671564f9f6e1
│       │   └── chunk-001.nq.gz
│       ├── 448be75222093041561d136f9f2f5577d6e361ee
│       │   └── chunk-001.nq.gz
│       ├── 44a3071654d6bfb4449da46aa885769820c4f0da
│       │   └── chunk-001.nq.gz
│       ├── 4adff7b5f85d388904e5ec53bf76334d773331b1
│       │   └── chunk-001.nq.gz
│       ├── 4f40b8495772eb3a1ab3613ffd7be5156f8e1389
│       │   └── chunk-001.nq.gz
│       ├── 5279296e620fad6c6839263c279ff23b4be8df32
│       │   └── chunk-001.nq.gz
│       ├── 59eeae66e926a7c6c1b6fd1a6d8fbe31719ab1c3
│       │   └── chunk-001.nq.gz
│       ├── 5bf788f0eb0fc771f5c4eed8f282c7ec256565d2
│       │   └── chunk-001.nq.gz
│       ├── 5e33d430f13622c8363fe74d97963ab37f3df3c2
│       │   └── chunk-001.nq.gz
│       ├── 5ee093b37cb410a462bdeec4ade365298d82bd30
│       │   └── chunk-001.nq.gz
│       ├── 5f142a884ed52790a38b8e34df7060a0c3c6c760
│       │   └── chunk-001.nq.gz
│       ├── 65ec8d132c37a8338a2f495fa1be9f14bd4368d9
│       │   └── chunk-001.nq.gz
│       ├── 695820ae9bf6b3867f3634bc0776681a7ddf9dd7
│       │   └── chunk-001.nq.gz
│       ├── 71043a9c8fb6436a63110179650e32bcae4a6cbf
│       │   └── chunk-001.nq.gz
│       ├── 73b7bcdcaa663dd9d74a9fcadea0ce3ec1761f2f
│       │   └── chunk-001.nq.gz
│       ├── 7983c1ae9c2276b94cd85217f7aa58bb248847c4
│       │   └── chunk-001.nq.gz
│       ├── 7dc027d5fb980c7bd52ab4611f3109a796cec974
│       │   └── chunk-001.nq.gz
│       ├── 83986d822686739dc033495494ebdc88c4e266e8
│       │   └── chunk-001.nq.gz
│       ├── 892c7888ec613c49dd5ff826c58acc6c7e349955
│       │   └── chunk-001.nq.gz
│       ├── 8d397c73191b49c6d5280098d7c09dbe474e00bf
│       │   └── chunk-001.nq.gz
│       ├── 8efa41c7da41f26c893204ff3fd65c0d06aa74ce
│       │   └── chunk-001.nq.gz
│       ├── 9283c0f15cfa82307f57daba4d1b1880902adfb2
│       │   └── chunk-001.nq.gz
│       ├── 99fafb3c3b15e32dbaa504993161cb0c6898227f
│       │   └── chunk-001.nq.gz
│       ├── 9a6b3a8249df6e38f3683c457df8297fb1319d80
│       │   └── chunk-001.nq.gz
│       ├── 9ff60042a53cd1bbfd5580ab0a91ea2d1d8f2f8c
│       │   └── chunk-001.nq.gz
│       ├── a05ae6426cc8f224f4f1a995f46a901ab0f5644b
│       │   └── chunk-001.nq.gz
│       ├── a50051308509600388ed170fdedacfb673757de4
│       │   └── chunk-001.nq.gz
│       ├── a50753268a9033dcdc57d6dee45f3829cdedf8f0
│       │   └── chunk-001.nq.gz
│       ├── b06cc6376dfc566637a79607d5755d9519b3d6c6
│       │   └── chunk-001.nq.gz
│       ├── b52f3f97842dfa59cbef2e1e6f6606d8ea21e4c2
│       │   └── chunk-001.nq.gz
│       ├── b6b783bb8d2148355b644ab5d143e94a958e511d
│       │   └── chunk-001.nq.gz
│       ├── bd552df8f95716d53eb6fdea80b8d6d34cbc1968
│       │   └── chunk-001.nq.gz
│       ├── bdf95fd3e71f5f904dc6f7f1194a5fe23d1c3f2f
│       │   └── chunk-001.nq.gz
│       ├── bf04afb292fd8704f8b5f24ae113ba74eab3c2e4
│       │   └── chunk-001.nq.gz
│       ├── bf8f52bec7af4cf391dcabade49213213c5ac84b
│       │   └── chunk-001.nq.gz
│       ├── c4591651e2488e7ec303dffe387345ca22b940c6
│       │   └── chunk-001.nq.gz
│       ├── ca24e1b52ca21e2dbe9c94824e042524fc06b831
│       │   └── chunk-001.nq.gz
│       ├── ccd1aae48e49dd8c9365600fd79e886efe88be1d
│       │   └── chunk-001.nq.gz
│       ├── cd18c3b14aa810a4a6ebb264b9a297d6f8afb9ac
│       │   └── chunk-001.nq.gz
│       ├── daecb45327702efe8f702f46fb0870c2d6357837
│       │   └── chunk-001.nq.gz
│       ├── e659cf5d87c2aaf9ca8863625be436d7694471a4
│       │   └── chunk-001.nq.gz
│       ├── e674b96c4f9e20c2f6501b0c9e292d386931f9d0
│       │   └── chunk-001.nq.gz
│       ├── edb54c43c0321c0b41eee1473f3f4cf145e8927f
│       │   └── chunk-001.nq.gz
│       ├── f3040fba6a9c628c95fd510bcd9714367a0f4f4e
│       │   └── chunk-001.nq.gz
│       ├── f39933c8501dd6bc2e8e0f5be45819d3ba2caad0
│       │   └── chunk-001.nq.gz
│       ├── f73b8beeb1499ca5fcec3067cf89dad5326a0984
│       │   └── chunk-001.nq.gz
│       ├── fe3910083e3990695bc19c2ef671dd447262ae18
│       │   └── chunk-001.nq.gz
│       ├── fe85206c5c79be52910ff1b7049591adbab72e4d
│       │   └── chunk-001.nq.gz
│       └── ff54b029b15adc5259cfbbfa2749778179c48d37
│           └── chunk-001.nq.gz
└── blob
    ├── 001c08df7cebe63fcbb0edafe57b641f040e8160.nq.gz
    ├── 00dab39b6a23e9d85b82af733900443390fd8c6e.nq.gz
    ├── 00f1fb720756628fb1daf30cab68624a598e09a6.nq.gz
    ├── 01605585857053e5292cf008698adc9c9d8c283b.nq.gz
    ├── 0165256254142b24c49d29e346eb97de1cae40de.nq.gz
    ├── 0174bcce6d48de946214d59bcae5543d38d89c3a.nq.gz
    ├── 017ae769f81a89149b92c97ee3c0c3af6a2bd408.nq.gz
    ├── 02544382040cd438717a91d57820bfb6a45f80a0.nq.gz
    ├── 026016c77302e28b2d5e2333c1b5b45775f8e6e0.nq.gz
    ├── 027e6cc283d7dfc311d1901613cdf430344eef79.nq.gz
    ├── 02f455d8eefd53ef88da5424315589610bf7edd7.nq.gz
    ├── 03023639477c1b37b44be5b1820d92db69a8ddd2.nq.gz
    ├── 039b554df7304f7987536637e11466f0c4cc8b36.nq.gz
    ├── 0402b0bf5e4365b7896bf316c72fb788366190c5.nq.gz
    ├── 0492cc33e934a75b14a2f1765c5a208785e2b48e.nq.gz
    ├── 04b997ffeb10729c3ccf9f79b1f9873f3265a2a0.nq.gz
    ├── 04bfb41cf2e4c9dec01953d749e355370d99fbb0.nq.gz
    ├── 04c13b5fac46571c8784f748b76b76346430335c.nq.gz
    ├── 04d41bad9cc5f7e62f221af9d9408f047f7e32f7.nq.gz
    ├── 04d51dfdb976ec5e24a85a279dd2034a6475ae20.nq.gz
    ├── 05ee166af38f217d520eb15bcab6264a0c74390a.nq.gz
    ├── 061805b6c31f8b086c64e3e2a9339f058c09169e.nq.gz
    ├── 069d63923ec8b95bbbb5fef3b5dc3bd92a8781bd.nq.gz
    ├── 06fdf295eeb6ae0a513f145077bf57c3bde3a9a3.nq.gz
    ├── 072dec942d7c1358b1d78787b0451ff020955b98.nq.gz
    └── 074c01d0339a46835196be6e8a9672b8b103e7f5.nq.gz

122 directories, 200 files
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
*Parsed on 2026-09-21 by [repolex](https://repolex.ai)*
