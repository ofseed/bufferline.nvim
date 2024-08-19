# Changelog

## [5.0.0](https://github.com/ofseed/bufferline.nvim/compare/v4.7.0...v5.0.0) (2024-08-19)


### ⚠ BREAKING CHANGES

* **groups:** change argument to group matcher
* **config:** deprecate show_buffer_default_icon
* **tests:** load dependencies in init.lua
* **commands:** reuse close_command for deleting commands ([#582](https://github.com/ofseed/bufferline.nvim/issues/582))
* **config:** add underline indicator style ([#514](https://github.com/ofseed/bufferline.nvim/issues/514))
* **highlights:** use nvim_set_hl style args ([#497](https://github.com/ofseed/bufferline.nvim/issues/497))
* **ui:** Change internal representation of tabline ([#412](https://github.com/ofseed/bufferline.nvim/issues/412))
* **diagnostics:** remove deprecated function

### break

* **highlights:** use nvim_set_hl style args ([#497](https://github.com/ofseed/bufferline.nvim/issues/497)) ([f248437](https://github.com/ofseed/bufferline.nvim/commit/f248437e31b97f2a91173ee770b181b8d8ccdd42))


### Features

* add `auto_toggle_bufferline` option ([#876](https://github.com/ofseed/bufferline.nvim/issues/876)) ([f6f00d9](https://github.com/ofseed/bufferline.nvim/commit/f6f00d9ac1a51483ac78418f9e63126119a70709))
* add `get_elements` command ([#583](https://github.com/ofseed/bufferline.nvim/issues/583)) ([5b1add3](https://github.com/ofseed/bufferline.nvim/commit/5b1add37a2ea2a666dcd44380bd793832e35835e))
* add auto close option for groups ([6e76969](https://github.com/ofseed/bufferline.nvim/commit/6e76969d937ec11be58d6862b2e223ae79a519ee))
* add cterm color support ([#417](https://github.com/ofseed/bufferline.nvim/issues/417)) ([737566c](https://github.com/ofseed/bufferline.nvim/commit/737566c7c6ea0dc348455ef1b11ca5491d77b931))
* add FUNDING.yaml ([b2a0691](https://github.com/ofseed/bufferline.nvim/commit/b2a0691df8a51a7590122aef456db1d70445647d))
* Add hint diagnostic highlight ([#257](https://github.com/ofseed/bufferline.nvim/issues/257)) ([7b193b1](https://github.com/ofseed/bufferline.nvim/commit/7b193b1152fcede020d9f69c8239f8a9ef02356f))
* add option to disable ft icon highlights ([650afcd](https://github.com/ofseed/bufferline.nvim/commit/650afcd7a318071efbc795b381a891d613d7d37a)), closes [#237](https://github.com/ofseed/bufferline.nvim/issues/237)
* add option to disable name truncation ([#533](https://github.com/ofseed/bufferline.nvim/issues/533)) ([0caca76](https://github.com/ofseed/bufferline.nvim/commit/0caca766d1b579fb9947825b98c9504267a49504))
* add pinned groups ([#351](https://github.com/ofseed/bufferline.nvim/issues/351)) ([c703e8d](https://github.com/ofseed/bufferline.nvim/commit/c703e8d93a2489541fa1cc431f53edbac6b0966c))
* add slope separator ([#659](https://github.com/ofseed/bufferline.nvim/issues/659)) ([6837ad3](https://github.com/ofseed/bufferline.nvim/commit/6837ad30bdae5dfb812d5d6114f33d273fd4a66f))
* allow controlling numbers styling using a function ([#199](https://github.com/ofseed/bufferline.nvim/issues/199)) ([c9e0902](https://github.com/ofseed/bufferline.nvim/commit/c9e09021be4f578f4336c41a339ee535dc2f3986))
* allow moving buffers to arbitrary positions ([#675](https://github.com/ofseed/bufferline.nvim/issues/675)) ([e0aa1fd](https://github.com/ofseed/bufferline.nvim/commit/e0aa1fd8323609d9c7617b3d54e27236dea43741))
* buffer groups ([#179](https://github.com/ofseed/bufferline.nvim/issues/179)) ([efb9a69](https://github.com/ofseed/bufferline.nvim/commit/efb9a699d2132a1ace759dbb1405cf6f369c4adc))
* **colors:** add diagnostic underline fallback ([bd9915f](https://github.com/ofseed/bufferline.nvim/commit/bd9915fa13f53176fe3a4a943e3f95c7e4312e50))
* **command:** add BufferLineCloseOthers command ([#774](https://github.com/ofseed/bufferline.nvim/issues/774)) ([9d6ab3a](https://github.com/ofseed/bufferline.nvim/commit/9d6ab3a56ad71bed9929c7acd7620e827a073d25))
* **commands/go_to:** go to the last element if index out of bounds ([#758](https://github.com/ofseed/bufferline.nvim/issues/758)) ([6073426](https://github.com/ofseed/bufferline.nvim/commit/60734264a8655a7db3595159fb50076dc24c2f2c))
* **commands:** add option to wrap when moving buffers at ends ([#759](https://github.com/ofseed/bufferline.nvim/issues/759)) ([da1875c](https://github.com/ofseed/bufferline.nvim/commit/da1875c1eee9aa9b7e19cda5c70ed7d7702d5f06))
* **commands:** fallback to b{prev|next} when cycling buffers ([#493](https://github.com/ofseed/bufferline.nvim/issues/493)) ([b1a63fe](https://github.com/ofseed/bufferline.nvim/commit/b1a63fea34e630f73e84dff21d3c4b0097f6afd4))
* **commands:** reuse close_command for deleting commands ([#582](https://github.com/ofseed/bufferline.nvim/issues/582)) ([94a89ef](https://github.com/ofseed/bufferline.nvim/commit/94a89ef6198d9c489eb2138c635cdb4926ff74b2))
* **config:** add more detail to the deprecation message ([8fa9921](https://github.com/ofseed/bufferline.nvim/commit/8fa9921fe6878358c6f77f89e9941d20aafeccc8))
* **config:** add numbers highlight ([#366](https://github.com/ofseed/bufferline.nvim/issues/366)) ([30ccdd0](https://github.com/ofseed/bufferline.nvim/commit/30ccdd04eaa729a1c2921db70a40e7b97ef54087))
* **config:** add themeable option ([#329](https://github.com/ofseed/bufferline.nvim/issues/329)) ([2dca4a7](https://github.com/ofseed/bufferline.nvim/commit/2dca4a752dbd51b0ecb05da20933c76cc26efac8))
* **config:** add underline indicator style ([#514](https://github.com/ofseed/bufferline.nvim/issues/514)) ([df6c56a](https://github.com/ofseed/bufferline.nvim/commit/df6c56a2f275f3796ad9fbd7ce7a97bbece9b86d))
* **config:** allow specifying style presets ([13cb114](https://github.com/ofseed/bufferline.nvim/commit/13cb114e91c17238aaa271746aaeb8e967f350a2))
* **config:** ensure the config structure is correct ([408a094](https://github.com/ofseed/bufferline.nvim/commit/408a0945ddf264ccdf59fc6a5fa59507a0ff063b))
* **diag:** add `diagnostics_update_on_event` option ([#932](https://github.com/ofseed/bufferline.nvim/issues/932)) ([aa16daf](https://github.com/ofseed/bufferline.nvim/commit/aa16dafdc642594c7ade7e88d31a6119feb189d6))
* **diagnostics:** support coc as source ([#216](https://github.com/ofseed/bufferline.nvim/issues/216)) ([5d1a589](https://github.com/ofseed/bufferline.nvim/commit/5d1a589b9c1ebcf8f167ae30455c49eafa8e3e3c))
* **diag:** sane fallback to underline color ([0cd505b](https://github.com/ofseed/bufferline.nvim/commit/0cd505b333151e883cdd854539e5eae0e4f3e339))
* **duplicates:** handle identical buffers ([#501](https://github.com/ofseed/bufferline.nvim/issues/501)) ([e5e1c16](https://github.com/ofseed/bufferline.nvim/commit/e5e1c16f11a0715df0ab4e7c73f0174e89e2e383))
* **duplicates:** only treat as duplicate if in the same group ([#750](https://github.com/ofseed/bufferline.nvim/issues/750)) ([66949d0](https://github.com/ofseed/bufferline.nvim/commit/66949d0468b311e37fa815713c0c330e4da34243))
* **duplicates:** toggle unique buffer name ([#469](https://github.com/ofseed/bufferline.nvim/issues/469)) ([#556](https://github.com/ofseed/bufferline.nvim/issues/556)) ([1b605a3](https://github.com/ofseed/bufferline.nvim/commit/1b605a34e9cd596f796a8ac80d207d32010e1821))
* execute user function against visible buffers ([#169](https://github.com/ofseed/bufferline.nvim/issues/169)) ([d343bc3](https://github.com/ofseed/bufferline.nvim/commit/d343bc322e00e9b21bcb9b3c8bf6a989b64a92a2))
* go_to_buffer(-1) opens last buffer ([#471](https://github.com/ofseed/bufferline.nvim/issues/471)) ([8bfe81d](https://github.com/ofseed/bufferline.nvim/commit/8bfe81da99984de947ad27d23e32352b5b9a4416))
* **groups:** close and unpin ([#698](https://github.com/ofseed/bufferline.nvim/issues/698)) ([52241b5](https://github.com/ofseed/bufferline.nvim/commit/52241b57ed41c2283020c6c79ef48fc7cd808bea))
* **groups:** derive pill colors from fg highlight ([9427857](https://github.com/ofseed/bufferline.nvim/commit/9427857e2fdc8127df3bc66ab1338a8ebb549e71))
* **groups:** persist pinned buffers between sessions ([3628e4d](https://github.com/ofseed/bufferline.nvim/commit/3628e4d32dccd3ecb4bfee9d65bfcbab96ee8b72))
* **hover:** show buffer close icons on hover ([#539](https://github.com/ofseed/bufferline.nvim/issues/539)) ([1a199c3](https://github.com/ofseed/bufferline.nvim/commit/1a199c306e6f44bfbf54108503abb0a2d33d7bf5))
* **icons:** add `get_element_icon` option ([#686](https://github.com/ofseed/bufferline.nvim/issues/686)) ([9d95a6d](https://github.com/ofseed/bufferline.nvim/commit/9d95a6de91d83a7dd8559d2897082e89a85d5814))
* insert new buffers after current ([#342](https://github.com/ofseed/bufferline.nvim/issues/342)) ([5c72485](https://github.com/ofseed/bufferline.nvim/commit/5c724853ff1ae2041b9c817284a77d0dd44e9ce9))
* let commands "BufferLineCloseRight" and "BufferLineCloseRight" skip unwritten buffers without a bang ([78a65d2](https://github.com/ofseed/bufferline.nvim/commit/78a65d2d207553b0ce3d1e524e3f4e65a752cda4))
* **offset:** add optional offset win separator ([#515](https://github.com/ofseed/bufferline.nvim/issues/515)) ([04ea8a7](https://github.com/ofseed/bufferline.nvim/commit/04ea8a72381993a5d4a5b938d7c1ae5698b15016))
* **offset:** handle left or right aligned separator ([c6d980b](https://github.com/ofseed/bufferline.nvim/commit/c6d980bc1d817775ee262963b757d662d21cbf4e))
* Support `name_formatter` for unnamed buffers ([#806](https://github.com/ofseed/bufferline.nvim/issues/806)) ([9961d87](https://github.com/ofseed/bufferline.nvim/commit/9961d87bb3ec008213c46ba14b3f384a5f520eb5))
* support vertical split window offsets ([#173](https://github.com/ofseed/bufferline.nvim/issues/173)) ([93e3ee6](https://github.com/ofseed/bufferline.nvim/commit/93e3ee6848a814717c060e76fe0abb4e6b7984ba))
* **tabpages:** add custom_filter ([#400](https://github.com/ofseed/bufferline.nvim/issues/400)) ([1c8e845](https://github.com/ofseed/bufferline.nvim/commit/1c8e845389cd109621c2214a2afff75007457509))
* **tabpages:** add name_formatter ([#455](https://github.com/ofseed/bufferline.nvim/issues/455)) ([88c742f](https://github.com/ofseed/bufferline.nvim/commit/88c742f4af988c98aee5ac1c92f056905c636aae))
* **tabpages:** pass the bufnr to the `name_formatter` ([#941](https://github.com/ofseed/bufferline.nvim/issues/941)) ([28e347d](https://github.com/ofseed/bufferline.nvim/commit/28e347dbc6d0e8367ea56fb045fb9d135579ff79))
* **tabpages:** support unique tab names ([#485](https://github.com/ofseed/bufferline.nvim/issues/485)) ([c4dd9b4](https://github.com/ofseed/bufferline.nvim/commit/c4dd9b4de03b891f648b098c25e4dc1bc48a13e5))
* **tabs:** allow moving/reordering tabs ([#588](https://github.com/ofseed/bufferline.nvim/issues/588)) ([b4db22d](https://github.com/ofseed/bufferline.nvim/commit/b4db22d86fcc08e774b6208d0eb8bd59fc521bb0))
* **tabs:** pass buffers IDs to name_formatter ([#548](https://github.com/ofseed/bufferline.nvim/issues/548)) ([feddbae](https://github.com/ofseed/bufferline.nvim/commit/feddbae5ddd3b02337982a3a7e3708a79dfb4e43))
* **tabs:** sort by tab number instead of tab id ([#592](https://github.com/ofseed/bufferline.nvim/issues/592)) ([d358641](https://github.com/ofseed/bufferline.nvim/commit/d3586411499cc9abf862a5b170e37cc09c073c64))
* **tabs:** use separators matching current style ([#714](https://github.com/ofseed/bufferline.nvim/issues/714)) ([fafc5d2](https://github.com/ofseed/bufferline.nvim/commit/fafc5d28a9a2b36cf8baf10150c05b803e0a8108))
* **ui:** add `padded_slope` style ([#739](https://github.com/ofseed/bufferline.nvim/issues/739)) ([f336811](https://github.com/ofseed/bufferline.nvim/commit/f336811168e04362dfceb51b7e992dfd6ae4e78e))
* **ui:** pass formatter opts to icon fetcher as well ([802bd6b](https://github.com/ofseed/bufferline.nvim/commit/802bd6bdf07dec84525463c904f034bb76a61eec))
* **ui:** tab renaming ([#848](https://github.com/ofseed/bufferline.nvim/issues/848)) ([f2e6c86](https://github.com/ofseed/bufferline.nvim/commit/f2e6c86975deb0f4594d671b7f31c379802491d3))
* **ui:** trunc marker highlights ([#781](https://github.com/ofseed/bufferline.nvim/issues/781)) ([77779e3](https://github.com/ofseed/bufferline.nvim/commit/77779e34d673dd41244b710c22fb18bbfa4c455f)), closes [#792](https://github.com/ofseed/bufferline.nvim/issues/792)
* **utils:** get icon by filetype ([d545bf8](https://github.com/ofseed/bufferline.nvim/commit/d545bf8493c26aca0aeeddfd38795f3b4a98b90f))


### Bug Fixes

* 0.6.1 diagnostic deprecation warning [#285](https://github.com/ofseed/bufferline.nvim/issues/285) ([#286](https://github.com/ofseed/bufferline.nvim/issues/286)) ([d26d1fa](https://github.com/ofseed/bufferline.nvim/commit/d26d1fa89e8163301085ee2321e87c708dd726e9))
* always_show_bufferline should work in tabs mode ([#372](https://github.com/ofseed/bufferline.nvim/issues/372)) ([bb3ac30](https://github.com/ofseed/bufferline.nvim/commit/bb3ac3053f65f03b997b4f21ef37f4e7249389c3))
* **bufferline:** prevent cycling to closed buffers ([#360](https://github.com/ofseed/bufferline.nvim/issues/360)) ([49b007f](https://github.com/ofseed/bufferline.nvim/commit/49b007fa53f7507ca38701d8be72b14aea32faa4))
* **buffers:** use entire path for buffers ([8a3107c](https://github.com/ofseed/bufferline.nvim/commit/8a3107c13dc9fb41429e114bb4d5a6016cf90423))
* **color:** follow linked hl groups ([e6e7cc4](https://github.com/ofseed/bufferline.nvim/commit/e6e7cc454fa28304246e97a9acfe7c6cf2adc5d6))
* **commands:** correct references to click handlers ([a40f058](https://github.com/ofseed/bufferline.nvim/commit/a40f058c6284855ad6a8b8137b3e312beca4d6aa))
* **commands:** potential nil access ([#821](https://github.com/ofseed/bufferline.nvim/issues/821)) ([6e96fa2](https://github.com/ofseed/bufferline.nvim/commit/6e96fa27a0d4dd6c00a252b51c0b43b9b95cd302))
* **commands:** trigger redraw after buffer delete ([5f5b0db](https://github.com/ofseed/bufferline.nvim/commit/5f5b0db4171c2f8a96f02f89c86aa2e0886cc327))
* **commands:** trigger redraw after delete in direction ([#587](https://github.com/ofseed/bufferline.nvim/issues/587)) ([584e4a0](https://github.com/ofseed/bufferline.nvim/commit/584e4a000845b52a5dce1b437b8280410b13ee2f))
* **config:** deep copy user highlights ([97c6171](https://github.com/ofseed/bufferline.nvim/commit/97c6171f834cb98cafd61def0ceb3f1fc1001fbe))
* **config:** highlighting for tab separators ([#784](https://github.com/ofseed/bufferline.nvim/issues/784)) ([cd27a52](https://github.com/ofseed/bufferline.nvim/commit/cd27a52ecdfed7f14a41b61b7976f155e3d593c7))
* **config:** remove mappings field from defaults ([#403](https://github.com/ofseed/bufferline.nvim/issues/403)) ([61d93da](https://github.com/ofseed/bufferline.nvim/commit/61d93dac3cbc20c6fba4d6491968ed4d0f7631c9)), closes [#402](https://github.com/ofseed/bufferline.nvim/issues/402)
* **config:** update lsp highlights to support 0.6 ([782fab8](https://github.com/ofseed/bufferline.nvim/commit/782fab8a2352e872dc991c42f806dae18e848b2d)), closes [#245](https://github.com/ofseed/bufferline.nvim/issues/245)
* convert user config highlights before merging ([#222](https://github.com/ofseed/bufferline.nvim/issues/222)) ([1592327](https://github.com/ofseed/bufferline.nvim/commit/15923279b719ce77911caf34e5f4c83a0b5397c9))
* correctly pad buffers without close icons ([188af0f](https://github.com/ofseed/bufferline.nvim/commit/188af0fe62a74316fe24f7c154ed0e1717ea8a82)), closes [#217](https://github.com/ofseed/bufferline.nvim/issues/217)
* correctly re-export and document exec function([#373](https://github.com/ofseed/bufferline.nvim/issues/373)) ([7634b89](https://github.com/ofseed/bufferline.nvim/commit/7634b89bb513dffb70e0a41a060a94239d6db2db))
* custom area background highlight ([#537](https://github.com/ofseed/bufferline.nvim/issues/537)) ([0b4b863](https://github.com/ofseed/bufferline.nvim/commit/0b4b863244ef1369a8b9e4246dc95f8cdb5db026))
* **diagnostics:** don't add indicator if empty ([d8362e6](https://github.com/ofseed/bufferline.nvim/commit/d8362e65e00e926d52e74a67ffa8b177736e5c99))
* **diagnostics:** ignore disabled diagnostics ([#816](https://github.com/ofseed/bufferline.nvim/issues/816)) ([8a51c4b](https://github.com/ofseed/bufferline.nvim/commit/8a51c4b5d105d93fd2bc435bf93d4d5556fb2a60))
* **docs:** correct name for buffer id on numbers section ([#212](https://github.com/ofseed/bufferline.nvim/issues/212)) ([50f8112](https://github.com/ofseed/bufferline.nvim/commit/50f81127d44b374871c628b3c2889c3e4c16b775))
* **docs:** document hl groups for tab numbers ([#508](https://github.com/ofseed/bufferline.nvim/issues/508)) ([839c1f9](https://github.com/ofseed/bufferline.nvim/commit/839c1f9b0fca407d96d9d161b4404ab14f3d0e18))
* **docs:** tiny typo ([#509](https://github.com/ofseed/bufferline.nvim/issues/509)) ([f5791fd](https://github.com/ofseed/bufferline.nvim/commit/f5791fdd561c564491563cd4139727c38d135dbf))
* **docs:** use correct value for style presets ([#747](https://github.com/ofseed/bufferline.nvim/issues/747)) ([9eed863](https://github.com/ofseed/bufferline.nvim/commit/9eed86350dcb4a5cca13056d0d16ba85e20e5024))
* **duplicates:** remove extra trunc marker ([29d5789](https://github.com/ofseed/bufferline.nvim/commit/29d5789aa407e7105968c43dba566defd3ca96bd))
* **duplicates:** return buffer if it has no path ([c25d4f8](https://github.com/ofseed/bufferline.nvim/commit/c25d4f8079a6e58520891f58121775903b439604)), closes [#202](https://github.com/ofseed/bufferline.nvim/issues/202)
* **duplicates:** use utils.truncate_name to truncate ancestors ([#414](https://github.com/ofseed/bufferline.nvim/issues/414)) ([ee1d51e](https://github.com/ofseed/bufferline.nvim/commit/ee1d51e44ce361b4a037ca5fbbb27f270d3ea03c))
* freeze with miniscule truncation values ([#507](https://github.com/ofseed/bufferline.nvim/issues/507)) ([05db7ec](https://github.com/ofseed/bufferline.nvim/commit/05db7ec6bc1ffa0ada6d535b80d8f673a237f446))
* **group:** check that group exists before operating on it ([#681](https://github.com/ofseed/bufferline.nvim/issues/681)) ([f9239e4](https://github.com/ofseed/bufferline.nvim/commit/f9239e4dce203256a0e7416d54ca606f7481ac07))
* **groups:** assign priority based on if pinned specified ([#380](https://github.com/ofseed/bufferline.nvim/issues/380)) ([a01b48a](https://github.com/ofseed/bufferline.nvim/commit/a01b48a206315340efb8475e18f2c5fa070195fe))
* **groups:** clear unpinned buffers from session ([#688](https://github.com/ofseed/bufferline.nvim/issues/688)) ([6dbb3d4](https://github.com/ofseed/bufferline.nvim/commit/6dbb3d44a6149b1919f7b13e117416fb18f0814b))
* **groups:** correctly determine is pinned is set ([4917220](https://github.com/ofseed/bufferline.nvim/commit/49172206754f7ee0f3ac1b461bbac1a357cd0879))
* **groups:** correctly reset group highlights ([4fb5824](https://github.com/ofseed/bufferline.nvim/commit/4fb58244f15e9e5bb530db248c99021c8eb089e9))
* **groups:** don't exit early if persisted buffer is invalid ([a448b1c](https://github.com/ofseed/bufferline.nvim/commit/a448b1cbf02afd85538335499fec7837a9c68b61))
* **groups:** ensure groups are persisted correctly ([#693](https://github.com/ofseed/bufferline.nvim/issues/693)) ([894d0e8](https://github.com/ofseed/bufferline.nvim/commit/894d0e80583cacd27facdb6676a6b08764662537))
* **groups:** ensure highlights are set for all groups ([45ebe7b](https://github.com/ofseed/bufferline.nvim/commit/45ebe7bf38bbf5bcea260c8b1fda9cdd2690227f))
* **groups:** highlights should extend to deduplication ([87b2799](https://github.com/ofseed/bufferline.nvim/commit/87b2799090705cc07858497a06876251716abe0c))
* **groups:** increase padding for tab separator ([95397d6](https://github.com/ofseed/bufferline.nvim/commit/95397d6ccf62144b0b6341b4b022ae6e386ee7ec))
* **groups:** only apply group highlight to matching buffers ([3228948](https://github.com/ofseed/bufferline.nvim/commit/3228948e8a8fd08e422b74e496c9218d1ea3a993))
* **groups:** only extend if there are highlights ([c1816cb](https://github.com/ofseed/bufferline.nvim/commit/c1816cb4082d234af0a48138ed1369bc091f481f))
* **groups:** only reset the pinned group if it closed ([#696](https://github.com/ofseed/bufferline.nvim/issues/696)) ([2c232bf](https://github.com/ofseed/bufferline.nvim/commit/2c232bf5c19017b4cd97417098b88f5175b02efc))
* **groups:** re-enable clicking groups ([61da3cf](https://github.com/ofseed/bufferline.nvim/commit/61da3cfd1b9622b0ea1fd2fbc5160fd0216411ea)), closes [#341](https://github.com/ofseed/bufferline.nvim/issues/341)
* **groups:** refresh the UI when a group is closed ([#682](https://github.com/ofseed/bufferline.nvim/issues/682)) ([504d2ff](https://github.com/ofseed/bufferline.nvim/commit/504d2ff50017764e8bb1bc31faa092cdeacab013))
* **groups:** tab separator should take group ([3f85527](https://github.com/ofseed/bufferline.nvim/commit/3f855273cab29967bc454d3474224042815dd175))
* **groups:** typo in indicator segment highlight ([e450afe](https://github.com/ofseed/bufferline.nvim/commit/e450afeee6ce6abee89b3c26db64ae93b378019d)), closes [#578](https://github.com/ofseed/bufferline.nvim/issues/578)
* **groups:** use correct cmdline completion function ([a4bd445](https://github.com/ofseed/bufferline.nvim/commit/a4bd44523316928a7c4a5c09a3407d02c30b6027))
* **groups:** use correct name for indicator hl ([6211520](https://github.com/ofseed/bufferline.nvim/commit/6211520e6f4d8f312a448b92e57c6d52f1fde407))
* **groups:** use formatted name to create hls ([81033e9](https://github.com/ofseed/bufferline.nvim/commit/81033e9691690a649fd807fbe86b6af7c535bdf8))
* **highlights:** allow setting GUI attributes to NONE ([#432](https://github.com/ofseed/bufferline.nvim/issues/432)) ([f92df91](https://github.com/ofseed/bufferline.nvim/commit/f92df91d6fe4d1d6b94e404e0fad7feac2c59c60))
* **highlights:** decouple default from themeable ([dfebbd0](https://github.com/ofseed/bufferline.nvim/commit/dfebbd01ca9005b0514aab4d4452428a9de41ce2))
* **highlights:** if color_icons is false set to NONE ([8b32447](https://github.com/ofseed/bufferline.nvim/commit/8b32447f1ba00f71ec2ebb413249d1d84228d9fb)), closes [#702](https://github.com/ofseed/bufferline.nvim/issues/702)
* **highlights:** only set cterm values if not termguicolors ([ee7b723](https://github.com/ofseed/bufferline.nvim/commit/ee7b72329a1660f5ce6322030bc3379347789c00))
* **highlights:** preserve original user config ([1f5eed0](https://github.com/ofseed/bufferline.nvim/commit/1f5eed03474d1d081dc15c8b0a967ea4d9809df9))
* **highlights:** set default whilst setting highlight ([f3eb69f](https://github.com/ofseed/bufferline.nvim/commit/f3eb69f572aaea710e5939036bb8848b88a3d988))
* **highlights:** underline colors should be picked up ([4836975](https://github.com/ofseed/bufferline.nvim/commit/4836975de26134444448b6447bf66358b1b9cc4b))
* **highlights:** use correct background ([5b28eaf](https://github.com/ofseed/bufferline.nvim/commit/5b28eafb0e560f71c2fc5c03426b3720329c9e90))
* **hover:** check showtabline not laststatus ([#616](https://github.com/ofseed/bufferline.nvim/issues/616)) ([4ecfa81](https://github.com/ofseed/bufferline.nvim/commit/4ecfa81e470a589e74adcde3d5bb1727dd407363))
* **hover:** error wrap getting the mouse position ([2405c06](https://github.com/ofseed/bufferline.nvim/commit/2405c06d3e9598a6fb4f63ace1f1ba9ce3860956))
* **icons:** display overriden devicons ([#817](https://github.com/ofseed/bufferline.nvim/issues/817)) ([81cd04f](https://github.com/ofseed/bufferline.nvim/commit/81cd04fe7c914d020d331cea1e707da5f14c2665))
* improve handling of directory buffers ([be5866b](https://github.com/ofseed/bufferline.nvim/commit/be5866b77c713d92cf3d383a387bec1d55e3f798))
* maintain backwards compatibility ([#909](https://github.com/ofseed/bufferline.nvim/issues/909)) ([155b257](https://github.com/ofseed/bufferline.nvim/commit/155b257b0c1d7999b0ffc837e1dd3a110cdc33d0))
* merge current buffer hls with groups ([94211ea](https://github.com/ofseed/bufferline.nvim/commit/94211eac27c931f4458ce713fbe430b7cc82dea8))
* missing visibility method on TabPage ([#354](https://github.com/ofseed/bufferline.nvim/issues/354)) ([004cd57](https://github.com/ofseed/bufferline.nvim/commit/004cd5734fb21e39d48c1fb1469fa63e2797880b))
* move early return when not showing tabline ([f63be9a](https://github.com/ofseed/bufferline.nvim/commit/f63be9a3a3429a726af14c9085d547281bdf38cc)), closes [#338](https://github.com/ofseed/bufferline.nvim/issues/338) [#337](https://github.com/ofseed/bufferline.nvim/issues/337)
* **offset:** do not add trunc marker to empty offset ([1235fa3](https://github.com/ofseed/bufferline.nvim/commit/1235fa34049b7ece6e4acf814521541a29513a26))
* **offset:** handle COLUMN layout types ([#657](https://github.com/ofseed/bufferline.nvim/issues/657)) ([b02041a](https://github.com/ofseed/bufferline.nvim/commit/b02041a16bf37f13c3802223bad35aee8cfcf3b5))
* **offset:** Search winhl in reverse order when guessing hl. ([#234](https://github.com/ofseed/bufferline.nvim/issues/234)) ([729e900](https://github.com/ofseed/bufferline.nvim/commit/729e90094cf444d69d1dbfd52a98806d900972f4))
* **offsets:** only use nvim eval statusline in nightly ([d5904e8](https://github.com/ofseed/bufferline.nvim/commit/d5904e8a3434acb151a4948b1b3d4760a2a12bb1))
* **offsets:** use nvim_eval_statusline to calculate the size ([#333](https://github.com/ofseed/bufferline.nvim/issues/333)) ([4269835](https://github.com/ofseed/bufferline.nvim/commit/4269835d2d02f4bbf4c69235be3bae56ee8ebf93))
* **offset:** truncate long offset text with multibyte characters ([#503](https://github.com/ofseed/bufferline.nvim/issues/503)) ([4d28b3c](https://github.com/ofseed/bufferline.nvim/commit/4d28b3ca15c14a328b08b5935dbd2632862611d8))
* only notify once if version is outdated ([f343a17](https://github.com/ofseed/bufferline.nvim/commit/f343a17cd014de16ef193f52fdeaa95be7951b07))
* **pick:** error handle &lt;c-c&gt; keyboard interrupts ([7783c2a](https://github.com/ofseed/bufferline.nvim/commit/7783c2ac40c7dbfa5fa3e4dbc7d0c640019bd5fb))
* **pick:** error handle &lt;c-c&gt; keyboard interrupts ([374ef05](https://github.com/ofseed/bufferline.nvim/commit/374ef05019bf4708e12cd20a135b4766cf0cf9a5))
* **pick:** measure correct letter variable ([f400745](https://github.com/ofseed/bufferline.nvim/commit/f400745691834ab04b9ba24217c9e9e1a3ada55f))
* **pick:** swap padding values buffer icon ([0d673a0](https://github.com/ofseed/bufferline.nvim/commit/0d673a07308f94b582f4ec0ac3dcb4a6bf3b1476))
* re-apply user overrides on scheme change ([65a2431](https://github.com/ofseed/bufferline.nvim/commit/65a24314a2ace829356a3b7e5c791ef3e19c9ed9))
* **readme:** correct name for buffer id on numbers section ([#214](https://github.com/ofseed/bufferline.nvim/issues/214)) ([bede234](https://github.com/ofseed/bufferline.nvim/commit/bede234e1036ab04dd6c6caf3bd7f9ed1d194c3c))
* **README:** replace deprecated api ([#303](https://github.com/ofseed/bufferline.nvim/issues/303)) ([00a9820](https://github.com/ofseed/bufferline.nvim/commit/00a98203a38dd38b670aa70ef965c4e9be5573ef))
* **readme:** Typo ([#793](https://github.com/ofseed/bufferline.nvim/issues/793)) ([99f0932](https://github.com/ofseed/bufferline.nvim/commit/99f0932365b34e22549ff58e1bea388465d15e99))
* reimplement the deprecated function tbl_add_reverse_lookup ([#904](https://github.com/ofseed/bufferline.nvim/issues/904)) ([9ae49d7](https://github.com/ofseed/bufferline.nvim/commit/9ae49d71c84b42b91795f7b7cead223c6346e774))
* remove `missing required fields` diagnostic from config ([#812](https://github.com/ofseed/bufferline.nvim/issues/812)) ([1a33975](https://github.com/ofseed/bufferline.nvim/commit/1a3397556d194bb1f2cc530b07124ccc512c5501))
* remove unintentional usages of string.len ([9d8bf06](https://github.com/ofseed/bufferline.nvim/commit/9d8bf067012fa02ea0e966de316b92d706253369))
* replace tbl_flatten to flatten():totable() ([#912](https://github.com/ofseed/bufferline.nvim/issues/912)) ([b2dc003](https://github.com/ofseed/bufferline.nvim/commit/b2dc003aca1dc638ccc3e7752ab3969b4184a690))
* skip invalid regex in truncate_name ([#841](https://github.com/ofseed/bufferline.nvim/issues/841)) ([ac788fb](https://github.com/ofseed/bufferline.nvim/commit/ac788fbc493839c1e76daa8d119934b715fdb90e))
* **sorters.lua:** reference the correct sort func ([cb9bd12](https://github.com/ofseed/bufferline.nvim/commit/cb9bd12875d1a75c706a2f0ab62a460b5250528c)), closes [#344](https://github.com/ofseed/bufferline.nvim/issues/344)
* **sorters.lua:** reference the correct sort func ([e1202c6](https://github.com/ofseed/bufferline.nvim/commit/e1202c6569353d03ef0cb3da11b839dba26854dd)), closes [#344](https://github.com/ofseed/bufferline.nvim/issues/344)
* **sorters:** handle nil buffers in id sorter ([871495d](https://github.com/ofseed/bufferline.nvim/commit/871495d9e2dbe3314a421fd2d5e46f47de7ee537)), closes [#324](https://github.com/ofseed/bufferline.nvim/issues/324)
* **sorters:** insert_after_current strategy ([1620cfe](https://github.com/ofseed/bufferline.nvim/commit/1620cfe8f226b49bfc4886a092449f565b4d84ab))
* **sorters:** invert sorting for insert at end ([8c79861](https://github.com/ofseed/bufferline.nvim/commit/8c79861742c513481f51f3f6c6a4002d5d5d39da))
* store paths in g:BufferlinePositions ([#780](https://github.com/ofseed/bufferline.nvim/issues/780)) ([2f391fd](https://github.com/ofseed/bufferline.nvim/commit/2f391fde91b9c3876eee359ee24cc352050e5e48))
* **tabpages:** renaming bug on reopened tab ([#877](https://github.com/ofseed/bufferline.nvim/issues/877)) ([1064399](https://github.com/ofseed/bufferline.nvim/commit/10643990c33ca295bfe970d775c6e7697354aa0f))
* **tabpages:** typo in rename_tab ([#873](https://github.com/ofseed/bufferline.nvim/issues/873)) ([5bf13d1](https://github.com/ofseed/bufferline.nvim/commit/5bf13d17a8c8abbce8d3ef83c8658b32e08ce913))
* **tabpages:** use tabpagenr for closing tabpages ([#465](https://github.com/ofseed/bufferline.nvim/issues/465)) ([0652db6](https://github.com/ofseed/bufferline.nvim/commit/0652db63345454701bfb8ed7705546c177bc4ef2))
* **tabs:** explicitly convert segments text attribute to string ([#442](https://github.com/ofseed/bufferline.nvim/issues/442)) ([4b10426](https://github.com/ofseed/bufferline.nvim/commit/4b1042653edaf536990374075e4c59aaa4f2f10d))
* **tabs:** re-add incorrectly removed method ([2e5d92e](https://github.com/ofseed/bufferline.nvim/commit/2e5d92efacf40d488c4647a9e3e5100357b184cf))
* **tabs:** show unnamed buffers ([#613](https://github.com/ofseed/bufferline.nvim/issues/613)) ([65465b4](https://github.com/ofseed/bufferline.nvim/commit/65465b431576bc58618c8223ae501196f9078dac))
* **tabs:** use custom separator_style in tabpages ([#852](https://github.com/ofseed/bufferline.nvim/issues/852)) ([81820ca](https://github.com/ofseed/bufferline.nvim/commit/81820cac7c85e51e4cf179f8a66d13dbf7b032d9))
* truncate multibyte characters by cell ([#180](https://github.com/ofseed/bufferline.nvim/issues/180)) ([067ec55](https://github.com/ofseed/bufferline.nvim/commit/067ec55a10ef8a58f8c7b45621daca759ab54437))
* **truncation:** handle multibyte characters ([5c82307](https://github.com/ofseed/bufferline.nvim/commit/5c82307c64143ed2848e6ea1777ee51a40d3b978))
* **ui:** adjust hover position using tabline offset ([8c895e9](https://github.com/ofseed/bufferline.nvim/commit/8c895e971a39ba40554bac2ca9547d961db0ba29))
* **ui:** always schedule refreshing ([fe77474](https://github.com/ofseed/bufferline.nvim/commit/fe774743cc7434d8f5539093108bf7d6d950f416))
* **ui:** create proper icon highlights for bufferline ([46cfe4c](https://github.com/ofseed/bufferline.nvim/commit/46cfe4c87e03a10854e4c88bf1aa5867183e32b5))
* **ui:** extension logic should be correctly applied ([#423](https://github.com/ofseed/bufferline.nvim/issues/423)) ([be45195](https://github.com/ofseed/bufferline.nvim/commit/be451957bab8689106a72f0ec42f3fc0bedee5d6))
* **ui:** icons should inherit all of the buffer highlights ([15e2e33](https://github.com/ofseed/bufferline.nvim/commit/15e2e338de15911da2accffb55be2db120016e8c))
* **ui:** return correct empty value from truncation ([60d8f4d](https://github.com/ofseed/bufferline.nvim/commit/60d8f4d44372cf273e93c450945a852166567e6b))
* **ui:** Use correct function to check for list ([#726](https://github.com/ofseed/bufferline.nvim/issues/726)) ([dd86c31](https://github.com/ofseed/bufferline.nvim/commit/dd86c312fd225549ac02567d47570c04ba456402))
* UNKNOWN PLUGIN error resulting from unloaded buffers ([#928](https://github.com/ofseed/bufferline.nvim/issues/928)) ([6ac7e4f](https://github.com/ofseed/bufferline.nvim/commit/6ac7e4f1eead72507cfdbc94dcd0c26b98b2f86e))
* UNKNOWN PLUGIN error resulting from unloaded buffers ([#931](https://github.com/ofseed/bufferline.nvim/issues/931)) ([1662fed](https://github.com/ofseed/bufferline.nvim/commit/1662fed6ecd512d1f381fc2a4e77532c379d25c6))
* update highlights on colorscheme change ([37587b6](https://github.com/ofseed/bufferline.nvim/commit/37587b699020b7eee93cf2c4cd556451b7d7a866)), closes [#218](https://github.com/ofseed/bufferline.nvim/issues/218)
* use link if specified in custom areas ([#839](https://github.com/ofseed/bufferline.nvim/issues/839)) ([9ca364d](https://github.com/ofseed/bufferline.nvim/commit/9ca364d488b98894ca780c40aae9ea63967c8fcf))
* use vim.diagnostic.get instead of vim.lsp.diagnostic.get_all ([#272](https://github.com/ofseed/bufferline.nvim/issues/272)) ([b7afa98](https://github.com/ofseed/bufferline.nvim/commit/b7afa98f00145c2a35b6bb97cfde95f272a0f9b3))
* **utils:** detect if a buffer filetype is empty ([4443b2a](https://github.com/ofseed/bufferline.nvim/commit/4443b2af3df764ef4b6411efbb356dcffe7a2142))
* **utils:** fix utils.is_list ([#728](https://github.com/ofseed/bufferline.nvim/issues/728)) ([2c8d615](https://github.com/ofseed/bufferline.nvim/commit/2c8d615c47a5013b24b3b4bdebec2fda1b38cdd9))
* **utils:** improve debug logging ([09d3098](https://github.com/ofseed/bufferline.nvim/commit/09d3098500e34bc6eaffb675ab2ab5c6e904e976))
* **utils:** improve path separator detection on windows ([#519](https://github.com/ofseed/bufferline.nvim/issues/519)) ([5a755ea](https://github.com/ofseed/bufferline.nvim/commit/5a755ea88752af31684f5ac88074c2ae12964a6d))
* **utils:** improve path separator detection on Windows ([#888](https://github.com/ofseed/bufferline.nvim/issues/888)) ([d7ebc0d](https://github.com/ofseed/bufferline.nvim/commit/d7ebc0de62a2f752dcd3cadf6f3235a0702f15a3))
* **utils:** specify opts for notify helper ([874f869](https://github.com/ofseed/bufferline.nvim/commit/874f869a24e568980294b3200fc9dd842db65a36)), closes [#364](https://github.com/ofseed/bufferline.nvim/issues/364)
* **utils:** update is_list to handle breaking change ([#892](https://github.com/ofseed/bufferline.nvim/issues/892)) ([a6ad228](https://github.com/ofseed/bufferline.nvim/commit/a6ad228f77c276a4324924a6899cbfad70541547))
* vim.diagnostic.is_disabled() deprecation warning ([#907](https://github.com/ofseed/bufferline.nvim/issues/907)) ([2cd3984](https://github.com/ofseed/bufferline.nvim/commit/2cd39842c6426fb6c9a79fa57420121cc81c9804))


### Performance Improvements

* **coc-diagnostics:** use event `CocDiagnosticChange` ([#323](https://github.com/ofseed/bufferline.nvim/issues/323)) ([e97a404](https://github.com/ofseed/bufferline.nvim/commit/e97a404bd7449ecebab243c796c1016c98397fc0))
* **ui:** avoid (some) expensive functions ([#754](https://github.com/ofseed/bufferline.nvim/issues/754)) ([018bdf6](https://github.com/ofseed/bufferline.nvim/commit/018bdf61a97e00caeff05d16977437c63018762e))


### Reverts

* remove fix for referencing unloaded buffers ([#930](https://github.com/ofseed/bufferline.nvim/issues/930)) ([46192e7](https://github.com/ofseed/bufferline.nvim/commit/46192e794b73f92136326c10ecdbdbf15e35705f))
* **tabs:** allow moving/reordering tabs ([#588](https://github.com/ofseed/bufferline.nvim/issues/588)) ([#590](https://github.com/ofseed/bufferline.nvim/issues/590)) ([dc1d4e5](https://github.com/ofseed/bufferline.nvim/commit/dc1d4e500f18ab9d7b311b6f298f6758c3abcfaf))


### Miscellaneous Chores

* **diagnostics:** remove deprecated function ([09c50ba](https://github.com/ofseed/bufferline.nvim/commit/09c50ba679103e0af4a7f35076c5ee645a90875f))


### Code Refactoring

* **config:** deprecate show_buffer_default_icon ([6ccdee8](https://github.com/ofseed/bufferline.nvim/commit/6ccdee8e931503699eb8f92c7faafd0ad1a8cf69))
* **groups:** change argument to group matcher ([38d62b8](https://github.com/ofseed/bufferline.nvim/commit/38d62b8bae62c681d6e259de54421d4155976897))
* **tests:** load dependencies in init.lua ([dea64b9](https://github.com/ofseed/bufferline.nvim/commit/dea64b9ed5b709bbf75b5e952badab78fe697bf1))
* **ui:** Change internal representation of tabline ([#412](https://github.com/ofseed/bufferline.nvim/issues/412)) ([9f2f314](https://github.com/ofseed/bufferline.nvim/commit/9f2f3149444be8976d836ee8d396e4839e64ff72))

## [4.7.0](https://github.com/akinsho/bufferline.nvim/compare/v4.6.1...v4.7.0) (2024-07-10)


### Features

* **diag:** add `diagnostics_update_on_event` option ([#932](https://github.com/akinsho/bufferline.nvim/issues/932)) ([aa16daf](https://github.com/akinsho/bufferline.nvim/commit/aa16dafdc642594c7ade7e88d31a6119feb189d6))


### Bug Fixes

* **tabs:** use custom separator_style in tabpages ([#852](https://github.com/akinsho/bufferline.nvim/issues/852)) ([81820ca](https://github.com/akinsho/bufferline.nvim/commit/81820cac7c85e51e4cf179f8a66d13dbf7b032d9))
* UNKNOWN PLUGIN error resulting from unloaded buffers ([#928](https://github.com/akinsho/bufferline.nvim/issues/928)) ([6ac7e4f](https://github.com/akinsho/bufferline.nvim/commit/6ac7e4f1eead72507cfdbc94dcd0c26b98b2f86e))
* UNKNOWN PLUGIN error resulting from unloaded buffers ([#931](https://github.com/akinsho/bufferline.nvim/issues/931)) ([1662fed](https://github.com/akinsho/bufferline.nvim/commit/1662fed6ecd512d1f381fc2a4e77532c379d25c6))


### Reverts

* remove fix for referencing unloaded buffers ([#930](https://github.com/akinsho/bufferline.nvim/issues/930)) ([46192e7](https://github.com/akinsho/bufferline.nvim/commit/46192e794b73f92136326c10ecdbdbf15e35705f))

## [4.6.1](https://github.com/akinsho/bufferline.nvim/compare/v4.6.0...v4.6.1) (2024-05-21)


### Bug Fixes

* replace tbl_flatten to flatten():totable() ([#912](https://github.com/akinsho/bufferline.nvim/issues/912)) ([b2dc003](https://github.com/akinsho/bufferline.nvim/commit/b2dc003aca1dc638ccc3e7752ab3969b4184a690))

## [4.6.0](https://github.com/akinsho/bufferline.nvim/compare/v4.5.3...v4.6.0) (2024-05-20)


### Features

* add `auto_toggle_bufferline` option ([#876](https://github.com/akinsho/bufferline.nvim/issues/876)) ([f6f00d9](https://github.com/akinsho/bufferline.nvim/commit/f6f00d9ac1a51483ac78418f9e63126119a70709))


### Bug Fixes

* maintain backwards compatibility ([#909](https://github.com/akinsho/bufferline.nvim/issues/909)) ([155b257](https://github.com/akinsho/bufferline.nvim/commit/155b257b0c1d7999b0ffc837e1dd3a110cdc33d0))
* reimplement the deprecated function tbl_add_reverse_lookup ([#904](https://github.com/akinsho/bufferline.nvim/issues/904)) ([9ae49d7](https://github.com/akinsho/bufferline.nvim/commit/9ae49d71c84b42b91795f7b7cead223c6346e774))
* **utils:** update is_list to handle breaking change ([#892](https://github.com/akinsho/bufferline.nvim/issues/892)) ([a6ad228](https://github.com/akinsho/bufferline.nvim/commit/a6ad228f77c276a4324924a6899cbfad70541547))
* vim.diagnostic.is_disabled() deprecation warning ([#907](https://github.com/akinsho/bufferline.nvim/issues/907)) ([2cd3984](https://github.com/akinsho/bufferline.nvim/commit/2cd39842c6426fb6c9a79fa57420121cc81c9804))

## [4.5.3](https://github.com/akinsho/bufferline.nvim/compare/v4.5.2...v4.5.3) (2024-04-19)


### Bug Fixes

* **utils:** improve path separator detection on Windows ([#888](https://github.com/akinsho/bufferline.nvim/issues/888)) ([d7ebc0d](https://github.com/akinsho/bufferline.nvim/commit/d7ebc0de62a2f752dcd3cadf6f3235a0702f15a3))

## [4.5.2](https://github.com/akinsho/bufferline.nvim/compare/v4.5.1...v4.5.2) (2024-03-07)


### Bug Fixes

* **tabpages:** renaming bug on reopened tab ([#877](https://github.com/akinsho/bufferline.nvim/issues/877)) ([1064399](https://github.com/akinsho/bufferline.nvim/commit/10643990c33ca295bfe970d775c6e7697354aa0f))

## [4.5.1](https://github.com/akinsho/bufferline.nvim/compare/v4.5.0...v4.5.1) (2024-03-05)


### Bug Fixes

* **tabpages:** typo in rename_tab ([#873](https://github.com/akinsho/bufferline.nvim/issues/873)) ([5bf13d1](https://github.com/akinsho/bufferline.nvim/commit/5bf13d17a8c8abbce8d3ef83c8658b32e08ce913))

## [4.5.0](https://github.com/akinsho/bufferline.nvim/compare/v4.4.1...v4.5.0) (2024-01-22)


### Features

* **ui:** tab renaming ([#848](https://github.com/akinsho/bufferline.nvim/issues/848)) ([f2e6c86](https://github.com/akinsho/bufferline.nvim/commit/f2e6c86975deb0f4594d671b7f31c379802491d3))


### Bug Fixes

* skip invalid regex in truncate_name ([#841](https://github.com/akinsho/bufferline.nvim/issues/841)) ([ac788fb](https://github.com/akinsho/bufferline.nvim/commit/ac788fbc493839c1e76daa8d119934b715fdb90e))

## [4.4.1](https://github.com/akinsho/bufferline.nvim/compare/v4.4.0...v4.4.1) (2023-12-06)


### Bug Fixes

* **commands:** potential nil access ([#821](https://github.com/akinsho/bufferline.nvim/issues/821)) ([6e96fa2](https://github.com/akinsho/bufferline.nvim/commit/6e96fa27a0d4dd6c00a252b51c0b43b9b95cd302))
* remove `missing required fields` diagnostic from config ([#812](https://github.com/akinsho/bufferline.nvim/issues/812)) ([1a33975](https://github.com/akinsho/bufferline.nvim/commit/1a3397556d194bb1f2cc530b07124ccc512c5501))
* use link if specified in custom areas ([#839](https://github.com/akinsho/bufferline.nvim/issues/839)) ([9ca364d](https://github.com/akinsho/bufferline.nvim/commit/9ca364d488b98894ca780c40aae9ea63967c8fcf))

## [4.4.0](https://github.com/akinsho/bufferline.nvim/compare/v4.3.0...v4.4.0) (2023-09-20)


### Features

* Support `name_formatter` for unnamed buffers ([#806](https://github.com/akinsho/bufferline.nvim/issues/806)) ([9961d87](https://github.com/akinsho/bufferline.nvim/commit/9961d87bb3ec008213c46ba14b3f384a5f520eb5))


### Bug Fixes

* **diagnostics:** ignore disabled diagnostics ([#816](https://github.com/akinsho/bufferline.nvim/issues/816)) ([8a51c4b](https://github.com/akinsho/bufferline.nvim/commit/8a51c4b5d105d93fd2bc435bf93d4d5556fb2a60))
* **icons:** display overriden devicons ([#817](https://github.com/akinsho/bufferline.nvim/issues/817)) ([81cd04f](https://github.com/akinsho/bufferline.nvim/commit/81cd04fe7c914d020d331cea1e707da5f14c2665))
* **readme:** Typo ([#793](https://github.com/akinsho/bufferline.nvim/issues/793)) ([99f0932](https://github.com/akinsho/bufferline.nvim/commit/99f0932365b34e22549ff58e1bea388465d15e99))

## [4.3.0](https://github.com/akinsho/bufferline.nvim/compare/v4.2.0...v4.3.0) (2023-07-17)


### Features

* **command:** add BufferLineCloseOthers command ([#774](https://github.com/akinsho/bufferline.nvim/issues/774)) ([9d6ab3a](https://github.com/akinsho/bufferline.nvim/commit/9d6ab3a56ad71bed9929c7acd7620e827a073d25))
* **ui:** trunc marker highlights ([#781](https://github.com/akinsho/bufferline.nvim/issues/781)) ([77779e3](https://github.com/akinsho/bufferline.nvim/commit/77779e34d673dd41244b710c22fb18bbfa4c455f)), closes [#792](https://github.com/akinsho/bufferline.nvim/issues/792)


### Bug Fixes

* **config:** highlighting for tab separators ([#784](https://github.com/akinsho/bufferline.nvim/issues/784)) ([cd27a52](https://github.com/akinsho/bufferline.nvim/commit/cd27a52ecdfed7f14a41b61b7976f155e3d593c7))
* store paths in g:BufferlinePositions ([#780](https://github.com/akinsho/bufferline.nvim/issues/780)) ([2f391fd](https://github.com/akinsho/bufferline.nvim/commit/2f391fde91b9c3876eee359ee24cc352050e5e48))
* **ui:** always schedule refreshing ([fe77474](https://github.com/akinsho/bufferline.nvim/commit/fe774743cc7434d8f5539093108bf7d6d950f416))

## [4.2.0](https://github.com/akinsho/bufferline.nvim/compare/v4.1.0...v4.2.0) (2023-06-26)


### Features

* **commands/go_to:** go to the last element if index out of bounds ([#758](https://github.com/akinsho/bufferline.nvim/issues/758)) ([6073426](https://github.com/akinsho/bufferline.nvim/commit/60734264a8655a7db3595159fb50076dc24c2f2c))
* **commands:** add option to wrap when moving buffers at ends ([#759](https://github.com/akinsho/bufferline.nvim/issues/759)) ([da1875c](https://github.com/akinsho/bufferline.nvim/commit/da1875c1eee9aa9b7e19cda5c70ed7d7702d5f06))


### Performance Improvements

* **ui:** avoid (some) expensive functions ([#754](https://github.com/akinsho/bufferline.nvim/issues/754)) ([018bdf6](https://github.com/akinsho/bufferline.nvim/commit/018bdf61a97e00caeff05d16977437c63018762e))

## [4.1.0](https://github.com/akinsho/bufferline.nvim/compare/v4.0.0...v4.1.0) (2023-05-03)


### Features

* **ui:** add `padded_slope` style ([#739](https://github.com/akinsho/bufferline.nvim/issues/739)) ([f336811](https://github.com/akinsho/bufferline.nvim/commit/f336811168e04362dfceb51b7e992dfd6ae4e78e))


### Bug Fixes

* **docs:** use correct value for style presets ([#747](https://github.com/akinsho/bufferline.nvim/issues/747)) ([9eed863](https://github.com/akinsho/bufferline.nvim/commit/9eed86350dcb4a5cca13056d0d16ba85e20e5024))
* **groups:** use correct cmdline completion function ([a4bd445](https://github.com/akinsho/bufferline.nvim/commit/a4bd44523316928a7c4a5c09a3407d02c30b6027))

## [4.0.0](https://github.com/akinsho/bufferline.nvim/compare/v3.7.0...v4.0.0) (2023-04-23)


### ⚠ BREAKING CHANGES

* **groups:** change argument to group matcher
* **config:** deprecate show_buffer_default_icon

### Features

* **colors:** add diagnostic underline fallback ([bd9915f](https://github.com/akinsho/bufferline.nvim/commit/bd9915fa13f53176fe3a4a943e3f95c7e4312e50))
* **config:** allow specifying style presets ([13cb114](https://github.com/akinsho/bufferline.nvim/commit/13cb114e91c17238aaa271746aaeb8e967f350a2))
* **diag:** sane fallback to underline color ([0cd505b](https://github.com/akinsho/bufferline.nvim/commit/0cd505b333151e883cdd854539e5eae0e4f3e339))


### Bug Fixes

* **color:** follow linked hl groups ([e6e7cc4](https://github.com/akinsho/bufferline.nvim/commit/e6e7cc454fa28304246e97a9acfe7c6cf2adc5d6))
* **highlights:** if color_icons is false set to NONE ([8b32447](https://github.com/akinsho/bufferline.nvim/commit/8b32447f1ba00f71ec2ebb413249d1d84228d9fb)), closes [#702](https://github.com/akinsho/bufferline.nvim/issues/702)
* **sorters:** insert_after_current strategy ([1620cfe](https://github.com/akinsho/bufferline.nvim/commit/1620cfe8f226b49bfc4886a092449f565b4d84ab))


### Code Refactoring

* **config:** deprecate show_buffer_default_icon ([6ccdee8](https://github.com/akinsho/bufferline.nvim/commit/6ccdee8e931503699eb8f92c7faafd0ad1a8cf69))
* **groups:** change argument to group matcher ([38d62b8](https://github.com/akinsho/bufferline.nvim/commit/38d62b8bae62c681d6e259de54421d4155976897))

## [3.7.0](https://github.com/akinsho/bufferline.nvim/compare/v3.6.0...v3.7.0) (2023-04-15)


### Features

* **groups:** close and unpin ([#698](https://github.com/akinsho/bufferline.nvim/issues/698)) ([52241b5](https://github.com/akinsho/bufferline.nvim/commit/52241b57ed41c2283020c6c79ef48fc7cd808bea))


### Bug Fixes

* **ui:** Use correct function to check for list ([#726](https://github.com/akinsho/bufferline.nvim/issues/726)) ([dd86c31](https://github.com/akinsho/bufferline.nvim/commit/dd86c312fd225549ac02567d47570c04ba456402))
* **utils:** fix utils.is_list ([#728](https://github.com/akinsho/bufferline.nvim/issues/728)) ([2c8d615](https://github.com/akinsho/bufferline.nvim/commit/2c8d615c47a5013b24b3b4bdebec2fda1b38cdd9))
