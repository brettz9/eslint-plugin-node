# Changelog

## [18.0.0](https://github.com/brettz9/eslint-plugin-node/compare/v17.9.0...v18.0.0) (2024-07-24)


### ⚠ BREAKING CHANGES

* prefer-node-prefix: pass moduleName ([#203](https://github.com/brettz9/eslint-plugin-node/issues/203))
* rename rule shebang => hashbang, deprecate rule shebang ([#198](https://github.com/brettz9/eslint-plugin-node/issues/198))
* remove "n/no-unsupported-features" #140 ([#173](https://github.com/brettz9/eslint-plugin-node/issues/173))
* Start using `enhanced-resolve` to improve ts support ([#139](https://github.com/brettz9/eslint-plugin-node/issues/139))
* drop eslint v7 & node.js < 18 ([#161](https://github.com/brettz9/eslint-plugin-node/issues/161))
* update default `ecmaVersion` to 2021 ([#96](https://github.com/brettz9/eslint-plugin-node/issues/96))
* engines.node defaults to 16.0.0 ([#91](https://github.com/brettz9/eslint-plugin-node/issues/91))
* drop node.js < 16 ([#90](https://github.com/brettz9/eslint-plugin-node/issues/90))
* add support for Node.js ESM resolution ([#4](https://github.com/brettz9/eslint-plugin-node/issues/4))
* support eslint v8 ([#1](https://github.com/brettz9/eslint-plugin-node/issues/1))

### 🌟 Features

* add `name` to flat configs ([#224](https://github.com/brettz9/eslint-plugin-node/issues/224)) ([24512a0](https://github.com/brettz9/eslint-plugin-node/commit/24512a0fe27bcb9b2a0ed20cd83bcbd3c0060d0b))
* Add builtins check for ES2021 to no-unsupported-features/es-builtins rule ([#153](https://github.com/brettz9/eslint-plugin-node/issues/153)) ([15a5850](https://github.com/brettz9/eslint-plugin-node/commit/15a5850138bffb64c1e2134ac9f2eacd2c04d219))
* add config `flat/recommended` and `flat/mixed-esm-and-cjs` ([#111](https://github.com/brettz9/eslint-plugin-node/issues/111)) ([78595c4](https://github.com/brettz9/eslint-plugin-node/commit/78595c42642349c5f5bb2e0ae9986da9ae93fed8))
* Add flag ignorePrivate to no-unpublished-x rules ([#298](https://github.com/brettz9/eslint-plugin-node/issues/298)) ([0609431](https://github.com/brettz9/eslint-plugin-node/commit/0609431dabcd9402720071025c0206d2686e1d78))
* Add n/prefer-node-protocol rule ([#183](https://github.com/brettz9/eslint-plugin-node/issues/183)) ([88d1c37](https://github.com/brettz9/eslint-plugin-node/commit/88d1c377cb6ba3aa4fe744e130bbb81117dbecb3))
* Add support for ignoring experemental features ([#269](https://github.com/brettz9/eslint-plugin-node/issues/269)) ([c046376](https://github.com/brettz9/eslint-plugin-node/commit/c046376fb52bef8104502ffab3c457412d1a1e27))
* add support for Node.js ESM resolution ([#4](https://github.com/brettz9/eslint-plugin-node/issues/4)) ([d24be36](https://github.com/brettz9/eslint-plugin-node/commit/d24be36e7a2ee405b268cd057f92b31558525233))
* Add syntax check for ES2021 to no-unsupported-features/es-syntax rule ([#152](https://github.com/brettz9/eslint-plugin-node/issues/152)) ([6835a10](https://github.com/brettz9/eslint-plugin-node/commit/6835a1055a785f0b394de37d1a1aa7c8686f15a9))
* add the ability to configure typescript to javascript file extension conversion ([#112](https://github.com/brettz9/eslint-plugin-node/issues/112)) ([20d2713](https://github.com/brettz9/eslint-plugin-node/commit/20d2713de7054b823ab29f40925ba782123208c3))
* add version as a setting ([#70](https://github.com/brettz9/eslint-plugin-node/issues/70)) ([273b937](https://github.com/brettz9/eslint-plugin-node/commit/273b937730e7513b327e3497a8c412c80bd3853c))
* Added supported version for module imports(13.2.0) ([#52](https://github.com/brettz9/eslint-plugin-node/issues/52)) ([98b873a](https://github.com/brettz9/eslint-plugin-node/commit/98b873a571d98462b28bec444570147dba743d26))
* Allow dynamic import for Node.js &gt;=12.17 &lt;13 || >=13.2 ([#13](https://github.com/brettz9/eslint-plugin-node/issues/13)) ([caccbef](https://github.com/brettz9/eslint-plugin-node/commit/caccbef9d1e802d52e1089bd49dd331ca465672d))
* Allow for automatic ts mapping detection ([#114](https://github.com/brettz9/eslint-plugin-node/issues/114)) ([2ab30ce](https://github.com/brettz9/eslint-plugin-node/commit/2ab30ce5b6ff424c6d7f217f35c07375e9fdd925))
* detect non-member expressions in n/no-sync ([#127](https://github.com/brettz9/eslint-plugin-node/issues/127)) ([6d02512](https://github.com/brettz9/eslint-plugin-node/commit/6d02512d9f68e7cd06f27bc51de673c4e9f91496))
* Disable the `no-unpublished-x` rules in private packages ([#57](https://github.com/brettz9/eslint-plugin-node/issues/57)) ([5ccd0c5](https://github.com/brettz9/eslint-plugin-node/commit/5ccd0c5a55d5e6dc61a82d81dd63ae317535fa97))
* drop eslint v7 & node.js &lt; 18 ([#161](https://github.com/brettz9/eslint-plugin-node/issues/161)) ([41ceed7](https://github.com/brettz9/eslint-plugin-node/commit/41ceed7ad17e42f3074e664081f69639d0fb4322))
* drop node.js &lt; 16 ([#90](https://github.com/brettz9/eslint-plugin-node/issues/90)) ([38a67ef](https://github.com/brettz9/eslint-plugin-node/commit/38a67ef182091faa846cfd0836653741403c4e4d)), closes [#42](https://github.com/brettz9/eslint-plugin-node/issues/42)
* engines.node defaults to 16.0.0 ([#91](https://github.com/brettz9/eslint-plugin-node/issues/91)) ([075f0c5](https://github.com/brettz9/eslint-plugin-node/commit/075f0c5170a0a2ae797b04c1725ebf360b10b678))
* eslint v9.0.0 compatibility (fixes [#143](https://github.com/brettz9/eslint-plugin-node/issues/143)) ([#144](https://github.com/brettz9/eslint-plugin-node/issues/144)) ([b075568](https://github.com/brettz9/eslint-plugin-node/commit/b075568b34b45454d655ab1fc91f164a6b59f1b4))
* export flat/recommended-script and flat/recommended-module ([#113](https://github.com/brettz9/eslint-plugin-node/issues/113)) ([1f8fdc8](https://github.com/brettz9/eslint-plugin-node/commit/1f8fdc88a7d36603bf8571d11a407290e4106327))
* Export the moduleType from ImportTarget ([#132](https://github.com/brettz9/eslint-plugin-node/issues/132)) ([ff01930](https://github.com/brettz9/eslint-plugin-node/commit/ff019309acf0078ba827769bdb4a6bf58becfbb4))
* export-style fixable ([#17](https://github.com/brettz9/eslint-plugin-node/issues/17)) ([7e2bf41](https://github.com/brettz9/eslint-plugin-node/commit/7e2bf41f44dd0f1744b20547997cb5ef54dea0d5))
* **hashbang:** Add support to map extensions to executables ([#278](https://github.com/brettz9/eslint-plugin-node/issues/278)) ([3fd7639](https://github.com/brettz9/eslint-plugin-node/commit/3fd7639e4d98d2cd936682197ef4004d59adadfd))
* **import-target:** Add resolution error reason ([ed7b25c](https://github.com/brettz9/eslint-plugin-node/commit/ed7b25cf4ccb3f27bf89993a7fc8c706e3491ad5))
* **import-target:** Add resolution error reason ([#264](https://github.com/brettz9/eslint-plugin-node/issues/264)) ([982a723](https://github.com/brettz9/eslint-plugin-node/commit/982a723dfb81dc141b093e27b41cd67f82ba8587))
* More es-syntax deprecations ([#249](https://github.com/brettz9/eslint-plugin-node/issues/249)) ([2ecee79](https://github.com/brettz9/eslint-plugin-node/commit/2ecee796c53733c70ea671a1e029aed9cf06d050))
* no-deprecated-api support removed api ([#240](https://github.com/brettz9/eslint-plugin-node/issues/240)) ([36fd35d](https://github.com/brettz9/eslint-plugin-node/commit/36fd35d9bbbaec43dd911e06bd83625cd1650fb3))
* **no-missing-imports:** add `tryExtensions` option ([#228](https://github.com/brettz9/eslint-plugin-node/issues/228)) ([ae5329c](https://github.com/brettz9/eslint-plugin-node/commit/ae5329c06b38da1220a352d4d268cfa8038c0d00))
* no-unpublished-import supports ignoreTypeImport (fixes [#78](https://github.com/brettz9/eslint-plugin-node/issues/78)) ([#79](https://github.com/brettz9/eslint-plugin-node/issues/79)) ([1fc0bf6](https://github.com/brettz9/eslint-plugin-node/commit/1fc0bf6fd0ff8e91b28698ec3d00d1a181d1bf4d))
* no-unsupported-features support process.report ([#60](https://github.com/brettz9/eslint-plugin-node/issues/60)) ([8ce1a64](https://github.com/brettz9/eslint-plugin-node/commit/8ce1a64c83b74c1823c32f88774c90c7df6d5039))
* **no-unsupported-features:** ✨ Update to node v20.12.0/v21.7.0 ([#229](https://github.com/brettz9/eslint-plugin-node/issues/229)) ([a8d0539](https://github.com/brettz9/eslint-plugin-node/commit/a8d0539ae99697f0e3441625c61e2e6ed7a10b9a))
* **no-unsupported-features:** Update to v21.6.1 of node ([#180](https://github.com/brettz9/eslint-plugin-node/issues/180)) ([d24f645](https://github.com/brettz9/eslint-plugin-node/commit/d24f645d14beacb2d7c89af2997edf5c2c91421f))
* node builtins ([ecdf019](https://github.com/brettz9/eslint-plugin-node/commit/ecdf019c54c5bd720c20d2ea21886559c15f3205))
* **node-builtin:** Add node 20.13.0, 22.0.0, and 22.1.0 support ([#276](https://github.com/brettz9/eslint-plugin-node/issues/276)) ([4a685c0](https://github.com/brettz9/eslint-plugin-node/commit/4a685c05e2d5770e22c46dcb78267fa8c484f725))
* **node-builtin:** Add node 22.2.0 support ([#282](https://github.com/brettz9/eslint-plugin-node/issues/282)) ([5221c40](https://github.com/brettz9/eslint-plugin-node/commit/5221c4015fb939cfb33231b7b6f4669cf1197ef7))
* **node-builtins:** Add node globals ([#261](https://github.com/brettz9/eslint-plugin-node/issues/261)) ([9466731](https://github.com/brettz9/eslint-plugin-node/commit/946673149b51b84581f91890495c810a496e0022))
* prefer-node-prefix: pass moduleName ([#203](https://github.com/brettz9/eslint-plugin-node/issues/203)) ([38985ca](https://github.com/brettz9/eslint-plugin-node/commit/38985ca63537cc56ae2476457ec7d5e433bf0a2f))
* remove "is-builtin-module" dependency (fixes [#232](https://github.com/brettz9/eslint-plugin-node/issues/232)) ([#227](https://github.com/brettz9/eslint-plugin-node/issues/227)) ([03619ee](https://github.com/brettz9/eslint-plugin-node/commit/03619eed4d24cb8ed79c467fe4a620bd58fea4cd))
* rename rule shebang =&gt; hashbang, deprecate rule shebang ([#198](https://github.com/brettz9/eslint-plugin-node/issues/198)) ([cefdb1c](https://github.com/brettz9/eslint-plugin-node/commit/cefdb1c26d856b544470e825daef2dfa5d0e4a30)), closes [#196](https://github.com/brettz9/eslint-plugin-node/issues/196)
* **shebang:** Add options to ignore unpublished files ([#172](https://github.com/brettz9/eslint-plugin-node/issues/172)) ([5609abb](https://github.com/brettz9/eslint-plugin-node/commit/5609abb0420554a955e1ca004eabf11ea4383657))
* **shebang:** add support for env's split-string option ([#195](https://github.com/brettz9/eslint-plugin-node/issues/195)) ([b383b49](https://github.com/brettz9/eslint-plugin-node/commit/b383b4971df4f4b67099655797b654b36d6a8fdf))
* Start using `enhanced-resolve` to improve ts support ([#139](https://github.com/brettz9/eslint-plugin-node/issues/139)) ([dc9f473](https://github.com/brettz9/eslint-plugin-node/commit/dc9f4731907a6408b2971e6ee833eba4c5c16adf))
* support eslint v8 ([#1](https://github.com/brettz9/eslint-plugin-node/issues/1)) ([3ea88d1](https://github.com/brettz9/eslint-plugin-node/commit/3ea88d16c67436d5052627b9a936fc8df42bd829))
* support eslint.config.js ([#95](https://github.com/brettz9/eslint-plugin-node/issues/95)) ([ebc97bf](https://github.com/brettz9/eslint-plugin-node/commit/ebc97bf337c004963d2f3faf1fe98cc386c4f1a6))
* supported new globals added in the new node.js versions ([#154](https://github.com/brettz9/eslint-plugin-node/issues/154)) ([7628925](https://github.com/brettz9/eslint-plugin-node/commit/762892590a0bb5fdc0704e6dd34923e3991ae744))
* typescript (jsdoc) checking and definition generation ([#169](https://github.com/brettz9/eslint-plugin-node/issues/169)) ([6d8ed14](https://github.com/brettz9/eslint-plugin-node/commit/6d8ed14c186a814c3a258993fb6c986a02ed5568))
* update default `ecmaVersion` to 2021 ([#96](https://github.com/brettz9/eslint-plugin-node/issues/96)) ([49d3ee7](https://github.com/brettz9/eslint-plugin-node/commit/49d3ee780c57be2eabdb577d892e2f2430ec3888))
* Update ES Syntax ([#189](https://github.com/brettz9/eslint-plugin-node/issues/189)) ([4778ae8](https://github.com/brettz9/eslint-plugin-node/commit/4778ae86c398f90da13248c2d31bfc4a83cd2dea))
* Update es-builtins ([#174](https://github.com/brettz9/eslint-plugin-node/issues/174)) ([fbc9e7b](https://github.com/brettz9/eslint-plugin-node/commit/fbc9e7bfb6a4b805f83c1ac1c103394910ca9892))
* Update to node v22.4.0 ([#310](https://github.com/brettz9/eslint-plugin-node/issues/310)) ([f7a74eb](https://github.com/brettz9/eslint-plugin-node/commit/f7a74eb147875d7e2125125863befe61d0be0614)), closes [#308](https://github.com/brettz9/eslint-plugin-node/issues/308)
* Update to node v22.5.0 ([#312](https://github.com/brettz9/eslint-plugin-node/issues/312)) ([2539c9d](https://github.com/brettz9/eslint-plugin-node/commit/2539c9deaa0c339b520dcd45ba4998dca6b678e3))
* upgrade deps to latest ([#93](https://github.com/brettz9/eslint-plugin-node/issues/93)) ([aa75610](https://github.com/brettz9/eslint-plugin-node/commit/aa75610d38c7a43135636248bb93c05ea7ebb7aa))


### 🩹 Fixes

* `no-deprecated-api` crash on undeclared assignment (fixes [#55](https://github.com/brettz9/eslint-plugin-node/issues/55)) ([#56](https://github.com/brettz9/eslint-plugin-node/issues/56)) ([610b905](https://github.com/brettz9/eslint-plugin-node/commit/610b9052e7d7013101f1c2a09574f2949ffde8ef))
* `no-deprecated-api` has false positive on Mac/Linux. ([1bc22af](https://github.com/brettz9/eslint-plugin-node/commit/1bc22af34d7fbe6ff7cd94a67c3984f01236588b))
* `no-unsupported-features` crash if only `ignores` option ([8275cfc](https://github.com/brettz9/eslint-plugin-node/commit/8275cfc9ce85cce951d9d94a6fe618bd7403f7b7))
* `no-unsupported-features` goes wrong on `&gt;=7.10.0` (fixes [#78](https://github.com/brettz9/eslint-plugin-node/issues/78)) ([deb4f55](https://github.com/brettz9/eslint-plugin-node/commit/deb4f55ac99082c8b74121c9f6bb1474c9003177))
* `no-unsupported-features` has false positive (fixes [#59](https://github.com/brettz9/eslint-plugin-node/issues/59)) ([143f509](https://github.com/brettz9/eslint-plugin-node/commit/143f50906034dbf64232d5aa574fe26eb5cbe019))
* `shebang` should allow CLI flags (fixes [#51](https://github.com/brettz9/eslint-plugin-node/issues/51)) ([e42d161](https://github.com/brettz9/eslint-plugin-node/commit/e42d161072a8c08d56c5fc5d7f69d402fbf10104))
* `stream/promises` is stable ([02a264e](https://github.com/brettz9/eslint-plugin-node/commit/02a264e0acb7ba913500e195fe0a2a6aaae74c6e))
* Add proper file extensions when importing a typescript file from a typescript file ([#20](https://github.com/brettz9/eslint-plugin-node/issues/20)) ([c8d0484](https://github.com/brettz9/eslint-plugin-node/commit/c8d048477897af19828b44904edc0ea4367d8296))
* Add supported version to Buffer constructor ([#266](https://github.com/brettz9/eslint-plugin-node/issues/266)) ([030f51b](https://github.com/brettz9/eslint-plugin-node/commit/030f51bacd21918ef6d5b2bba9ec77cd701c3eba))
* Allow for misconfigured default exports ([#288](https://github.com/brettz9/eslint-plugin-node/issues/288)) ([92e18b5](https://github.com/brettz9/eslint-plugin-node/commit/92e18b572f7bd2427f050eab8484cb393e1dac7a))
* Allow imports of self-referenced package ([#74](https://github.com/brettz9/eslint-plugin-node/issues/74)) ([17270f8](https://github.com/brettz9/eslint-plugin-node/commit/17270f8e9d76c10e57041c7a2bed0d9a7a9c4638))
* allow settings.n (fixes [#3](https://github.com/brettz9/eslint-plugin-node/issues/3)) ([769cce9](https://github.com/brettz9/eslint-plugin-node/commit/769cce9c3b1c9c777cf7627b430e6e73e4ec01b6))
* change peer dependencies to allow eslint v9 ([#216](https://github.com/brettz9/eslint-plugin-node/issues/216)) ([5e82d7f](https://github.com/brettz9/eslint-plugin-node/commit/5e82d7f26aa8dc58b46584c9fe3c74a11c265228))
* Change to using is-builtin-module ([#138](https://github.com/brettz9/eslint-plugin-node/issues/138)) ([2846f4f](https://github.com/brettz9/eslint-plugin-node/commit/2846f4f6a7505b963a3000fb6d635a61ac604e2e))
* consider node: prefix in prefer-global rules ([#63](https://github.com/brettz9/eslint-plugin-node/issues/63)) ([dbb7264](https://github.com/brettz9/eslint-plugin-node/commit/dbb72642fdc0987fa915c5375c96275516f44529))
* default mapping of sourc .ts import of unspecified extension should be  .js ([#29](https://github.com/brettz9/eslint-plugin-node/issues/29)) ([3736fa9](https://github.com/brettz9/eslint-plugin-node/commit/3736fa9edb863573c76c875e59b0ceba8b9395af)), closes [#28](https://github.com/brettz9/eslint-plugin-node/issues/28)
* do not crash rule `no-unpublished-require` ([#49](https://github.com/brettz9/eslint-plugin-node/issues/49)) ([38b0298](https://github.com/brettz9/eslint-plugin-node/commit/38b0298b7414506222758e83be2d8d6441f0da48)), closes [#48](https://github.com/brettz9/eslint-plugin-node/issues/48)
* ensure "version" always has a valid value in parseOptions ([#109](https://github.com/brettz9/eslint-plugin-node/issues/109)) ([234703c](https://github.com/brettz9/eslint-plugin-node/commit/234703cc58d1d8ebfdf0be367d958bf6682b299f))
* ensure files exist with case sensitive (fixes [#68](https://github.com/brettz9/eslint-plugin-node/issues/68)) ([8be4d96](https://github.com/brettz9/eslint-plugin-node/commit/8be4d96c2ad991a78c11c1281d91a201d580e02c))
* Errors on Travis CI ([0da386a](https://github.com/brettz9/eslint-plugin-node/commit/0da386af3c680ac5f4fccc26335e91dc04c1bd5e))
* eslint 7.0 support ([#156](https://github.com/brettz9/eslint-plugin-node/issues/156)) ([2419888](https://github.com/brettz9/eslint-plugin-node/commit/241988828e30c2a32cc58982548dfce1cc56b87f))
* explicitly support ESLint 9.0.0 pre-releases ([#200](https://github.com/brettz9/eslint-plugin-node/issues/200)) ([a5eaa9c](https://github.com/brettz9/eslint-plugin-node/commit/a5eaa9c867bc2e87b1fa54920c85acd1e8f9f927))
* exported configs ([6d9b240](https://github.com/brettz9/eslint-plugin-node/commit/6d9b240e5218f5d2f5e77fc43a04dabf63bc8950))
* false positive 'no-unsupported-features/node-builtins' ([44b57ed](https://github.com/brettz9/eslint-plugin-node/commit/44b57edfb46e37e6a635d85c66d60ae6a66bb6c4))
* false positive of `no-unsupported-features` about code point escapes. ([292e8f8](https://github.com/brettz9/eslint-plugin-node/commit/292e8f8b210593ff0d0b3c36e9c3a98d04e46980))
* fix tests for linter.reset ([effdd10](https://github.com/brettz9/eslint-plugin-node/commit/effdd10468c5a81e36208a2ae63d1a1927a42ad2))
* hashbang + eslint v8 compat issue ([e82974f](https://github.com/brettz9/eslint-plugin-node/commit/e82974fc724e4a410f85459f4cd3e5367939cc9c))
* hashbang + eslint v8 compat issue ([#290](https://github.com/brettz9/eslint-plugin-node/issues/290)) ([e82974f](https://github.com/brettz9/eslint-plugin-node/commit/e82974fc724e4a410f85459f4cd3e5367939cc9c))
* improve the message of `no-deprecated-api` for `Buffer` ([d8142a1](https://github.com/brettz9/eslint-plugin-node/commit/d8142a1ae87124d140a6e5efb8069cf335b0ac5b))
* lint errors ([ac4cb6e](https://github.com/brettz9/eslint-plugin-node/commit/ac4cb6efde62b89d1c8ba15c412a3659acaae6c7))
* missing import recognise tsx extension ([#97](https://github.com/brettz9/eslint-plugin-node/issues/97)) ([5fae8a5](https://github.com/brettz9/eslint-plugin-node/commit/5fae8a5703f1338c5d86ba320081e49d620dfd87))
* modules support range ([#71](https://github.com/brettz9/eslint-plugin-node/issues/71)) ([79b7984](https://github.com/brettz9/eslint-plugin-node/commit/79b7984da43b6a82c191e0643efbbd77e2817e74))
* New Buffer APIs are available in 4.5.0 ([#64](https://github.com/brettz9/eslint-plugin-node/issues/64)) ([2991302](https://github.com/brettz9/eslint-plugin-node/commit/2991302d509d16f75c68518a6db3797ccd1e6be1))
* no-callback-literal ignore unknown nodes ([#163](https://github.com/brettz9/eslint-plugin-node/issues/163)) ([5449752](https://github.com/brettz9/eslint-plugin-node/commit/54497527e948830d9c1d176734c558c989ba5a50)), closes [#162](https://github.com/brettz9/eslint-plugin-node/issues/162)
* no-deprecated-api crash in self-assign (fixes [#87](https://github.com/brettz9/eslint-plugin-node/issues/87)) ([0295a7f](https://github.com/brettz9/eslint-plugin-node/commit/0295a7f6608be458f5a380108bdc1406137b0ebe))
* no-missing-import for typescript ([#24](https://github.com/brettz9/eslint-plugin-node/issues/24)) ([f65ca8b](https://github.com/brettz9/eslint-plugin-node/commit/f65ca8ba3b4d48846a767217aa52a776104164d6))
* no-missing-require had false positive (fixes [#70](https://github.com/brettz9/eslint-plugin-node/issues/70)) ([113c68f](https://github.com/brettz9/eslint-plugin-node/commit/113c68f5621c2f1f73ca7e97145e384fc7835ee4))
* **no-unsupported-features:** `stream/promises` is stable ([#235](https://github.com/brettz9/eslint-plugin-node/issues/235)) ([02a264e](https://github.com/brettz9/eslint-plugin-node/commit/02a264e0acb7ba913500e195fe0a2a6aaae74c6e)), closes [#234](https://github.com/brettz9/eslint-plugin-node/issues/234)
* **no-unsupported-features:** Remove use of `static` as a variable ([#190](https://github.com/brettz9/eslint-plugin-node/issues/190)) ([e31d868](https://github.com/brettz9/eslint-plugin-node/commit/e31d8683b65a6f982cb91634f951afd0fe5583ae))
* **node-builtins:** Remove "node:" prefix from "ignores" message ([#277](https://github.com/brettz9/eslint-plugin-node/issues/277)) ([704f0b9](https://github.com/brettz9/eslint-plugin-node/commit/704f0b9373542e03b42102d30bc44cb7e30fc5d8))
* Normalise `package.json#files` before checking ignores and whitelist ([#123](https://github.com/brettz9/eslint-plugin-node/issues/123)) (fixes [#122](https://github.com/brettz9/eslint-plugin-node/issues/122)) ([2d43f48](https://github.com/brettz9/eslint-plugin-node/commit/2d43f48eeb8c57f37e1ff4506d9c484e13c2f576))
* prefer-node-protocol: not first target ([#204](https://github.com/brettz9/eslint-plugin-node/issues/204)) ([caab777](https://github.com/brettz9/eslint-plugin-node/commit/caab77714ec9195c07290d4c212a95f11b48bb5f))
* **prefer-node-protocol:** continue on version range check ([#206](https://github.com/brettz9/eslint-plugin-node/issues/206)) ([14d2ea9](https://github.com/brettz9/eslint-plugin-node/commit/14d2ea90c1609b49e95cc805105711c62bf6fd50))
* range matching fails ([#31](https://github.com/brettz9/eslint-plugin-node/issues/31)) ([5a22112](https://github.com/brettz9/eslint-plugin-node/commit/5a22112bd7d9e152008f4be9c6d5655c55867c4f))
* README etc. are only assumed published if in pkg root (fixes [#73](https://github.com/brettz9/eslint-plugin-node/issues/73)) ([#74](https://github.com/brettz9/eslint-plugin-node/issues/74)) ([b2c6877](https://github.com/brettz9/eslint-plugin-node/commit/b2c68771449851c2a3473dddba387457a417e023))
* release-it config ([4c42a2c](https://github.com/brettz9/eslint-plugin-node/commit/4c42a2cb5a718e94e79e5bf0d2d8b6432194c879))
* remove `fs.existsSync` from `no-deprecated-api` (fixes [#52](https://github.com/brettz9/eslint-plugin-node/issues/52)) ([d849588](https://github.com/brettz9/eslint-plugin-node/commit/d8495887cb3247c7b54dde25489663db5d7face8))
* Remove `require("util")` import in import-target ([#181](https://github.com/brettz9/eslint-plugin-node/issues/181)) ([d32eff3](https://github.com/brettz9/eslint-plugin-node/commit/d32eff365bb8f98633ab4ae65875e8fbe61e6278))
* remove invalid es-builtins ([#258](https://github.com/brettz9/eslint-plugin-node/issues/258)) ([ecdf019](https://github.com/brettz9/eslint-plugin-node/commit/ecdf019c54c5bd720c20d2ea21886559c15f3205))
* revert minimatch to 3.1.2 ([44cec62](https://github.com/brettz9/eslint-plugin-node/commit/44cec62c4555c7855877cf8064bcf0d3338f4c95))
* support `node:` prefix ([#109](https://github.com/brettz9/eslint-plugin-node/issues/109)) ([fde2ba6](https://github.com/brettz9/eslint-plugin-node/commit/fde2ba6cc1aafcc7880a62b2684b68cd877154b6))
* support negative patterns in files field ([2aaa994](https://github.com/brettz9/eslint-plugin-node/commit/2aaa9943850f63348d2b194e79725c627a267ea7))
* tests for eslint@2 ([064f9b1](https://github.com/brettz9/eslint-plugin-node/commit/064f9b15a73f62310854aecc15b2b8c3aca73cca))
* third-party does not hide core modules ([4cc0e3f](https://github.com/brettz9/eslint-plugin-node/commit/4cc0e3fcc80e4b7e716043e4aba762bbe8001908))
* unsupported-features/node-builtins-modules range compare ([#252](https://github.com/brettz9/eslint-plugin-node/issues/252)) ([d50ae85](https://github.com/brettz9/eslint-plugin-node/commit/d50ae85c209a47a8a5d4c1bedaa94e6a77540095))
* unsupported-features/node-builtins-modules version comparation ([#257](https://github.com/brettz9/eslint-plugin-node/issues/257)) ([5c67787](https://github.com/brettz9/eslint-plugin-node/commit/5c67787cb191ff7409fa17ec5b12cfdc3a7a26d3))
* **unsupported-features:** Improve URL module ([#244](https://github.com/brettz9/eslint-plugin-node/issues/244)) ([6581979](https://github.com/brettz9/eslint-plugin-node/commit/6581979cfb6afa6a50531d37303af24aa7b4db37)), closes [#243](https://github.com/brettz9/eslint-plugin-node/issues/243)
* Update all dependencies.  Fix a few tests where eslint now reports nodeType: null. ([44cec62](https://github.com/brettz9/eslint-plugin-node/commit/44cec62c4555c7855877cf8064bcf0d3338f4c95))
* Updated `import-meta-resolve` & pack it automatically ([#87](https://github.com/brettz9/eslint-plugin-node/issues/87)) ([f74d35e](https://github.com/brettz9/eslint-plugin-node/commit/f74d35e1c62a45773eb5693379a5725842179a39))
* upgrade a few (dev)deps to latest ([b4ec37b](https://github.com/brettz9/eslint-plugin-node/commit/b4ec37b4e4266c8b36d7f581282a9a5a2a2c5e79))
* version number for tests. ([95b8164](https://github.com/brettz9/eslint-plugin-node/commit/95b816459980fac6cfa32acc3ae89c6ddb2d3bca))


### 📚 Documentation

* add clarifications to readme ([dbdfa8e](https://github.com/brettz9/eslint-plugin-node/commit/dbdfa8e0abdeb96f2f843c4112cc43f16f2657ea))
* add deprecated rules table (fixes [#129](https://github.com/brettz9/eslint-plugin-node/issues/129)) ([#130](https://github.com/brettz9/eslint-plugin-node/issues/130)) ([4467dcb](https://github.com/brettz9/eslint-plugin-node/commit/4467dcb9ccedf301f7f28b25b8681437a492f8ba))
* add issue templates ([#130](https://github.com/brettz9/eslint-plugin-node/issues/130)) ([2200c43](https://github.com/brettz9/eslint-plugin-node/commit/2200c433aaadf5547e5c7af7160088d2d1fe9f7e))
* add maintainance info ([#271](https://github.com/brettz9/eslint-plugin-node/issues/271)) ([b454488](https://github.com/brettz9/eslint-plugin-node/commit/b454488bd63c046d101305c40d24bf44ae83971e)), closes [#194](https://github.com/brettz9/eslint-plugin-node/issues/194)
* add playground (fixes [#25](https://github.com/brettz9/eslint-plugin-node/issues/25)) ([#145](https://github.com/brettz9/eslint-plugin-node/issues/145)) ([8bd6c7e](https://github.com/brettz9/eslint-plugin-node/commit/8bd6c7e590414fc36756cd035779025d479f6603))
* Add URL to rule documentation to the metadata ([#102](https://github.com/brettz9/eslint-plugin-node/issues/102)) ([27ac4a8](https://github.com/brettz9/eslint-plugin-node/commit/27ac4a834769cb2e26ac4a69aab823098366157f))
* add v17 changelog ([#223](https://github.com/brettz9/eslint-plugin-node/issues/223)) ([4fb36eb](https://github.com/brettz9/eslint-plugin-node/commit/4fb36eb253536b694d16b72d31221c98f1012f9f))
* auto-generate configs list with eslint-doc-generator ([6409e34](https://github.com/brettz9/eslint-plugin-node/commit/6409e34c8beb4242c575b4f53b9df0202898def4))
* Auto-generate configs list with eslint-doc-generator ([#146](https://github.com/brettz9/eslint-plugin-node/issues/146)) ([6409e34](https://github.com/brettz9/eslint-plugin-node/commit/6409e34c8beb4242c575b4f53b9df0202898def4))
* automate docs with eslint-doc-generator ([#61](https://github.com/brettz9/eslint-plugin-node/issues/61)) ([237b2a1](https://github.com/brettz9/eslint-plugin-node/commit/237b2a1f486eda527a6cb386ff08ca781cb00adf))
* change rule desc input to textarea in new-rule template ([446e744](https://github.com/brettz9/eslint-plugin-node/commit/446e7441ce85031761648a45100025f4e3d79b0c))
* cleanup docs, add markdownlint, tweak eslint-doc-generator options ([#64](https://github.com/brettz9/eslint-plugin-node/issues/64)) ([bdfd61a](https://github.com/brettz9/eslint-plugin-node/commit/bdfd61a0cba307175d3e171cc568f54a24de4269))
* Create a shared settings document ([#115](https://github.com/brettz9/eslint-plugin-node/issues/115)) ([7d855e6](https://github.com/brettz9/eslint-plugin-node/commit/7d855e65e31e447434f5863aa39d4279d31887a6))
* fix an accidental replacement. ([4cb5fd7](https://github.com/brettz9/eslint-plugin-node/commit/4cb5fd7c9bc5abab8e78bfab0d43bb08fa254607))
* fix comma JSON error on the first example ([#98](https://github.com/brettz9/eslint-plugin-node/issues/98)) ([d5a8985](https://github.com/brettz9/eslint-plugin-node/commit/d5a8985c0cdf8329d2e16013f0070bc437190a64))
* Fix grammatically incorrect `Additional ESLint's rules` ([#129](https://github.com/brettz9/eslint-plugin-node/issues/129)) ([fba650a](https://github.com/brettz9/eslint-plugin-node/commit/fba650aaea2b54abc60a43b370b9f5d9525f1047))
* Fix link ([#15](https://github.com/brettz9/eslint-plugin-node/issues/15)) ([e113f19](https://github.com/brettz9/eslint-plugin-node/commit/e113f195ecb87b4063fcdd1d29881808d799b8c4))
* fix repository URL:s, tweak badges + remove old non-working `codecov` ([#125](https://github.com/brettz9/eslint-plugin-node/issues/125)) ([5507f43](https://github.com/brettz9/eslint-plugin-node/commit/5507f4350cba36f28aa830674595063f43a1824f))
* fix ruleId in exports-style.md (fixes [#62](https://github.com/brettz9/eslint-plugin-node/issues/62)) ([7f37c7c](https://github.com/brettz9/eslint-plugin-node/commit/7f37c7c3131b28a0dfd0ca72def2d989682e1c04))
* fix spacings in the example ([#306](https://github.com/brettz9/eslint-plugin-node/issues/306)) ([c092cd8](https://github.com/brettz9/eslint-plugin-node/commit/c092cd893010f8da894f87da567c07d69be6cc0d))
* Fix spelling in no-callback-literal.md ([#135](https://github.com/brettz9/eslint-plugin-node/issues/135)) ([79c8afd](https://github.com/brettz9/eslint-plugin-node/commit/79c8afd4eb5e7b36e4ddf3aa6674898fdc9cb6c2))
* fix typo ([#154](https://github.com/brettz9/eslint-plugin-node/issues/154)) ([84b2646](https://github.com/brettz9/eslint-plugin-node/commit/84b2646e63e63d94c798bb75e6d95a32ca7151ce))
* fix url-search-params documentation ([#132](https://github.com/brettz9/eslint-plugin-node/issues/132)) ([51be232](https://github.com/brettz9/eslint-plugin-node/commit/51be232a7d60b181cda87c17b70e94b582538b55))
* improve wording of file-extension-in-import docs ([#110](https://github.com/brettz9/eslint-plugin-node/issues/110)) ([3f178ab](https://github.com/brettz9/eslint-plugin-node/commit/3f178abd04e1a0d1f4e1772a914497317ea85fcf))
* improve? ([f02bc9b](https://github.com/brettz9/eslint-plugin-node/commit/f02bc9b5788daea489d7e846f635bc6f87afb9d0))
* minor fix ([fd75f09](https://github.com/brettz9/eslint-plugin-node/commit/fd75f096bd88231478cfd13a893b0b20a69c5e79))
* **node-builtins:** Specify that only static properties are supported ([#272](https://github.com/brettz9/eslint-plugin-node/issues/272)) ([735a520](https://github.com/brettz9/eslint-plugin-node/commit/735a5207aee828e324835bdb0c7fa743347ef4b9))
* Provide an example with eslint-plugin-n to Playground ([#275](https://github.com/brettz9/eslint-plugin-node/issues/275)) ([cb8ffa6](https://github.com/brettz9/eslint-plugin-node/commit/cb8ffa62d07869dd23985f7d861ad3c60deec4f8))
* Remove text "Node does not support modules yet" ([#202](https://github.com/brettz9/eslint-plugin-node/issues/202)) ([5abca5b](https://github.com/brettz9/eslint-plugin-node/commit/5abca5bb6f1166045578ba7d51cda36b32cb333b))
* remove trailing comma from sample .eslintc.json in README ([#131](https://github.com/brettz9/eslint-plugin-node/issues/131)) ([ef0f103](https://github.com/brettz9/eslint-plugin-node/commit/ef0f1032d444d8c318995043e90e36228a2092c6))
* update description for recommended preset ([#114](https://github.com/brettz9/eslint-plugin-node/issues/114)) ([019ddd3](https://github.com/brettz9/eslint-plugin-node/commit/019ddd34ea918354200fe1752df2c6e81d05f221))
* update fork info ([fbede25](https://github.com/brettz9/eslint-plugin-node/commit/fbede253e983c5fe114b1ddf0f2ddff7779c50db))
* update pkgname in readme ([b129713](https://github.com/brettz9/eslint-plugin-node/commit/b129713edbd882ebf87d8fbce5a0bde84c422c9f))
* update README.md ([cde4c82](https://github.com/brettz9/eslint-plugin-node/commit/cde4c82503580d0cfd17e578e10b3c6f5883c776))
* update README.md ([a42d38e](https://github.com/brettz9/eslint-plugin-node/commit/a42d38ecafeefdc0df567f1994f2306bc5d7cf98))
* update README.md for deprecation rules ([a589060](https://github.com/brettz9/eslint-plugin-node/commit/a589060d98326631d2fafc912480b82de75a1d0d))
* update required node.js/eslint versions ([77ea5dc](https://github.com/brettz9/eslint-plugin-node/commit/77ea5dc975ca266501121ecb6b69febd2bba76ab))
* update ruleId in docs/rules/* ([26c90b1](https://github.com/brettz9/eslint-plugin-node/commit/26c90b1c13d882b2175eec58ccdfed7ae65862cf))
* Use link to tagged version for rule docs ([#104](https://github.com/brettz9/eslint-plugin-node/issues/104)) ([dc32ab5](https://github.com/brettz9/eslint-plugin-node/commit/dc32ab57cedf8566597dd7a9718084d4ed875542))


### 🧹 Chores

* `npm run format` ([#175](https://github.com/brettz9/eslint-plugin-node/issues/175)) ([17e658e](https://github.com/brettz9/eslint-plugin-node/commit/17e658e297996db3f432f171095136e61ab995cc))
* Add a .editorconfig file ([#126](https://github.com/brettz9/eslint-plugin-node/issues/126)) ([574df88](https://github.com/brettz9/eslint-plugin-node/commit/574df880a345e72885343454a41d05ddf7b6a9ab))
* add a test for [#109](https://github.com/brettz9/eslint-plugin-node/issues/109) ([9ccc91d](https://github.com/brettz9/eslint-plugin-node/commit/9ccc91debc86c5adbc8772e3180ed928aa53b989))
* add a test for self-ref ([#280](https://github.com/brettz9/eslint-plugin-node/issues/280)) ([4f50dfe](https://github.com/brettz9/eslint-plugin-node/commit/4f50dfe6528e32749aac315e53b351345cfc8c13))
* add cache to exists() ([fa95be2](https://github.com/brettz9/eslint-plugin-node/commit/fa95be2c73cc816912424b2d243b1a16b2adbcd5))
* add Node 7 to .travis.yml ([02a3ace](https://github.com/brettz9/eslint-plugin-node/commit/02a3ace5a2f936d334e2a97dab270a2e2de92655))
* add Node.js 8 to CI ([fdd7877](https://github.com/brettz9/eslint-plugin-node/commit/fdd7877687fe6608d131fefa52aefc88b542c416))
* add non-rule-change issue template ([#159](https://github.com/brettz9/eslint-plugin-node/issues/159)) ([c191101](https://github.com/brettz9/eslint-plugin-node/commit/c19110141717bd9772ba6410574a9b93d66094e8))
* add note about `require("punycode/")` (fixes [#72](https://github.com/brettz9/eslint-plugin-node/issues/72)) ([118a1de](https://github.com/brettz9/eslint-plugin-node/commit/118a1dea7c159ee366785b9e61dfb246350ad9ac))
* add prettier & lint-staged ([#7](https://github.com/brettz9/eslint-plugin-node/issues/7)) ([4deaca7](https://github.com/brettz9/eslint-plugin-node/commit/4deaca769e11289a309fd5ca4e4918ba19ac59b1))
* add release-it ([c2580a6](https://github.com/brettz9/eslint-plugin-node/commit/c2580a64dcac9e54a0659d27777ae878406763fc))
* add release-please ([#170](https://github.com/brettz9/eslint-plugin-node/issues/170)) ([fc77da2](https://github.com/brettz9/eslint-plugin-node/commit/fc77da2a0c3fc3720521f09bd6ca0aa196868ad2))
* apply eslint --fix ([3bce0e3](https://github.com/brettz9/eslint-plugin-node/commit/3bce0e344d2b314e12ddb504b38d2bfcf4d3e930))
* Configure Renovate ([0d6a0fe](https://github.com/brettz9/eslint-plugin-node/commit/0d6a0fe394508c5ef2fb7a0ff4cae6c8536a0182))
* do not run format in pretest ([ab87146](https://github.com/brettz9/eslint-plugin-node/commit/ab8714619c7aace70751a4d6771c645a379cf763))
* Enable global strict eslint rule ([#191](https://github.com/brettz9/eslint-plugin-node/issues/191)) ([99fe387](https://github.com/brettz9/eslint-plugin-node/commit/99fe38722d02de867f4bd8061a343b9754b62610))
* ESBuild externals (ESM to CJS bundle) ([#10](https://github.com/brettz9/eslint-plugin-node/issues/10)) ([e3e8c3f](https://github.com/brettz9/eslint-plugin-node/commit/e3e8c3f1fe55d0f88dd4cbe2b13fdcb50f75b231))
* extract reference tracking logic ([e957849](https://github.com/brettz9/eslint-plugin-node/commit/e957849ce0691794741fb793cab0e61090773340))
* fix a small misspelling. ([#95](https://github.com/brettz9/eslint-plugin-node/issues/95)) ([155f714](https://github.com/brettz9/eslint-plugin-node/commit/155f71400a83416e010faa617cfc16d2f8056f11))
* fix eslint &lt; v8 tests failing ([44cec62](https://github.com/brettz9/eslint-plugin-node/commit/44cec62c4555c7855877cf8064bcf0d3338f4c95))
* fix tests to follow moving files in eslint ([044ecce](https://github.com/brettz9/eslint-plugin-node/commit/044ecce462843e980cd4bbdf6aa3f4ca7d51887d))
* hide a complexity warning. ([16973f9](https://github.com/brettz9/eslint-plugin-node/commit/16973f98133fe4d406d29fd93dba9ef697e18cb5))
* improve auto-generation script ([cf36e6d](https://github.com/brettz9/eslint-plugin-node/commit/cf36e6d13d9cfcaf236c788e2f61faa017b1c39e))
* make defineUnsupportedModuleHandlers supporting globals ([f40be0e](https://github.com/brettz9/eslint-plugin-node/commit/f40be0e5842fad05ccbcbece8aaa8e5af1a8faa6))
* **master:** release 17.0.0-4 ([#176](https://github.com/brettz9/eslint-plugin-node/issues/176)) ([b7c6409](https://github.com/brettz9/eslint-plugin-node/commit/b7c6409f58e092a54898fabe30242bf1f956fa88))
* **master:** release 17.0.0-5 ([#201](https://github.com/brettz9/eslint-plugin-node/issues/201)) ([8327d11](https://github.com/brettz9/eslint-plugin-node/commit/8327d116c367fd3e137ab838c0b9bd38f17d4dfc))
* **master:** release 17.0.0-6 ([#205](https://github.com/brettz9/eslint-plugin-node/issues/205)) ([d96976d](https://github.com/brettz9/eslint-plugin-node/commit/d96976d5fa8780ad98c91f207cd67a79346e2c3d))
* **master:** release 17.0.0-7 ([#217](https://github.com/brettz9/eslint-plugin-node/issues/217)) ([438d6fa](https://github.com/brettz9/eslint-plugin-node/commit/438d6fae5f0c19c0ae4f396a0464a2c30bbba94e))
* **master:** release 17.0.0-8 ([#221](https://github.com/brettz9/eslint-plugin-node/issues/221)) ([aa580f4](https://github.com/brettz9/eslint-plugin-node/commit/aa580f4a7395639319d391548decc561d8a3757f))
* **master:** release 17.1.0 ([#225](https://github.com/brettz9/eslint-plugin-node/issues/225)) ([3504227](https://github.com/brettz9/eslint-plugin-node/commit/35042273322e2076ff66470100763be570c56315))
* **master:** release 17.2.0 ([#233](https://github.com/brettz9/eslint-plugin-node/issues/233)) ([539da1e](https://github.com/brettz9/eslint-plugin-node/commit/539da1e089805de1f504ef4f611e0a57285f1dc6))
* **master:** release 17.2.1 ([#239](https://github.com/brettz9/eslint-plugin-node/issues/239)) ([bad971c](https://github.com/brettz9/eslint-plugin-node/commit/bad971c90a57b302182d3d8dc883d6fc390d49b1))
* **master:** release 17.3.0 ([#247](https://github.com/brettz9/eslint-plugin-node/issues/247)) ([d8d8454](https://github.com/brettz9/eslint-plugin-node/commit/d8d8454879047e39497fd50fb867dd16572b8add))
* **master:** release 17.4.0 ([#256](https://github.com/brettz9/eslint-plugin-node/issues/256)) ([2f71e08](https://github.com/brettz9/eslint-plugin-node/commit/2f71e08a17f9d88de0a9529055190c475f9e0c4f))
* **master:** release 17.5.0 ([#262](https://github.com/brettz9/eslint-plugin-node/issues/262)) ([c7a014c](https://github.com/brettz9/eslint-plugin-node/commit/c7a014c2d9bf834c18384aa194eb521ba73f9538))
* **master:** release 17.5.1 ([#267](https://github.com/brettz9/eslint-plugin-node/issues/267)) ([c3e5a19](https://github.com/brettz9/eslint-plugin-node/commit/c3e5a19a3bcbd831dd719a6f9f8245fc4cfc904f))
* **master:** release 17.6.0 ([#270](https://github.com/brettz9/eslint-plugin-node/issues/270)) ([a99acb7](https://github.com/brettz9/eslint-plugin-node/commit/a99acb7bcb2a0d697ddbf00341d4e6724ae9a0e4))
* **master:** release 17.7.0 ([#273](https://github.com/brettz9/eslint-plugin-node/issues/273)) ([8551596](https://github.com/brettz9/eslint-plugin-node/commit/8551596aab2641ae786984ae6a0d1c5a3a4cb1ea))
* **master:** release 17.8.0 ([#281](https://github.com/brettz9/eslint-plugin-node/issues/281)) ([6dca24c](https://github.com/brettz9/eslint-plugin-node/commit/6dca24c4b0ced3f3b00ba68400cb3ab6c04bf721))
* **master:** release 17.8.1 ([#291](https://github.com/brettz9/eslint-plugin-node/issues/291)) ([988bdd4](https://github.com/brettz9/eslint-plugin-node/commit/988bdd4668543d287df7a2bc127f7b5dfd48021c))
* **master:** release 17.9.0 ([#299](https://github.com/brettz9/eslint-plugin-node/issues/299)) ([67bbfdf](https://github.com/brettz9/eslint-plugin-node/commit/67bbfdf3c6862dcbfe455a4afbd83fa60f9d1ea4))
* Merge supported and backport properties ([#177](https://github.com/brettz9/eslint-plugin-node/issues/177)) ([5d1cb98](https://github.com/brettz9/eslint-plugin-node/commit/5d1cb98ab4768e087718f4e09d6ab0fd5317ebb6))
* move data into rules ([4dd9baf](https://github.com/brettz9/eslint-plugin-node/commit/4dd9baff98e24783f1cbd909df9196a9566fb2a3))
* move recommended.json ([2a540a6](https://github.com/brettz9/eslint-plugin-node/commit/2a540a667bd7a17b43ea30a9b0840608e9ebbeb4))
* move rule tests parserOptions to ruleTester ([#157](https://github.com/brettz9/eslint-plugin-node/issues/157)) ([ad8f4f4](https://github.com/brettz9/eslint-plugin-node/commit/ad8f4f4fde1c356d1647005498c4709b2bfa4217))
* npm run format ([17e658e](https://github.com/brettz9/eslint-plugin-node/commit/17e658e297996db3f432f171095136e61ab995cc))
* prettier ignore lib/index.js ([fe82e2e](https://github.com/brettz9/eslint-plugin-node/commit/fe82e2e0af9ed05833351bf80cfd1134ae9a511d))
* punycode → domain in tests ([a6f90e1](https://github.com/brettz9/eslint-plugin-node/commit/a6f90e127ba95ca8d6d724fe4f48884304e19385))
* re-organize no-unsupported-features (fixes [#118](https://github.com/brettz9/eslint-plugin-node/issues/118)) ([217411d](https://github.com/brettz9/eslint-plugin-node/commit/217411d150956ceb55738265a25e66ea046a87c9))
* rebuild readme ([9a67d1e](https://github.com/brettz9/eslint-plugin-node/commit/9a67d1e52abbc83013d876ef3917f6d0f0da24b3))
* refactor a few rules ([d879ccb](https://github.com/brettz9/eslint-plugin-node/commit/d879ccbd6614d4421ac0bfaeef958b75d4c0d9ca))
* refactor with classes. ([ffc7fcb](https://github.com/brettz9/eslint-plugin-node/commit/ffc7fcb84296ee6cf5e52ed80c996f6ba5306a8a))
* refactoring ([d34e09c](https://github.com/brettz9/eslint-plugin-node/commit/d34e09cb936003ffff342f18449d6d067a2b178f))
* refactoring for no-unsupported-features/* ([fa25150](https://github.com/brettz9/eslint-plugin-node/commit/fa251507113b966ec501b95e7fabeb56d588334b))
* refactoring for prefer-global/* ([8f25248](https://github.com/brettz9/eslint-plugin-node/commit/8f25248006c98183588a5a7fc14359df50cee5f6))
* refactoring no-deprecated-api ([7ab875a](https://github.com/brettz9/eslint-plugin-node/commit/7ab875adfa2b3fd588c249e242788fc839a1c075))
* release latest version ([#218](https://github.com/brettz9/eslint-plugin-node/issues/218)) ([9814627](https://github.com/brettz9/eslint-plugin-node/commit/9814627748f07129659f7d86ee500f8465c1ab26))
* remove "n/no-unsupported-features" [#140](https://github.com/brettz9/eslint-plugin-node/issues/140) ([#173](https://github.com/brettz9/eslint-plugin-node/issues/173)) ([372b283](https://github.com/brettz9/eslint-plugin-node/commit/372b283b7b773963d34a3f7f761bdc1144c2e0d6))
* remove deprecated rule's tests ([aea8e82](https://github.com/brettz9/eslint-plugin-node/commit/aea8e82d1d01dfbbcfe18952fd59fb44a67f0872))
* remove object-assign from dependencies ([8f00ebb](https://github.com/brettz9/eslint-plugin-node/commit/8f00ebb381023193600687544f87a65acc5f5833))
* remove package-lock.json ([4f4e216](https://github.com/brettz9/eslint-plugin-node/commit/4f4e21677752edf0f012b2d6d4bbedef3cf3978f))
* Remove unused "meta.docs.category" property ([#133](https://github.com/brettz9/eslint-plugin-node/issues/133)) ([22ba54c](https://github.com/brettz9/eslint-plugin-node/commit/22ba54c07d956ab47edf1999ae5c6d090bc56c01))
* remove unused funding.yml ([4f3891c](https://github.com/brettz9/eslint-plugin-node/commit/4f3891c0224a0588aa210db67a4399268976fbc2))
* remove usage of @eslint/eslintrc ([#116](https://github.com/brettz9/eslint-plugin-node/issues/116)) ([150b34f](https://github.com/brettz9/eslint-plugin-node/commit/150b34fa60287b088fc51cf754ff716e4862883c))
* remove useless code. ([0ed6aa5](https://github.com/brettz9/eslint-plugin-node/commit/0ed6aa563592fca93200e3b94f2eec3410916d16))
* rename .eslintrc → .eslintrc.json ([719fb4d](https://github.com/brettz9/eslint-plugin-node/commit/719fb4d52bbebba4032cbc04d53dc71558b61ebe))
* rm superfluous argument. ([#93](https://github.com/brettz9/eslint-plugin-node/issues/93)) ([52ceb11](https://github.com/brettz9/eslint-plugin-node/commit/52ceb112383cff345d871023b2767659597f4f36))
* simpify tests for es modules ([390c9ec](https://github.com/brettz9/eslint-plugin-node/commit/390c9ec4c8c89b9f65699d6e00a7a11fabd591be))
* support the new rule `meta.type` property (fixes [#143](https://github.com/brettz9/eslint-plugin-node/issues/143)) ([#145](https://github.com/brettz9/eslint-plugin-node/issues/145)) ([153ab03](https://github.com/brettz9/eslint-plugin-node/commit/153ab03214dd2ed340d31fc91f18376c1ab47d76))
* switch 'eslint-utils' for some utilities ([1738d86](https://github.com/brettz9/eslint-plugin-node/commit/1738d868215db5acc6c6d568333983542751e309))
* switch to new rule-tester. ([41ceed7](https://github.com/brettz9/eslint-plugin-node/commit/41ceed7ad17e42f3074e664081f69639d0fb4322))
* tweak eslint config ([d7b975a](https://github.com/brettz9/eslint-plugin-node/commit/d7b975a07e1b876ca2c75597d054a81564b25685))
* tweak report timing ([3a0279c](https://github.com/brettz9/eslint-plugin-node/commit/3a0279caa1a7f62880d697caa8e98017bbcf15e2))
* update .travis.yml ([c849a27](https://github.com/brettz9/eslint-plugin-node/commit/c849a27add22fee81744dd89826576e3252853f1))
* update .travis.yml ([ecf6b11](https://github.com/brettz9/eslint-plugin-node/commit/ecf6b1194ec5b569d02669b3e14449f56ee60f9a))
* update .travis.yml ([453c4a5](https://github.com/brettz9/eslint-plugin-node/commit/453c4a559861b42fa2226efea63c3ff2084eb988))
* update .travis.yml ([69dc50a](https://github.com/brettz9/eslint-plugin-node/commit/69dc50af373aa4383690a5e5ef28d9b569c51628))
* update a few rules to use messageId ([c9138e5](https://github.com/brettz9/eslint-plugin-node/commit/c9138e5b53129f27d9db3be6d9fb472d6db57611))
* update dependency @typescript-eslint/parser to v6 ([#166](https://github.com/brettz9/eslint-plugin-node/issues/166)) ([4265094](https://github.com/brettz9/eslint-plugin-node/commit/4265094e1235dbd741f13ac6c70dd6b2f848452d))
* update dependency @typescript-eslint/parser to v7 ([#207](https://github.com/brettz9/eslint-plugin-node/issues/207)) ([0b8aeb3](https://github.com/brettz9/eslint-plugin-node/commit/0b8aeb3e8d8f1837a443d93a5bf55ad55bba085d))
* update dependency @typescript-eslint/typescript-estree to v7 ([#236](https://github.com/brettz9/eslint-plugin-node/issues/236)) ([a0b45ee](https://github.com/brettz9/eslint-plugin-node/commit/a0b45ee9c35279c29d3602609dad3b36d95d6f5f))
* update dependency eslint-plugin-eslint-plugin to v6 ([#237](https://github.com/brettz9/eslint-plugin-node/issues/237)) ([7addf99](https://github.com/brettz9/eslint-plugin-node/commit/7addf998e72d0f8ae92c52b112667bcb2c9558cd))
* update dependency globals to v14 ([#185](https://github.com/brettz9/eslint-plugin-node/issues/185)) ([9930101](https://github.com/brettz9/eslint-plugin-node/commit/993010140a686ca0aa43d5cdd5e00be7b0b1c97e))
* update dependency husky to v9 ([#208](https://github.com/brettz9/eslint-plugin-node/issues/208)) ([e84d47b](https://github.com/brettz9/eslint-plugin-node/commit/e84d47b98de65eb77ac96cef44af2adb901acac0))
* update dependency markdownlint-cli to ^0.38.0 ([#149](https://github.com/brettz9/eslint-plugin-node/issues/149)) ([3fd61be](https://github.com/brettz9/eslint-plugin-node/commit/3fd61bec4fde569405723757c48af08af27bf7b6))
* update dependency markdownlint-cli to ^0.39.0 ([#179](https://github.com/brettz9/eslint-plugin-node/issues/179)) ([cd5cbbb](https://github.com/brettz9/eslint-plugin-node/commit/cd5cbbba4d00d4ae888e42e7a481794c9aafc1d8))
* update dependency markdownlint-cli to ^0.40.0 ([#263](https://github.com/brettz9/eslint-plugin-node/issues/263)) ([1e41e7c](https://github.com/brettz9/eslint-plugin-node/commit/1e41e7cf5328df05d07aeab8bc9c5d0f27d33695))
* update dependency markdownlint-cli to ^0.41.0 ([#287](https://github.com/brettz9/eslint-plugin-node/issues/287)) ([0efe751](https://github.com/brettz9/eslint-plugin-node/commit/0efe751b1fa1194ddc58b0934a1299d982e93d35))
* update dependency minimatch to v9 ([#167](https://github.com/brettz9/eslint-plugin-node/issues/167)) ([5ad657c](https://github.com/brettz9/eslint-plugin-node/commit/5ad657cf2fd70f62f40b70734564af050cd58428))
* update dependency release-it to v17 ([#168](https://github.com/brettz9/eslint-plugin-node/issues/168)) ([1c91e05](https://github.com/brettz9/eslint-plugin-node/commit/1c91e053b310896e5f9aaec621c1929154699958))
* update eslint-doc-generator to v1.0.0 ([#72](https://github.com/brettz9/eslint-plugin-node/issues/72)) ([27a73d5](https://github.com/brettz9/eslint-plugin-node/commit/27a73d5a5b4b45cae4697215d139dac788a1fed5))
* update outdated funding ([#246](https://github.com/brettz9/eslint-plugin-node/issues/246)) ([8d711f5](https://github.com/brettz9/eslint-plugin-node/commit/8d711f5446655c9874aeffb2ef28b3c4d8463fb6))
* Update package.json links to new repository location ([#62](https://github.com/brettz9/eslint-plugin-node/issues/62)) ([63fc031](https://github.com/brettz9/eslint-plugin-node/commit/63fc03176513782c91631ee25afdf1a1ecb005c3))
* Update release manifest (17.3.1) ([#255](https://github.com/brettz9/eslint-plugin-node/issues/255)) ([cf576cb](https://github.com/brettz9/eslint-plugin-node/commit/cf576cb45bd1f13b675b1612e79f571acfb780af))
* update rules meta.url ([ffed3ed](https://github.com/brettz9/eslint-plugin-node/commit/ffed3edbc94dfac87ee817fafc3f6e1d4125477f))
* update travis.yml ([04e0cf7](https://github.com/brettz9/eslint-plugin-node/commit/04e0cf7401239f91363bbf162b10f22b233ac5b1))
* upgrade compatible deps ([8f6f11d](https://github.com/brettz9/eslint-plugin-node/commit/8f6f11da5d072fe7b0ca1e916744e527ee260db2))
* upgrade dependencies ([0eb4927](https://github.com/brettz9/eslint-plugin-node/commit/0eb49270060f8863f425d86f8f6e7cc393fbce13))
* upgrade dependencies ([5936718](https://github.com/brettz9/eslint-plugin-node/commit/5936718d266e24cd1af7542ab7e456bf846a00c8))
* upgrade dependencies ([6982b34](https://github.com/brettz9/eslint-plugin-node/commit/6982b343c02ef98676f9fe75735235de0706a937))
* upgrade dependencies ([2e2d464](https://github.com/brettz9/eslint-plugin-node/commit/2e2d464d9afe0ce1e1e2ad8899c6f744d182b4bb))
* upgrade dependencies ([9931ded](https://github.com/brettz9/eslint-plugin-node/commit/9931ded1228dc440160b5e444db1514b55e455e1))
* upgrade dependencies ([734d2e7](https://github.com/brettz9/eslint-plugin-node/commit/734d2e73b1fbd506bf5bdcb0dc375bfaf9046cab))
* upgrade deps to latest ([#18](https://github.com/brettz9/eslint-plugin-node/issues/18)) ([88b4d95](https://github.com/brettz9/eslint-plugin-node/commit/88b4d957f7673227bd578ed6e45edbbe2504ae11))
* upgrade eslint & eslint-config-mysticatea ([9e77b54](https://github.com/brettz9/eslint-plugin-node/commit/9e77b54bcccbfd6a370e390516155af80e0e1439))
* upgrade ESLint config ([c071fdb](https://github.com/brettz9/eslint-plugin-node/commit/c071fdb1c9ff32853c32fe06b2e1e5520b6574c3))
* upgrade eslint-config-mysticatea ([382886e](https://github.com/brettz9/eslint-plugin-node/commit/382886e54d9c863dda8e731670b544feaf581e33))
* upgrade eslint-doc-generator v1.4 ([#76](https://github.com/brettz9/eslint-plugin-node/issues/76)) ([83446a1](https://github.com/brettz9/eslint-plugin-node/commit/83446a1678128c65f76270c79619c16e542f9041))
* upgrade globals v15 ([#241](https://github.com/brettz9/eslint-plugin-node/issues/241)) ([eb11b5b](https://github.com/brettz9/eslint-plugin-node/commit/eb11b5b35a6a797dc7fba6df53b1c4dada3a2a55))
* upgrade non-major deps ([b0faa87](https://github.com/brettz9/eslint-plugin-node/commit/b0faa87f3d1931ab10ecb4cfbeec2546ceb45792))
* upgrade prettier v3 ([#165](https://github.com/brettz9/eslint-plugin-node/issues/165)) ([bbfde8d](https://github.com/brettz9/eslint-plugin-node/commit/bbfde8d4274c68f75c6518d5aaab8aae49891c27))
* use `ts-ignore-import` to lighten the dependencies ([#219](https://github.com/brettz9/eslint-plugin-node/issues/219)) ([fb0aaae](https://github.com/brettz9/eslint-plugin-node/commit/fb0aaae9a5d540542a4122fe333097c200b78b95))
* use maintained `npm-run-all` fork ([#124](https://github.com/brettz9/eslint-plugin-node/issues/124)) ([98ea90e](https://github.com/brettz9/eslint-plugin-node/commit/98ea90e745081578c0888d17a980a3a9239e1e95))
* use new rule format ([fb485af](https://github.com/brettz9/eslint-plugin-node/commit/fb485af744dae63b6ceba978176a4565f980b8f4))
* use semver public API's. ([#99](https://github.com/brettz9/eslint-plugin-node/issues/99)) ([846e677](https://github.com/brettz9/eslint-plugin-node/commit/846e677789dc290c1f7a9fff658fbdc1c5bf5171))


### 🤖 Automation

* add node v18 ([#16](https://github.com/brettz9/eslint-plugin-node/issues/16)) ([e20cc18](https://github.com/brettz9/eslint-plugin-node/commit/e20cc18e59a4e60491f0c69f0a61935fa5931904))
* add node v19(ubuntu) ([#68](https://github.com/brettz9/eslint-plugin-node/issues/68)) ([1665777](https://github.com/brettz9/eslint-plugin-node/commit/16657772886f047d0f967f1a4b0648da636b521a))
* add node v20 ([#117](https://github.com/brettz9/eslint-plugin-node/issues/117)) ([b7d0536](https://github.com/brettz9/eslint-plugin-node/commit/b7d0536d3724522b66cc1495c3acb8f12d74341f))
* run test on eslint pre-releases ([#171](https://github.com/brettz9/eslint-plugin-node/issues/171)) ([77de809](https://github.com/brettz9/eslint-plugin-node/commit/77de80903c01b1c4e9a9c4bb04983e8f5f5f3f04))
* update scripts to use the new package name ([#6](https://github.com/brettz9/eslint-plugin-node/issues/6)) ([df759eb](https://github.com/brettz9/eslint-plugin-node/commit/df759eb1a2891545efcd861e9fdd95de121802f3))
* update scripts/update-lib-index.js for eslint v8 ([e183f6e](https://github.com/brettz9/eslint-plugin-node/commit/e183f6e132feb2018107411536426ffa46bfbcd9))

## [17.9.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.8.1...v17.9.0) (2024-06-14)


### 🌟 Features

* Add flag ignorePrivate to no-unpublished-x rules ([#298](https://github.com/eslint-community/eslint-plugin-n/issues/298)) ([0609431](https://github.com/eslint-community/eslint-plugin-n/commit/0609431dabcd9402720071025c0206d2686e1d78))

## [17.8.1](https://github.com/eslint-community/eslint-plugin-n/compare/v17.8.0...v17.8.1) (2024-06-06)


### 🩹 Fixes

* hashbang + eslint v8 compat issue ([e82974f](https://github.com/eslint-community/eslint-plugin-n/commit/e82974fc724e4a410f85459f4cd3e5367939cc9c))
* hashbang + eslint v8 compat issue ([#290](https://github.com/eslint-community/eslint-plugin-n/issues/290)) ([e82974f](https://github.com/eslint-community/eslint-plugin-n/commit/e82974fc724e4a410f85459f4cd3e5367939cc9c))

## [17.8.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.7.0...v17.8.0) (2024-06-05)


### 🌟 Features

* **node-builtin:** Add node 22.2.0 support ([#282](https://github.com/eslint-community/eslint-plugin-n/issues/282)) ([5221c40](https://github.com/eslint-community/eslint-plugin-n/commit/5221c4015fb939cfb33231b7b6f4669cf1197ef7))


### 🩹 Fixes

* Allow for misconfigured default exports ([#288](https://github.com/eslint-community/eslint-plugin-n/issues/288)) ([92e18b5](https://github.com/eslint-community/eslint-plugin-n/commit/92e18b572f7bd2427f050eab8484cb393e1dac7a))


### 🧹 Chores

* add a test for self-ref ([#280](https://github.com/eslint-community/eslint-plugin-n/issues/280)) ([4f50dfe](https://github.com/eslint-community/eslint-plugin-n/commit/4f50dfe6528e32749aac315e53b351345cfc8c13))
* update dependency markdownlint-cli to ^0.41.0 ([#287](https://github.com/eslint-community/eslint-plugin-n/issues/287)) ([0efe751](https://github.com/eslint-community/eslint-plugin-n/commit/0efe751b1fa1194ddc58b0934a1299d982e93d35))

## [17.7.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.6.0...v17.7.0) (2024-05-14)


### 🌟 Features

* **hashbang:** Add support to map extensions to executables ([#278](https://github.com/eslint-community/eslint-plugin-n/issues/278)) ([3fd7639](https://github.com/eslint-community/eslint-plugin-n/commit/3fd7639e4d98d2cd936682197ef4004d59adadfd))
* **node-builtin:** Add node 20.13.0, 22.0.0, and 22.1.0 support ([#276](https://github.com/eslint-community/eslint-plugin-n/issues/276)) ([4a685c0](https://github.com/eslint-community/eslint-plugin-n/commit/4a685c05e2d5770e22c46dcb78267fa8c484f725))


### 🩹 Fixes

* **node-builtins:** Remove "node:" prefix from "ignores" message ([#277](https://github.com/eslint-community/eslint-plugin-n/issues/277)) ([704f0b9](https://github.com/eslint-community/eslint-plugin-n/commit/704f0b9373542e03b42102d30bc44cb7e30fc5d8))


### 📚 Documentation

* **node-builtins:** Specify that only static properties are supported ([#272](https://github.com/eslint-community/eslint-plugin-n/issues/272)) ([735a520](https://github.com/eslint-community/eslint-plugin-n/commit/735a5207aee828e324835bdb0c7fa743347ef4b9))
* Provide an example with eslint-plugin-n to Playground ([#275](https://github.com/eslint-community/eslint-plugin-n/issues/275)) ([cb8ffa6](https://github.com/eslint-community/eslint-plugin-n/commit/cb8ffa62d07869dd23985f7d861ad3c60deec4f8))

## [17.6.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.5.1...v17.6.0) (2024-05-10)


### 🌟 Features

* Add support for ignoring experemental features ([#269](https://github.com/eslint-community/eslint-plugin-n/issues/269)) ([c046376](https://github.com/eslint-community/eslint-plugin-n/commit/c046376fb52bef8104502ffab3c457412d1a1e27))


### 📚 Documentation

* add maintainance info ([#271](https://github.com/eslint-community/eslint-plugin-n/issues/271)) ([b454488](https://github.com/eslint-community/eslint-plugin-n/commit/b454488bd63c046d101305c40d24bf44ae83971e)), closes [#194](https://github.com/eslint-community/eslint-plugin-n/issues/194)

## [17.5.1](https://github.com/eslint-community/eslint-plugin-n/compare/v17.5.0...v17.5.1) (2024-05-07)


### 🩹 Fixes

* Add supported version to Buffer constructor ([#266](https://github.com/eslint-community/eslint-plugin-n/issues/266)) ([030f51b](https://github.com/eslint-community/eslint-plugin-n/commit/030f51bacd21918ef6d5b2bba9ec77cd701c3eba))

## [17.5.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.4.0...v17.5.0) (2024-05-07)


### 🌟 Features

* **import-target:** Add resolution error reason ([#264](https://github.com/eslint-community/eslint-plugin-n/issues/264)) ([982a723](https://github.com/eslint-community/eslint-plugin-n/commit/982a723dfb81dc141b093e27b41cd67f82ba8587))
* **node-builtins:** Add node globals ([#261](https://github.com/eslint-community/eslint-plugin-n/issues/261)) ([9466731](https://github.com/eslint-community/eslint-plugin-n/commit/946673149b51b84581f91890495c810a496e0022))


### 🩹 Fixes

* remove invalid es-builtins ([#258](https://github.com/eslint-community/eslint-plugin-n/issues/258)) ([ecdf019](https://github.com/eslint-community/eslint-plugin-n/commit/ecdf019c54c5bd720c20d2ea21886559c15f3205))


### 🧹 Chores

* update dependency markdownlint-cli to ^0.40.0 ([#263](https://github.com/eslint-community/eslint-plugin-n/issues/263)) ([1e41e7c](https://github.com/eslint-community/eslint-plugin-n/commit/1e41e7cf5328df05d07aeab8bc9c5d0f27d33695))

## [17.4.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.3.1...v17.4.0) (2024-04-30)


### 🌟 Features

* no-deprecated-api support removed api ([#240](https://github.com/eslint-community/eslint-plugin-n/issues/240)) ([36fd35d](https://github.com/eslint-community/eslint-plugin-n/commit/36fd35d9bbbaec43dd911e06bd83625cd1650fb3))


### 🩹 Fixes

* unsupported-features/node-builtins-modules version comparation ([#257](https://github.com/eslint-community/eslint-plugin-n/issues/257)) ([5c67787](https://github.com/eslint-community/eslint-plugin-n/commit/5c67787cb191ff7409fa17ec5b12cfdc3a7a26d3))


### 🧹 Chores

* Update release manifest (17.3.1) ([#255](https://github.com/eslint-community/eslint-plugin-n/issues/255)) ([cf576cb](https://github.com/eslint-community/eslint-plugin-n/commit/cf576cb45bd1f13b675b1612e79f571acfb780af))

## [17.3.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.2.1...v17.3.0) (2024-04-24)


### 🌟 Features

* More es-syntax deprecations ([#249](https://github.com/eslint-community/eslint-plugin-n/issues/249)) ([2ecee79](https://github.com/eslint-community/eslint-plugin-n/commit/2ecee796c53733c70ea671a1e029aed9cf06d050))


### 🩹 Fixes

* unsupported-features/node-builtins-modules range compare ([#252](https://github.com/eslint-community/eslint-plugin-n/issues/252)) ([d50ae85](https://github.com/eslint-community/eslint-plugin-n/commit/d50ae85c209a47a8a5d4c1bedaa94e6a77540095))


### 🧹 Chores

* update outdated funding ([#246](https://github.com/eslint-community/eslint-plugin-n/issues/246)) ([8d711f5](https://github.com/eslint-community/eslint-plugin-n/commit/8d711f5446655c9874aeffb2ef28b3c4d8463fb6))
* upgrade globals v15 ([#241](https://github.com/eslint-community/eslint-plugin-n/issues/241)) ([eb11b5b](https://github.com/eslint-community/eslint-plugin-n/commit/eb11b5b35a6a797dc7fba6df53b1c4dada3a2a55))

## [17.2.1](https://github.com/eslint-community/eslint-plugin-n/compare/v17.2.0...v17.2.1) (2024-04-15)


### 🩹 Fixes

* **unsupported-features:** Improve URL module ([#244](https://github.com/eslint-community/eslint-plugin-n/issues/244)) ([6581979](https://github.com/eslint-community/eslint-plugin-n/commit/6581979cfb6afa6a50531d37303af24aa7b4db37)), closes [#243](https://github.com/eslint-community/eslint-plugin-n/issues/243)


### 🧹 Chores

* update dependency @typescript-eslint/typescript-estree to v7 ([#236](https://github.com/eslint-community/eslint-plugin-n/issues/236)) ([a0b45ee](https://github.com/eslint-community/eslint-plugin-n/commit/a0b45ee9c35279c29d3602609dad3b36d95d6f5f))
* update dependency eslint-plugin-eslint-plugin to v6 ([#237](https://github.com/eslint-community/eslint-plugin-n/issues/237)) ([7addf99](https://github.com/eslint-community/eslint-plugin-n/commit/7addf998e72d0f8ae92c52b112667bcb2c9558cd))

## [17.2.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.1.0...v17.2.0) (2024-04-10)


### 🌟 Features

* **no-missing-imports:** add `tryExtensions` option ([#228](https://github.com/eslint-community/eslint-plugin-n/issues/228)) ([ae5329c](https://github.com/eslint-community/eslint-plugin-n/commit/ae5329c06b38da1220a352d4d268cfa8038c0d00))
* **no-unsupported-features:** ✨ Update to node v20.12.0/v21.7.0 ([#229](https://github.com/eslint-community/eslint-plugin-n/issues/229)) ([a8d0539](https://github.com/eslint-community/eslint-plugin-n/commit/a8d0539ae99697f0e3441625c61e2e6ed7a10b9a))


### 🩹 Fixes

* `stream/promises` is stable ([02a264e](https://github.com/eslint-community/eslint-plugin-n/commit/02a264e0acb7ba913500e195fe0a2a6aaae74c6e))
* **no-unsupported-features:** `stream/promises` is stable ([#235](https://github.com/eslint-community/eslint-plugin-n/issues/235)) ([02a264e](https://github.com/eslint-community/eslint-plugin-n/commit/02a264e0acb7ba913500e195fe0a2a6aaae74c6e)), closes [#234](https://github.com/eslint-community/eslint-plugin-n/issues/234)

## [17.1.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.0.0...v17.1.0) (2024-04-09)


### 🌟 Features

* add `name` to flat configs ([#224](https://github.com/eslint-community/eslint-plugin-n/issues/224)) ([24512a0](https://github.com/eslint-community/eslint-plugin-n/commit/24512a0fe27bcb9b2a0ed20cd83bcbd3c0060d0b))
* **import-target:** Add resolution error reason ([ed7b25c](https://github.com/eslint-community/eslint-plugin-n/commit/ed7b25cf4ccb3f27bf89993a7fc8c706e3491ad5))
* remove "is-builtin-module" dependency (fixes [#232](https://github.com/eslint-community/eslint-plugin-n/issues/232)) ([#227](https://github.com/eslint-community/eslint-plugin-n/issues/227)) ([03619ee](https://github.com/eslint-community/eslint-plugin-n/commit/03619eed4d24cb8ed79c467fe4a620bd58fea4cd))


### 📚 Documentation

* add v17 changelog ([#223](https://github.com/eslint-community/eslint-plugin-n/issues/223)) ([4fb36eb](https://github.com/eslint-community/eslint-plugin-n/commit/4fb36eb253536b694d16b72d31221c98f1012f9f))

## [17.0.0](https://github.com/eslint-community/eslint-plugin-n/compare/v17.0.0...v17.0.0-8) (2024-04-08)

## 💥 Breaking changes:

* feat!: drop eslint v7 & node.js < 18 ([#161](https://github.com/eslint-community/eslint-plugin-n/issues/161)) ([41ceed7](https://github.com/eslint-community/eslint-plugin-n/commit/41ceed7))
* feat!: Start using `enhanced-resolve` to improve ts support ([#139](https://github.com/eslint-community/eslint-plugin-n/issues/139)) ([dc9f473](https://github.com/eslint-community/eslint-plugin-n/commit/dc9f473))
* rename rule shebang => hashbang, deprecate rule shebang ([#198](https://github.com/eslint-community/eslint-plugin-n/issues/198))

## Features

* typescript (jsdoc) checking and definition generation ([#169](https://github.com/eslint-community/eslint-plugin-n/issues/169)) ([6d8ed14](https://github.com/eslint-community/eslint-plugin-n/commit/6d8ed14c186a814c3a258993fb6c986a02ed5568))
* rename rule shebang =&gt; hashbang, deprecate rule shebang ([#198](https://github.com/eslint-community/eslint-plugin-n/issues/198)) ([cefdb1c](https://github.com/eslint-community/eslint-plugin-n/commit/cefdb1c26d856b544470e825daef2dfa5d0e4a30)), closes [#196](https://github.com/eslint-community/eslint-plugin-n/issues/196)
* **shebang:** add support for env's split-string option ([#195](https://github.com/eslint-community/eslint-plugin-n/issues/195)) ([b383b49](https://github.com/eslint-community/eslint-plugin-n/commit/b383b4971df4f4b67099655797b654b36d6a8fdf))
* Update ES Syntax ([#189](https://github.com/eslint-community/eslint-plugin-n/issues/189)) ([4778ae8](https://github.com/eslint-community/eslint-plugin-n/commit/4778ae86c398f90da13248c2d31bfc4a83cd2dea))
* feat: Update es-builtins ([#174](https://github.com/eslint-community/eslint-plugin-n/issues/174)) ([fbc9e7b](https://github.com/eslint-community/eslint-plugin-n/commit/fbc9e7b))
* feat(no-unsupported-features): Update to v21.6.1 of node ([#180](https://github.com/eslint-community/eslint-plugin-n/issues/180)) ([d24f645](https://github.com/eslint-community/eslint-plugin-n/commit/d24f645))
* feat: Add n/prefer-node-protocol rule ([#183](https://github.com/eslint-community/eslint-plugin-n/issues/183)) ([88d1c37](https://github.com/eslint-community/eslint-plugin-n/commit/88d1c37))
* feat(shebang): Add options to ignore unpublished files ([#172](https://github.com/eslint-community/eslint-plugin-n/issues/172)) ([5609abb](https://github.com/eslint-community/eslint-plugin-n/commit/5609abb))

## Bugfixes

* prefer-node-protocol: not first target ([#204](https://github.com/eslint-community/eslint-plugin-n/issues/204)) ([caab777](https://github.com/eslint-community/eslint-plugin-n/commit/caab77714ec9195c07290d4c212a95f11b48bb5f))
* **prefer-node-protocol:** continue on version range check ([#206](https://github.com/eslint-community/eslint-plugin-n/issues/206)) ([14d2ea9](https://github.com/eslint-community/eslint-plugin-n/commit/14d2ea90c1609b49e95cc805105711c62bf6fd50))
* prefer-node-prefix: pass moduleName ([#203](https://github.com/eslint-community/eslint-plugin-n/issues/203))
* **no-unsupported-features:** Remove use of `static` as a variable ([#190](https://github.com/eslint-community/eslint-plugin-n/issues/190)) ([e31d868](https://github.com/eslint-community/eslint-plugin-n/commit/e31d8683b65a6f982cb91634f951afd0fe5583ae))
* fix: Remove `require("util")` import in import-target (#181) (d32eff3)

## Chores

* use `ts-ignore-import` to lighten the dependencies ([#219](https://github.com/eslint-community/eslint-plugin-n/issues/219)) ([fb0aaae](https://github.com/eslint-community/eslint-plugin-n/commit/fb0aaae9a5d540542a4122fe333097c200b78b95))
* update dependency @typescript-eslint/parser to v7 ([#207](https://github.com/eslint-community/eslint-plugin-n/issues/207)) ([0b8aeb3](https://github.com/eslint-community/eslint-plugin-n/commit/0b8aeb3e8d8f1837a443d93a5bf55ad55bba085d))
* update dependency husky to v9 ([#208](https://github.com/eslint-community/eslint-plugin-n/issues/208)) ([e84d47b](https://github.com/eslint-community/eslint-plugin-n/commit/e84d47b98de65eb77ac96cef44af2adb901acac0))
* Enable global strict eslint rule ([#191](https://github.com/eslint-community/eslint-plugin-n/issues/191)) ([99fe387](https://github.com/eslint-community/eslint-plugin-n/commit/99fe38722d02de867f4bd8061a343b9754b62610))
* Migrate to manifest config ([#192](https://github.com/eslint-community/eslint-plugin-n/issues/192)) ([c8a87f3](https://github.com/eslint-community/eslint-plugin-n/commit/c8a87f3ef99348e547259f3939274cdf4da72b08))
* docs: improve wording of file-extension-in-import docs (#110) (3f178ab)
* build: run test on eslint pre-releases (#171) (77de809)
* ci: Make release-please publish pre-releases (#186) (4b12cdc)
* chore: update dependency globals to v14 (#185) (9930101)
* chore: update dependency markdownlint-cli to ^0.39.0 (#179) (cd5cbbb)
* chore: Merge supported and backport properties (#177) (5d1cb98)
* chore: `npm run format` (#175) (17e658e)
* chore!: remove "n/no-unsupported-features" #140 (#173) (372b283)
* chore: update dependency minimatch to v9 (#167) (5ad657c)
* chore: add release-please (#170) (fc77da2)
* chore: update dependency @typescript-eslint/parser to v6 (#166) (4265094)
* chore: update dependency markdownlint-cli to ^0.38.0 (#149) (3fd61be)
* chore: update dependency release-it to v17 (#168) (1c91e05)
* chore: upgrade prettier v3 (#165) (bbfde8d)

## [17.0.0-8](https://github.com/eslint-community/eslint-plugin-n/compare/v17.0.0-7...v17.0.0-8) (2024-04-08)


### Chores

* use `ts-ignore-import` to lighten the dependencies ([#219](https://github.com/eslint-community/eslint-plugin-n/issues/219)) ([fb0aaae](https://github.com/eslint-community/eslint-plugin-n/commit/fb0aaae9a5d540542a4122fe333097c200b78b95))

## [17.0.0-7](https://github.com/eslint-community/eslint-plugin-n/compare/v17.0.0-6...v17.0.0-7) (2024-04-07)


### Features

* typescript (jsdoc) checking and definition generation ([#169](https://github.com/eslint-community/eslint-plugin-n/issues/169)) ([6d8ed14](https://github.com/eslint-community/eslint-plugin-n/commit/6d8ed14c186a814c3a258993fb6c986a02ed5568))


### Bug Fixes

* change peer dependencies to allow eslint v9 ([#216](https://github.com/eslint-community/eslint-plugin-n/issues/216)) ([5e82d7f](https://github.com/eslint-community/eslint-plugin-n/commit/5e82d7f26aa8dc58b46584c9fe3c74a11c265228))

## [17.0.0-6](https://github.com/eslint-community/eslint-plugin-n/compare/v17.0.0-5...v17.0.0-6) (2024-03-25)


### Bug Fixes

* prefer-node-protocol: not first target ([#204](https://github.com/eslint-community/eslint-plugin-n/issues/204)) ([caab777](https://github.com/eslint-community/eslint-plugin-n/commit/caab77714ec9195c07290d4c212a95f11b48bb5f))
* **prefer-node-protocol:** continue on version range check ([#206](https://github.com/eslint-community/eslint-plugin-n/issues/206)) ([14d2ea9](https://github.com/eslint-community/eslint-plugin-n/commit/14d2ea90c1609b49e95cc805105711c62bf6fd50))


### Chores

* update dependency @typescript-eslint/parser to v7 ([#207](https://github.com/eslint-community/eslint-plugin-n/issues/207)) ([0b8aeb3](https://github.com/eslint-community/eslint-plugin-n/commit/0b8aeb3e8d8f1837a443d93a5bf55ad55bba085d))
* update dependency husky to v9 ([#208](https://github.com/eslint-community/eslint-plugin-n/issues/208)) ([e84d47b](https://github.com/eslint-community/eslint-plugin-n/commit/e84d47b98de65eb77ac96cef44af2adb901acac0))

## [17.0.0-5](https://github.com/eslint-community/eslint-plugin-n/compare/v17.0.0-4...v17.0.0-5) (2024-03-19)


### ⚠ BREAKING CHANGES

* prefer-node-prefix: pass moduleName ([#203](https://github.com/eslint-community/eslint-plugin-n/issues/203))

### Features

* prefer-node-prefix: pass moduleName ([#203](https://github.com/eslint-community/eslint-plugin-n/issues/203)) ([38985ca](https://github.com/eslint-community/eslint-plugin-n/commit/38985ca63537cc56ae2476457ec7d5e433bf0a2f))


### Bug Fixes

* explicitly support ESLint 9.0.0 pre-releases ([#200](https://github.com/eslint-community/eslint-plugin-n/issues/200)) ([a5eaa9c](https://github.com/eslint-community/eslint-plugin-n/commit/a5eaa9c867bc2e87b1fa54920c85acd1e8f9f927))


### Documentation

* Remove text "Node does not support modules yet" ([#202](https://github.com/eslint-community/eslint-plugin-n/issues/202)) ([5abca5b](https://github.com/eslint-community/eslint-plugin-n/commit/5abca5bb6f1166045578ba7d51cda36b32cb333b))

## [17.0.0-4](https://github.com/eslint-community/eslint-plugin-n/compare/17.0.0-3...v17.0.0-4) (2024-03-06)


### ⚠ BREAKING CHANGES

* rename rule shebang => hashbang, deprecate rule shebang ([#198](https://github.com/eslint-community/eslint-plugin-n/issues/198))

### Features

* rename rule shebang =&gt; hashbang, deprecate rule shebang ([#198](https://github.com/eslint-community/eslint-plugin-n/issues/198)) ([cefdb1c](https://github.com/eslint-community/eslint-plugin-n/commit/cefdb1c26d856b544470e825daef2dfa5d0e4a30)), closes [#196](https://github.com/eslint-community/eslint-plugin-n/issues/196)
* **shebang:** add support for env's split-string option ([#195](https://github.com/eslint-community/eslint-plugin-n/issues/195)) ([b383b49](https://github.com/eslint-community/eslint-plugin-n/commit/b383b4971df4f4b67099655797b654b36d6a8fdf))
* Update ES Syntax ([#189](https://github.com/eslint-community/eslint-plugin-n/issues/189)) ([4778ae8](https://github.com/eslint-community/eslint-plugin-n/commit/4778ae86c398f90da13248c2d31bfc4a83cd2dea))


### Bug Fixes

* **no-unsupported-features:** Remove use of `static` as a variable ([#190](https://github.com/eslint-community/eslint-plugin-n/issues/190)) ([e31d868](https://github.com/eslint-community/eslint-plugin-n/commit/e31d8683b65a6f982cb91634f951afd0fe5583ae))


### Chores

* Enable global strict eslint rule ([#191](https://github.com/eslint-community/eslint-plugin-n/issues/191)) ([99fe387](https://github.com/eslint-community/eslint-plugin-n/commit/99fe38722d02de867f4bd8061a343b9754b62610))
* Migrate to manifest config ([#192](https://github.com/eslint-community/eslint-plugin-n/issues/192)) ([c8a87f3](https://github.com/eslint-community/eslint-plugin-n/commit/c8a87f3ef99348e547259f3939274cdf4da72b08))
