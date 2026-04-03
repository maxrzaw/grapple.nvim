# Changelog

## [1.0.0](https://github.com/maxrzaw/grapple.nvim/compare/v0.30.0...v1.0.0) (2026-04-03)


### ⚠ BREAKING CHANGES

* use <s-cr> to change scope and <cr> to open tags in scopes window ([#100](https://github.com/maxrzaw/grapple.nvim/issues/100))
* better window keymaps ([#97](https://github.com/maxrzaw/grapple.nvim/issues/97))
* allow Grapple.quickfix to accept a scope id
* rewrite grapple ([#89](https://github.com/maxrzaw/grapple.nvim/issues/89))
* interval scope resolver ([#49](https://github.com/maxrzaw/grapple.nvim/issues/49))
* **performance:** scope path caching API and state lazy loading ([#40](https://github.com/maxrzaw/grapple.nvim/issues/40))
* support windows paths ([#34](https://github.com/maxrzaw/grapple.nvim/issues/34))
* portal.nvim and grapple.nvim coexistence and cooperation ([#3](https://github.com/maxrzaw/grapple.nvim/issues/3))

### Features

* add :list_scopes to Grapple app ([386b583](https://github.com/maxrzaw/grapple.nvim/commit/386b5838096052db5ae9db26c4556ca08498490e))
* add "?" to open the help window ([be3cff9](https://github.com/maxrzaw/grapple.nvim/commit/be3cff9d08bb426f0c6bcf300667851f1f9bff3b))
* add "help" footer for nvim-0.10 ([2545605](https://github.com/maxrzaw/grapple.nvim/commit/254560564779096cf646f78e585e4fd982da3924))
* add "shown" to scope definition to allow whitelisting scopes in settings ([d9600cd](https://github.com/maxrzaw/grapple.nvim/commit/d9600cd4c49dc1f4b17800a685c419ed600d4dc1))
* add #tags as virtual text in the loaded scopes ui ([0e48330](https://github.com/maxrzaw/grapple.nvim/commit/0e48330c80da1a8b075a456fb13356649b912623))
* add `Grapple.find` ([#114](https://github.com/maxrzaw/grapple.nvim/issues/114)) ([fbacb20](https://github.com/maxrzaw/grapple.nvim/commit/fbacb204370594a1bc9d28677c179928adb0d834))
* add `grapple.scope#root` ([#35](https://github.com/maxrzaw/grapple.nvim/issues/35)) ([3f9c567](https://github.com/maxrzaw/grapple.nvim/commit/3f9c5678a7f5b53cb764f61b909f7b953efc4880))
* add `grapple#tags` ([#64](https://github.com/maxrzaw/grapple.nvim/issues/64)) ([dc45705](https://github.com/maxrzaw/grapple.nvim/commit/dc45705e6dcfbe6f6cff83f5a6234c15fd21893f))
* add Cache:is_open(id) + some luadocs cleanup ([eee8d92](https://github.com/maxrzaw/grapple.nvim/commit/eee8d92e22facc4583e1431fc9de51b678e70234))
* add global cache to App ([526cf25](https://github.com/maxrzaw/grapple.nvim/commit/526cf25f277340c85f1992dcdfa12557fb4307c2))
* add grapple window highlight groups ([#164](https://github.com/maxrzaw/grapple.nvim/issues/164)) ([dd7fd96](https://github.com/maxrzaw/grapple.nvim/commit/dd7fd96975726b8758c3fc2e2899e206a184a589))
* add option to set popup tags window title via callback function ([#76](https://github.com/maxrzaw/grapple.nvim/issues/76)) ([4432252](https://github.com/maxrzaw/grapple.nvim/commit/44322522dc040c1f8349d08489a09f60faa7a2b9))
* add popup#current to obtain the currently open popup menu ([#52](https://github.com/maxrzaw/grapple.nvim/issues/52)) ([afc5ce7](https://github.com/maxrzaw/grapple.nvim/commit/afc5ce7168b4fa23eb78977753431a744f1fe9a1))
* add scope priority ([5e85367](https://github.com/maxrzaw/grapple.nvim/commit/5e853679a8f5412243f30e8a49d5670535fa251b))
* add unused settings.highlights for later ([8ca1e10](https://github.com/maxrzaw/grapple.nvim/commit/8ca1e10e2564d5225190f6fbcfcd5621bcac35ea))
* allow disabling of footer. Fixes [#171](https://github.com/maxrzaw/grapple.nvim/issues/171) ([5caf3c8](https://github.com/maxrzaw/grapple.nvim/commit/5caf3c8249d5cc51a98d2a78387811a0ad4f5ae0))
* allow window style to be passed as an argument ([7456b74](https://github.com/maxrzaw/grapple.nvim/commit/7456b74db6b9474b6b2bba6b755bcb10a45c6550))
* async git branch scope resolver ([#51](https://github.com/maxrzaw/grapple.nvim/issues/51)) ([81e195f](https://github.com/maxrzaw/grapple.nvim/commit/81e195f133d393b8bf5cd192fa0f62ec765aa1ff))
* better scope persistence ([#45](https://github.com/maxrzaw/grapple.nvim/issues/45)) ([6b159cb](https://github.com/maxrzaw/grapple.nvim/commit/6b159cb30dc9988748db206edda3366fc77fc3ad))
* better window keymaps ([#97](https://github.com/maxrzaw/grapple.nvim/issues/97)) ([5f1e10c](https://github.com/maxrzaw/grapple.nvim/commit/5f1e10c1424ba4aa8edcfcabc0afadf473e116b7))
* configure default command ([#127](https://github.com/maxrzaw/grapple.nvim/issues/127)) ([7a0a727](https://github.com/maxrzaw/grapple.nvim/commit/7a0a7273002c6ad0c02185b7d2d0f414dfdb06ad))
* configure default scopes ([#123](https://github.com/maxrzaw/grapple.nvim/issues/123)) ([f06f13a](https://github.com/maxrzaw/grapple.nvim/commit/f06f13acccca7e0433dc5a259a85e39376ed2d28))
* cycle scopes with Grapple.cycle_scopes ([6c88bfd](https://github.com/maxrzaw/grapple.nvim/commit/6c88bfde677036fd638fc11851383e370a374c69))
* dedicated lualine component ([#120](https://github.com/maxrzaw/grapple.nvim/issues/120)) ([b07efce](https://github.com/maxrzaw/grapple.nvim/commit/b07efce782ed47a20f9272598bc5a37216f33b4a))
* emit event on scope change "GrappleScopeChanged" (See [#147](https://github.com/maxrzaw/grapple.nvim/issues/147)) ([1e7ffdd](https://github.com/maxrzaw/grapple.nvim/commit/1e7ffdd48ed7a0e0f135c9b9684f5b74c5fbc243))
* **filetype:** set option filetype to "grapple" on popup buffer ([48b9d47](https://github.com/maxrzaw/grapple.nvim/commit/48b9d47f0835d5e6259669967ab63ca73508eb00))
* Grapple window status highlights ([#92](https://github.com/maxrzaw/grapple.nvim/issues/92)) ([cb6107d](https://github.com/maxrzaw/grapple.nvim/commit/cb6107d6497996660a0eedde5663f55db5b75d59))
* hide scopes in scopes window ([c9907ec](https://github.com/maxrzaw/grapple.nvim/commit/c9907ec0293297eecab2a52fd3b6dcae5159f88b))
* implement suffix scope resolver ([#44](https://github.com/maxrzaw/grapple.nvim/issues/44)) ([3b76f8b](https://github.com/maxrzaw/grapple.nvim/commit/3b76f8bf7b83bd602d10560308aca0dc85512c5c))
* **integrations:** add resession.nvim support ([#14](https://github.com/maxrzaw/grapple.nvim/issues/14)) ([3b616af](https://github.com/maxrzaw/grapple.nvim/commit/3b616af9e8da54c3344e2404495f49e01f7771bc))
* **integrations:** move "tagged" portal query to portal repo ([#4](https://github.com/maxrzaw/grapple.nvim/issues/4)) ([50b8271](https://github.com/maxrzaw/grapple.nvim/commit/50b82711cac90ab71da3094a1d6aaaa97881a6bf))
* interval scope resolver ([#49](https://github.com/maxrzaw/grapple.nvim/issues/49)) ([6c77aba](https://github.com/maxrzaw/grapple.nvim/commit/6c77aba224c8edac969bfc8a191975ac5f85426e))
* make quick select configurable ([#112](https://github.com/maxrzaw/grapple.nvim/issues/112)) ([e2e7fea](https://github.com/maxrzaw/grapple.nvim/commit/e2e7feab1285e04da42f1af7d04627b5f65d0624))
* new scope "root_from_buffer" ([#63](https://github.com/maxrzaw/grapple.nvim/issues/63)) ([65350ee](https://github.com/maxrzaw/grapple.nvim/commit/65350ee2de6d764aef25e4953601ba7553d7e368))
* open tagged file in split ([#43](https://github.com/maxrzaw/grapple.nvim/issues/43)) ([644efc7](https://github.com/maxrzaw/grapple.nvim/commit/644efc7293bb1da69feae5e39191ed347eebdba3))
* **performance:** scope path caching API and state lazy loading ([#40](https://github.com/maxrzaw/grapple.nvim/issues/40)) ([4b0a3e7](https://github.com/maxrzaw/grapple.nvim/commit/4b0a3e78bf873e99a031ba0fda5cb365ce9105a4))
* permit "scope" for grapple tagging operations ([#60](https://github.com/maxrzaw/grapple.nvim/issues/60)) ([6f33410](https://github.com/maxrzaw/grapple.nvim/commit/6f334101a6c2816e61190a3b0c7894caf5b2f68b))
* portal.nvim and grapple.nvim coexistence and cooperation ([#3](https://github.com/maxrzaw/grapple.nvim/issues/3)) ([053cae3](https://github.com/maxrzaw/grapple.nvim/commit/053cae329953520bfc59835305847e65768f1deb))
* prune scope save files based on last modified time ([#143](https://github.com/maxrzaw/grapple.nvim/issues/143)) ([f440b0a](https://github.com/maxrzaw/grapple.nvim/commit/f440b0a79e4c3cfa7e74b9bb68ca4a01621ce230))
* **readme:** improve readme ([dc1bdad](https://github.com/maxrzaw/grapple.nvim/commit/dc1bdad4db4cff992e680d66c976d67cb77188bb))
* **readme:** update readme with better api documentation ([c9a61dd](https://github.com/maxrzaw/grapple.nvim/commit/c9a61dd2c97a5e71d5373def1dd7e8692d691f12))
* **readme:** update tags popup menu section ([192f76f](https://github.com/maxrzaw/grapple.nvim/commit/192f76fa6c594a5ac6ffc3f11ed83d9e223939c1))
* rewrite grapple ([#89](https://github.com/maxrzaw/grapple.nvim/issues/89)) ([d05dd6a](https://github.com/maxrzaw/grapple.nvim/commit/d05dd6a9c2e42f6b82d01578104a6c6cc81ab121))
* **scope:** add "git_fallback" and "lsp_fallback" to further scope customization ([c3d27d7](https://github.com/maxrzaw/grapple.nvim/commit/c3d27d77c3c3c821a3d201494cb59634d08b0bcd))
* **scope:** custom scope resolution ([#17](https://github.com/maxrzaw/grapple.nvim/issues/17)) ([525fe11](https://github.com/maxrzaw/grapple.nvim/commit/525fe1125fe0fe1a4a9c8062f150bf038f6608a8))
* **scope:** fallback scope resolution ([#15](https://github.com/maxrzaw/grapple.nvim/issues/15)) ([402c9c5](https://github.com/maxrzaw/grapple.nvim/commit/402c9c5f7e17b5e6e82c1e04761c1ca68e13915b))
* **scope:** implement `static` scope ([#29](https://github.com/maxrzaw/grapple.nvim/issues/29)) ([490dedf](https://github.com/maxrzaw/grapple.nvim/commit/490dedf566fdecdc3accc5e150a84ac0c6bf95aa))
* **scope:** LSP scope resolution ([#16](https://github.com/maxrzaw/grapple.nvim/issues/16)) ([2c510cb](https://github.com/maxrzaw/grapple.nvim/commit/2c510cbad245c105288a29083e82a248d708026c))
* support windows paths ([#34](https://github.com/maxrzaw/grapple.nvim/issues/34)) ([5ae3551](https://github.com/maxrzaw/grapple.nvim/commit/5ae35517c0b69e26bf8b59948237fa24708fc818))
* tag path under cursor ([#108](https://github.com/maxrzaw/grapple.nvim/issues/108)) ([f9285cc](https://github.com/maxrzaw/grapple.nvim/commit/f9285cc859d9dfb6d2b4b467572dd8d3dd36c34e))
* tags quickfix list ([#42](https://github.com/maxrzaw/grapple.nvim/issues/42)) ([b3a98db](https://github.com/maxrzaw/grapple.nvim/commit/b3a98dbc26a3b0962248a5bad71c643e4e784d84))
* telescope extension ([#69](https://github.com/maxrzaw/grapple.nvim/issues/69)) ([fe3529c](https://github.com/maxrzaw/grapple.nvim/commit/fe3529c5b9af133d72581bb61a5818cd7c02df40))
* toggle showing loaded and unloaded scopes in UI with '&lt;s-cr&gt;' ([03ffbb9](https://github.com/maxrzaw/grapple.nvim/commit/03ffbb907adffd4d95214265ac987e312946674e))
* **ui:** (optional) add title to popup using new nvim-0.9 features ([fa2d4a6](https://github.com/maxrzaw/grapple.nvim/commit/fa2d4a6bebc0b2af5fbaa4ff41dc0e0b2192daf3))
* unload scopes ([5b184b6](https://github.com/maxrzaw/grapple.nvim/commit/5b184b6eea00e6c1083e74b472440b9c79e850f8))
* use &lt;s-cr&gt; to change scope and <cr> to open tags in scopes window ([#100](https://github.com/maxrzaw/grapple.nvim/issues/100)) ([5aaab2e](https://github.com/maxrzaw/grapple.nvim/commit/5aaab2ef1e07b8785e90f8e84f36e46caeaa341b))
* use quick_select for statusline ([#129](https://github.com/maxrzaw/grapple.nvim/issues/129)) ([9cb1749](https://github.com/maxrzaw/grapple.nvim/commit/9cb17495546f0f7839b16f4b1e0285d893232127))
* user command completion + default use "toggle" ([#99](https://github.com/maxrzaw/grapple.nvim/issues/99)) ([25128ee](https://github.com/maxrzaw/grapple.nvim/commit/25128ee23c9743e35656ddc940358a702457d5f7))
* window styles + tag renaming ([#106](https://github.com/maxrzaw/grapple.nvim/issues/106)) ([a5529b8](https://github.com/maxrzaw/grapple.nvim/commit/a5529b8899089ca27a3ace583ab19f66bcd32798))


### Bug Fixes

* add deprecated Grapple.key to avoid breaking statuslines ([f8bbae6](https://github.com/maxrzaw/grapple.nvim/commit/f8bbae610a8d48923496b2596cfbac59a26f8112))
* add missing :GrappleCycle command ([1369bd1](https://github.com/maxrzaw/grapple.nvim/commit/1369bd188a9a696723a990f81693dc9db9cd4713))
* add missing keymap description + handle nil descriptions in help window ([2f1011b](https://github.com/maxrzaw/grapple.nvim/commit/2f1011bd573c9a240e3eaed2365a8a050bdaeb5f))
* add nargs to :GrapplePopup ([65de44a](https://github.com/maxrzaw/grapple.nvim/commit/65de44abb66f93259a0c9f433a9c66527c53aad5))
* add nested test case to scope_spec #fallback ([484fef9](https://github.com/maxrzaw/grapple.nvim/commit/484fef9ad9cdd20154c208b180c1f3d83a5e360a))
* allow deletion of unloaded scopes ([9350912](https://github.com/maxrzaw/grapple.nvim/commit/9350912b46ce0c2fc0386c82f40d71f26e6d01be))
* allow Grapple.quickfix to accept a scope id ([e53c350](https://github.com/maxrzaw/grapple.nvim/commit/e53c3503d3ec00ef422b5a2336314ca778d2a0e3))
* allow paths with spaces in tags window ([7b53a86](https://github.com/maxrzaw/grapple.nvim/commit/7b53a86ba4e0cdb6a58ff38d9d0d2e9f802e1ff9))
* always save on ExitPre ([a714d01](https://github.com/maxrzaw/grapple.nvim/commit/a714d018cdebf5d01ffc7662600c0fdc168dad7d))
* always unset window ids on window close ([601a73a](https://github.com/maxrzaw/grapple.nvim/commit/601a73a9c07a6a8c3082673785af1d84c0a7d6da))
* always update and save on autocommand ([1994e80](https://github.com/maxrzaw/grapple.nvim/commit/1994e80bec734ddd2217b6c980c7de20778c06e8))
* **ci:** only publish docs when README.md changes ([3bcbd2a](https://github.com/maxrzaw/grapple.nvim/commit/3bcbd2ae5b0a14f74271a20ad809ea27a008313a))
* **ci:** remove "version" from luacheck gh action ([0d875be](https://github.com/maxrzaw/grapple.nvim/commit/0d875be0d8f497f62a7955cb6fb4e1a5c852eaa2))
* **ci:** remove token approach ([458c1b5](https://github.com/maxrzaw/grapple.nvim/commit/458c1b50fbe50074df868facff383d59657aa8fa))
* **ci:** typo in ci.yml ([2c2adc9](https://github.com/maxrzaw/grapple.nvim/commit/2c2adc9888cb5e3d00f6e5fd67a84479ab170f67))
* **ci:** update documentation link ([15d44ff](https://github.com/maxrzaw/grapple.nvim/commit/15d44fff935cdf402b76a0d3fab79f3883d14f2c))
* **ci:** use a personal access token to push vimdoc ([3628333](https://github.com/maxrzaw/grapple.nvim/commit/3628333a49681f1aae7efb5b5ee4af5bf767344f))
* **ci:** use correct PAT name ([87df929](https://github.com/maxrzaw/grapple.nvim/commit/87df92958095d8b2e632aa2d5e1693e5741e909f))
* **ci:** use force push ([b6e2e3b](https://github.com/maxrzaw/grapple.nvim/commit/b6e2e3bd86ebea45502a919af50ed7fccfbd4e70))
* deepcopy tags before returning in Grapple.tags ([5d96868](https://github.com/maxrzaw/grapple.nvim/commit/5d96868a6e9791b7a8ee51a9eef43fc408b9650e))
* **docs:** add &lt;br&gt; in grapple api section ([7a16d7e](https://github.com/maxrzaw/grapple.nvim/commit/7a16d7e1fc6d68cf82072e8b42cb8cc6a5b7bbdd))
* **docs:** correct [@cast](https://github.com/cast) for direction ([306eb36](https://github.com/maxrzaw/grapple.nvim/commit/306eb36d0bbf9e1e13cb36785dd377c90b78df77))
* **docs:** incorrect information for grapple.scope_definition type ([d256401](https://github.com/maxrzaw/grapple.nvim/commit/d256401e6850c30db96385df39f87db345e9c044))
* **docs:** remove old vimdocs ([f345bd1](https://github.com/maxrzaw/grapple.nvim/commit/f345bd14e16c14229f0857ec9e7b8e0343a2ea49))
* **docs:** reorder grapple.scope_definition fields ([c0a6b04](https://github.com/maxrzaw/grapple.nvim/commit/c0a6b040eade05192c9a8b744f151a511b3cb8fd))
* **docs:** resolve some linting errors ([fcca9e8](https://github.com/maxrzaw/grapple.nvim/commit/fcca9e8c2a0cc8eab75fd89f49642d38d17e72db))
* **docs:** s/forward/backward in jump section ([997b84a](https://github.com/maxrzaw/grapple.nvim/commit/997b84ae037691de62e9ae73a0f3f9698eb3b417))
* **docs:** s/uv_timer_t/uv.uv_timer_t/ ([22d0272](https://github.com/maxrzaw/grapple.nvim/commit/22d02729333069b37d28b64174e04719b15a9e8c))
* **docs:** typo in readme ([#74](https://github.com/maxrzaw/grapple.nvim/issues/74)) ([0897be8](https://github.com/maxrzaw/grapple.nvim/commit/0897be818a503039c396451580c239775ad90710))
* **docs:** update link to grapple.tag ([ce47f12](https://github.com/maxrzaw/grapple.nvim/commit/ce47f12e47c00dd633af1168d25365bd60cb7df3))
* don't allow empty tag names ([79fef01](https://github.com/maxrzaw/grapple.nvim/commit/79fef012fc2129865ac6612537835cb322ca2c74))
* don't break lualine if Grapple.tags returns an error ([7f6edfe](https://github.com/maxrzaw/grapple.nvim/commit/7f6edfefd80fb25cbe790be1fd77d2c72045ce36))
* don't close loaded scopes window when a scope is reset ([dcc5984](https://github.com/maxrzaw/grapple.nvim/commit/dcc598415ce24e5faaee232c5e6a792bda7c957c))
* don't eagerly load current scope on setup ([b2b0586](https://github.com/maxrzaw/grapple.nvim/commit/b2b058606ce2ef4c9cb2ca133bb649aca648ecd1))
* escape container_id in Loaded Scopes window ([8903901](https://github.com/maxrzaw/grapple.nvim/commit/89039013f6092053f1a45dd1abbc946ffc3d9f80))
* escape strings before use as a string pattern ([#109](https://github.com/maxrzaw/grapple.nvim/issues/109)) ([efa530c](https://github.com/maxrzaw/grapple.nvim/commit/efa530cfd4a3136b5d20d264b9f8f6d32f4dcc9e))
* help window should handle non-consecutive quick select mappings ([5720f81](https://github.com/maxrzaw/grapple.nvim/commit/5720f81718db14a831c8b4a822c24c70d0ef8795))
* improve window entry parsing ([#102](https://github.com/maxrzaw/grapple.nvim/issues/102)) ([374e72a](https://github.com/maxrzaw/grapple.nvim/commit/374e72a7e943bbad00917dbe11b41e00fa10fb34))
* incorrect docs regarding scope loading ([bbcbf20](https://github.com/maxrzaw/grapple.nvim/commit/bbcbf20b20405565558423695832addd5fac418d))
* **keymap:** add nowait ([218a58b](https://github.com/maxrzaw/grapple.nvim/commit/218a58bff8a91b1959cbab670b96a78dca64738a))
* **logfile:** put it in cache stdpath ([09117ca](https://github.com/maxrzaw/grapple.nvim/commit/09117ca8fc822a659d31f0dd6abb5941fdef0a94))
* **marks:** ensure buffer is valid ([2054dd2](https://github.com/maxrzaw/grapple.nvim/commit/2054dd27860c1cfcd137c75968b47da0b666fb43))
* minimum column ([#125](https://github.com/maxrzaw/grapple.nvim/issues/125)) ([42a150d](https://github.com/maxrzaw/grapple.nvim/commit/42a150d0f4674010cf7bee95bdd1648da0b1142d))
* minor cache module improvements ([1686932](https://github.com/maxrzaw/grapple.nvim/commit/1686932ad964bf4965b02900072cda716b0aed19))
* missing empty vimdoc file ([bf8e2a6](https://github.com/maxrzaw/grapple.nvim/commit/bf8e2a69db56fcdf41bca71d142e2c3b8028b4fc))
* notify when scope has been reset ([3166a6f](https://github.com/maxrzaw/grapple.nvim/commit/3166a6f99ccb9cda1d4f5b6dd8939101a021cef3))
* place cursor on "current" entry in ui ([5f7cbaa](https://github.com/maxrzaw/grapple.nvim/commit/5f7cbaa65d3656ea1d18ee6dbc1781c27761158f))
* **popup:** set filetype after creating both buffer and window ([946dbd0](https://github.com/maxrzaw/grapple.nvim/commit/946dbd0242067b441fcb5cfbc324c121113f7dd5))
* provide the popup_menu to the resolve function ([#53](https://github.com/maxrzaw/grapple.nvim/issues/53)) ([c531463](https://github.com/maxrzaw/grapple.nvim/commit/c5314637914e3bc94213c08e712fcfd5ef7ea6ef))
* **readme:** add missing &lt;/b&gt; tags ([057b3c9](https://github.com/maxrzaw/grapple.nvim/commit/057b3c9ab4336857f276f3161cf6ca9ef73a19ad))
* **readme:** custom scope needs one extra curly brackets to wrap it ([#162](https://github.com/maxrzaw/grapple.nvim/issues/162)) ([924807a](https://github.com/maxrzaw/grapple.nvim/commit/924807aa0522bf75a77126a8f4cbce1c67c42290))
* **readme:** fix docs for `grapple.scope#invalidate ([5734d7f](https://github.com/maxrzaw/grapple.nvim/commit/5734d7f3523743a24778948585e19a71a248edf8))
* **readme:** improve tag scopes documentation ([7c547e1](https://github.com/maxrzaw/grapple.nvim/commit/7c547e1fe657d728ad43b568ddca4e47e6acd30d))
* **readme:** note override in usage section ([4cec0fe](https://github.com/maxrzaw/grapple.nvim/commit/4cec0fe3e103585c5173e06ddcae64525d246e68))
* **readme:** note that scope is optional for #popup_tags ([3280b83](https://github.com/maxrzaw/grapple.nvim/commit/3280b8385ce961bad28c82a1dc0a5f03f38d6b7a))
* **readme:** s/@usage/#usage/ in link ([3b2dcf6](https://github.com/maxrzaw/grapple.nvim/commit/3b2dcf63090658632fe52447e636d54db77bfe1e))
* **readme:** s/grapple/Grapple/ ([60dcbe8](https://github.com/maxrzaw/grapple.nvim/commit/60dcbe83d86eb7a1057bf2434496f131b1a4e9bc))
* **readme:** typo s/config/settings/ ([c32e77b](https://github.com/maxrzaw/grapple.nvim/commit/c32e77b7feda01eaf20b6a576666b635f0a7582c))
* **readme:** typo/ScopeOptions[]/ScopeOptions/ ([5fa4103](https://github.com/maxrzaw/grapple.nvim/commit/5fa410348ebfc60d8cdb3f24ff70fea9e1ff74b3))
* recenter popup window on VimResize ([#79](https://github.com/maxrzaw/grapple.nvim/issues/79)) ([1a8ea56](https://github.com/maxrzaw/grapple.nvim/commit/1a8ea56e9c32121dec2a6f60e0d672732d2b84d3))
* reduce window flickering when toggling unloaded scopes ([b381b69](https://github.com/maxrzaw/grapple.nvim/commit/b381b690fc112acb7f89573e0052ffccb2818ab7))
* remove "cursor" from allowed user command args + fix typo in comment ([50dd1a2](https://github.com/maxrzaw/grapple.nvim/commit/50dd1a2aa9b3d4a2864947b5cb4a2b340a3e99c6))
* remove extra space in help footer ([9fb7660](https://github.com/maxrzaw/grapple.nvim/commit/9fb766082ebb908a8d89448f6aa50a593145c6a4))
* remove keyword completions that are already used ([3686de1](https://github.com/maxrzaw/grapple.nvim/commit/3686de1b0462232ae9665a0caa73f41d09b45052))
* remove unused "key" from excluded subcommands ([a370614](https://github.com/maxrzaw/grapple.nvim/commit/a3706147140bcac63311ab4cdf244e7f435bb9b5))
* remove vim.print in Grapple.prune ([5cc6023](https://github.com/maxrzaw/grapple.nvim/commit/5cc6023febab1aebe4c02fde427fe8c4e8ce7133))
* resetting a loaded scope should unwatch any cached values ([#103](https://github.com/maxrzaw/grapple.nvim/issues/103)) ([d8a87de](https://github.com/maxrzaw/grapple.nvim/commit/d8a87de35a6210ef4f83113febe0548adc539ba9))
* s/pull-request/pull_request ([f2b1e8b](https://github.com/maxrzaw/grapple.nvim/commit/f2b1e8beae506f6ee0c3aa68537e25c8d573ba92))
* send tag absolute path to command instead of short path ([34b8f47](https://github.com/maxrzaw/grapple.nvim/commit/34b8f4728294058e9fdad116fd21f72feb66ab73))
* split by "%s+" instead of " " for command completion ([f510cc8](https://github.com/maxrzaw/grapple.nvim/commit/f510cc8ab91114193dd3e8f143b26b312bd2d5d4))
* **style:** format telescope extension ([03030c4](https://github.com/maxrzaw/grapple.nvim/commit/03030c43567672b18dadc9c053a51060a043ed7d))
* **tags:** ensure file paths are always absolute ([#28](https://github.com/maxrzaw/grapple.nvim/issues/28)) ([bcb6b94](https://github.com/maxrzaw/grapple.nvim/commit/bcb6b94fac0481b8dcae6d9c8265d94cdaa0ef69))
* **tags:** open tag using relative file path ([#75](https://github.com/maxrzaw/grapple.nvim/issues/75)) ([d1c0b57](https://github.com/maxrzaw/grapple.nvim/commit/d1c0b5734111a2b898d45b52c5d1ec7f7101d5e3))
* **tags:** opts.file_path should take precedence over opts.buffer ([04c3877](https://github.com/maxrzaw/grapple.nvim/commit/04c38775d5bd6944c5688ae99f7639ca68699b02))
* **tags:** separate file path resolution in tags#key for "buffer" and "file_path" ([164b97b](https://github.com/maxrzaw/grapple.nvim/commit/164b97b206482edfc515a6879dbcd2c98744bdad))
* telescope entry_maker's ordinal should be a string ([2cbbedf](https://github.com/maxrzaw/grapple.nvim/commit/2cbbedfb3639394caa86b9e57bf7c52a65194112))
* **telescope:** ensure filname is only shortened, not further transformed ([27d58b1](https://github.com/maxrzaw/grapple.nvim/commit/27d58b1fc78836fb37f9db031fbf61f898d3609c))
* **test:** replace vim.fs.joinpath in testing until nvim-0.10 is released ([582b2be](https://github.com/maxrzaw/grapple.nvim/commit/582b2beb68a115bf3609beb8456777e8f0f3303d))
* **test:** update tag_content_spec for new name handling ([dadf665](https://github.com/maxrzaw/grapple.nvim/commit/dadf6658bc657b7f76a8d25b1977a9415d66eb0b))
* **ui:** tag parser should only append the scope path if the file path is relative ([21589e3](https://github.com/maxrzaw/grapple.nvim/commit/21589e38e229eec8c16f92427562974a4ba1c032))
* **ui:** use WinLeave and BufLeave to indicate popup menu closing ([c3902f7](https://github.com/maxrzaw/grapple.nvim/commit/c3902f726221555d0199ac7e4d00781cbabf07c2))
* use App.update instead of Settings.update during Grapple.setup ([c2c6cbf](https://github.com/maxrzaw/grapple.nvim/commit/c2c6cbf160cbf54e11af29eee3319162910045b6))
* use correct byte indexes for highlights in nvim 0.10 ([02bcc88](https://github.com/maxrzaw/grapple.nvim/commit/02bcc8845c1b78c2f22b52798806add4973fc67a))
* use correct starting cycle position when not on a tagged file ([e4d2031](https://github.com/maxrzaw/grapple.nvim/commit/e4d20319d34ff717cb2bbad4556454fd477476d3))
* use provided app instead of global app in scope content ([494b186](https://github.com/maxrzaw/grapple.nvim/commit/494b1862a841117a968cc1e243e9033ea905b193))
* use provided app instead of global app in scope_manager ([e967778](https://github.com/maxrzaw/grapple.nvim/commit/e967778ca5fa92c771da2f3d367d9940745ead0f))
* use types module for Direction ([da7b1b5](https://github.com/maxrzaw/grapple.nvim/commit/da7b1b50af447771b92f21b452c4d23a67b9bd12))
* warn when invoking user command with an invalid action ([1d4ef24](https://github.com/maxrzaw/grapple.nvim/commit/1d4ef242ed21c547a545e435d0f3f8d4e95e8b47))
* wrap nvim_win_set_cursor in pcall ([91c3962](https://github.com/maxrzaw/grapple.nvim/commit/91c396236d9f01b162136fecffb337e93ccee155))

## [0.30.0](https://github.com/cbochs/grapple.nvim/compare/v0.29.0...v0.30.0) (2024-05-18)


### Features

* add grapple window highlight groups ([#164](https://github.com/cbochs/grapple.nvim/issues/164)) ([dd7fd96](https://github.com/cbochs/grapple.nvim/commit/dd7fd96975726b8758c3fc2e2899e206a184a589))


### Bug Fixes

* **readme:** custom scope needs one extra curly brackets to wrap it ([#162](https://github.com/cbochs/grapple.nvim/issues/162)) ([924807a](https://github.com/cbochs/grapple.nvim/commit/924807aa0522bf75a77126a8f4cbce1c67c42290))

## [0.29.0](https://github.com/cbochs/grapple.nvim/compare/v0.28.3...v0.29.0) (2024-04-27)


### Features

* add :list_scopes to Grapple app ([386b583](https://github.com/cbochs/grapple.nvim/commit/386b5838096052db5ae9db26c4556ca08498490e))
* add "shown" to scope definition to allow whitelisting scopes in settings ([d9600cd](https://github.com/cbochs/grapple.nvim/commit/d9600cd4c49dc1f4b17800a685c419ed600d4dc1))
* cycle scopes with Grapple.cycle_scopes ([6c88bfd](https://github.com/cbochs/grapple.nvim/commit/6c88bfde677036fd638fc11851383e370a374c69))


### Bug Fixes

* **docs:** reorder grapple.scope_definition fields ([c0a6b04](https://github.com/cbochs/grapple.nvim/commit/c0a6b040eade05192c9a8b744f151a511b3cb8fd))
* **test:** update tag_content_spec for new name handling ([dadf665](https://github.com/cbochs/grapple.nvim/commit/dadf6658bc657b7f76a8d25b1977a9415d66eb0b))

## [0.28.3](https://github.com/cbochs/grapple.nvim/compare/v0.28.2...v0.28.3) (2024-04-26)


### Bug Fixes

* allow paths with spaces in tags window ([7b53a86](https://github.com/cbochs/grapple.nvim/commit/7b53a86ba4e0cdb6a58ff38d9d0d2e9f802e1ff9))
* **docs:** s/uv_timer_t/uv.uv_timer_t/ ([22d0272](https://github.com/cbochs/grapple.nvim/commit/22d02729333069b37d28b64174e04719b15a9e8c))
* incorrect docs regarding scope loading ([bbcbf20](https://github.com/cbochs/grapple.nvim/commit/bbcbf20b20405565558423695832addd5fac418d))
* minor cache module improvements ([1686932](https://github.com/cbochs/grapple.nvim/commit/1686932ad964bf4965b02900072cda716b0aed19))
* remove unused "key" from excluded subcommands ([a370614](https://github.com/cbochs/grapple.nvim/commit/a3706147140bcac63311ab4cdf244e7f435bb9b5))
* remove vim.print in Grapple.prune ([5cc6023](https://github.com/cbochs/grapple.nvim/commit/5cc6023febab1aebe4c02fde427fe8c4e8ce7133))
* use provided app instead of global app in scope content ([494b186](https://github.com/cbochs/grapple.nvim/commit/494b1862a841117a968cc1e243e9033ea905b193))
* use provided app instead of global app in scope_manager ([e967778](https://github.com/cbochs/grapple.nvim/commit/e967778ca5fa92c771da2f3d367d9940745ead0f))

## [0.28.2](https://github.com/cbochs/grapple.nvim/compare/v0.28.1...v0.28.2) (2024-04-09)


### Bug Fixes

* **docs:** correct [@cast](https://github.com/cast) for direction ([306eb36](https://github.com/cbochs/grapple.nvim/commit/306eb36d0bbf9e1e13cb36785dd377c90b78df77))
* **docs:** resolve some linting errors ([fcca9e8](https://github.com/cbochs/grapple.nvim/commit/fcca9e8c2a0cc8eab75fd89f49642d38d17e72db))

## [0.28.1](https://github.com/cbochs/grapple.nvim/compare/v0.28.0...v0.28.1) (2024-04-05)


### Bug Fixes

* **docs:** incorrect information for grapple.scope_definition type ([d256401](https://github.com/cbochs/grapple.nvim/commit/d256401e6850c30db96385df39f87db345e9c044))
* send tag absolute path to command instead of short path ([34b8f47](https://github.com/cbochs/grapple.nvim/commit/34b8f4728294058e9fdad116fd21f72feb66ab73))

## [0.28.0](https://github.com/cbochs/grapple.nvim/compare/v0.27.1...v0.28.0) (2024-03-31)


### Features

* add Cache:is_open(id) + some luadocs cleanup ([eee8d92](https://github.com/cbochs/grapple.nvim/commit/eee8d92e22facc4583e1431fc9de51b678e70234))
* add global cache to App ([526cf25](https://github.com/cbochs/grapple.nvim/commit/526cf25f277340c85f1992dcdfa12557fb4307c2))
* emit event on scope change "GrappleScopeChanged" (See [#147](https://github.com/cbochs/grapple.nvim/issues/147)) ([1e7ffdd](https://github.com/cbochs/grapple.nvim/commit/1e7ffdd48ed7a0e0f135c9b9684f5b74c5fbc243))

## [0.27.1](https://github.com/cbochs/grapple.nvim/compare/v0.27.0...v0.27.1) (2024-03-27)


### Bug Fixes

* **ci:** update documentation link ([15d44ff](https://github.com/cbochs/grapple.nvim/commit/15d44fff935cdf402b76a0d3fab79f3883d14f2c))

## [0.27.0](https://github.com/cbochs/grapple.nvim/compare/v0.26.0...v0.27.0) (2024-03-27)


### Features

* add scope priority ([5e85367](https://github.com/cbochs/grapple.nvim/commit/5e853679a8f5412243f30e8a49d5670535fa251b))
* hide scopes in scopes window ([c9907ec](https://github.com/cbochs/grapple.nvim/commit/c9907ec0293297eecab2a52fd3b6dcae5159f88b))


### Bug Fixes

* always unset window ids on window close ([601a73a](https://github.com/cbochs/grapple.nvim/commit/601a73a9c07a6a8c3082673785af1d84c0a7d6da))
* deepcopy tags before returning in Grapple.tags ([5d96868](https://github.com/cbochs/grapple.nvim/commit/5d96868a6e9791b7a8ee51a9eef43fc408b9650e))
* escape container_id in Loaded Scopes window ([8903901](https://github.com/cbochs/grapple.nvim/commit/89039013f6092053f1a45dd1abbc946ffc3d9f80))

## [0.26.0](https://github.com/cbochs/grapple.nvim/compare/v0.25.0...v0.26.0) (2024-03-21)


### Features

* prune scope save files based on last modified time ([#143](https://github.com/cbochs/grapple.nvim/issues/143)) ([f440b0a](https://github.com/cbochs/grapple.nvim/commit/f440b0a79e4c3cfa7e74b9bb68ca4a01621ce230))
* unload scopes ([5b184b6](https://github.com/cbochs/grapple.nvim/commit/5b184b6eea00e6c1083e74b472440b9c79e850f8))


### Bug Fixes

* add missing keymap description + handle nil descriptions in help window ([2f1011b](https://github.com/cbochs/grapple.nvim/commit/2f1011bd573c9a240e3eaed2365a8a050bdaeb5f))
* don't eagerly load current scope on setup ([b2b0586](https://github.com/cbochs/grapple.nvim/commit/b2b058606ce2ef4c9cb2ca133bb649aca648ecd1))
* place cursor on "current" entry in ui ([5f7cbaa](https://github.com/cbochs/grapple.nvim/commit/5f7cbaa65d3656ea1d18ee6dbc1781c27761158f))
* reduce window flickering when toggling unloaded scopes ([b381b69](https://github.com/cbochs/grapple.nvim/commit/b381b690fc112acb7f89573e0052ffccb2818ab7))

## [0.25.0](https://github.com/cbochs/grapple.nvim/compare/v0.24.1...v0.25.0) (2024-03-21)


### Features

* toggle showing loaded and unloaded scopes in UI with '&lt;s-cr&gt;' ([03ffbb9](https://github.com/cbochs/grapple.nvim/commit/03ffbb907adffd4d95214265ac987e312946674e))


### Bug Fixes

* allow deletion of unloaded scopes ([9350912](https://github.com/cbochs/grapple.nvim/commit/9350912b46ce0c2fc0386c82f40d71f26e6d01be))
* don't close loaded scopes window when a scope is reset ([dcc5984](https://github.com/cbochs/grapple.nvim/commit/dcc598415ce24e5faaee232c5e6a792bda7c957c))

## [0.24.1](https://github.com/cbochs/grapple.nvim/compare/v0.24.0...v0.24.1) (2024-03-19)


### Bug Fixes

* remove extra space in help footer ([9fb7660](https://github.com/cbochs/grapple.nvim/commit/9fb766082ebb908a8d89448f6aa50a593145c6a4))

## [0.24.0](https://github.com/cbochs/grapple.nvim/compare/v0.23.0...v0.24.0) (2024-03-19)


### Features

* add "help" footer for nvim-0.10 ([2545605](https://github.com/cbochs/grapple.nvim/commit/254560564779096cf646f78e585e4fd982da3924))

## [0.23.0](https://github.com/cbochs/grapple.nvim/compare/v0.22.0...v0.23.0) (2024-03-18)


### Features

* add "?" to open the help window ([be3cff9](https://github.com/cbochs/grapple.nvim/commit/be3cff9d08bb426f0c6bcf300667851f1f9bff3b))
* allow window style to be passed as an argument ([7456b74](https://github.com/cbochs/grapple.nvim/commit/7456b74db6b9474b6b2bba6b755bcb10a45c6550))


### Bug Fixes

* help window should handle non-consecutive quick select mappings ([5720f81](https://github.com/cbochs/grapple.nvim/commit/5720f81718db14a831c8b4a822c24c70d0ef8795))

## [0.22.0](https://github.com/cbochs/grapple.nvim/compare/v0.21.0...v0.22.0) (2024-03-18)


### Features

* use quick_select for statusline ([#129](https://github.com/cbochs/grapple.nvim/issues/129)) ([9cb1749](https://github.com/cbochs/grapple.nvim/commit/9cb17495546f0f7839b16f4b1e0285d893232127))

## [0.21.0](https://github.com/cbochs/grapple.nvim/compare/v0.20.1...v0.21.0) (2024-03-18)


### Features

* configure default command ([#127](https://github.com/cbochs/grapple.nvim/issues/127)) ([7a0a727](https://github.com/cbochs/grapple.nvim/commit/7a0a7273002c6ad0c02185b7d2d0f414dfdb06ad))

## [0.20.1](https://github.com/cbochs/grapple.nvim/compare/v0.20.0...v0.20.1) (2024-03-17)


### Bug Fixes

* minimum column ([#125](https://github.com/cbochs/grapple.nvim/issues/125)) ([42a150d](https://github.com/cbochs/grapple.nvim/commit/42a150d0f4674010cf7bee95bdd1648da0b1142d))

## [0.20.0](https://github.com/cbochs/grapple.nvim/compare/v0.19.0...v0.20.0) (2024-03-16)


### Features

* configure default scopes ([#123](https://github.com/cbochs/grapple.nvim/issues/123)) ([f06f13a](https://github.com/cbochs/grapple.nvim/commit/f06f13acccca7e0433dc5a259a85e39376ed2d28))


### Bug Fixes

* don't break lualine if Grapple.tags returns an error ([7f6edfe](https://github.com/cbochs/grapple.nvim/commit/7f6edfefd80fb25cbe790be1fd77d2c72045ce36))

## [0.19.0](https://github.com/cbochs/grapple.nvim/compare/v0.18.1...v0.19.0) (2024-03-15)


### Features

* dedicated lualine component ([#120](https://github.com/cbochs/grapple.nvim/issues/120)) ([b07efce](https://github.com/cbochs/grapple.nvim/commit/b07efce782ed47a20f9272598bc5a37216f33b4a))


### Bug Fixes

* don't allow empty tag names ([79fef01](https://github.com/cbochs/grapple.nvim/commit/79fef012fc2129865ac6612537835cb322ca2c74))
* use App.update instead of Settings.update during Grapple.setup ([c2c6cbf](https://github.com/cbochs/grapple.nvim/commit/c2c6cbf160cbf54e11af29eee3319162910045b6))
* use correct starting cycle position when not on a tagged file ([e4d2031](https://github.com/cbochs/grapple.nvim/commit/e4d20319d34ff717cb2bbad4556454fd477476d3))

## [0.18.1](https://github.com/cbochs/grapple.nvim/compare/v0.18.0...v0.18.1) (2024-03-14)


### Bug Fixes

* use correct byte indexes for highlights in nvim 0.10 ([02bcc88](https://github.com/cbochs/grapple.nvim/commit/02bcc8845c1b78c2f22b52798806add4973fc67a))

## [0.18.0](https://github.com/cbochs/grapple.nvim/compare/v0.17.2...v0.18.0) (2024-03-11)


### Features

* add `Grapple.find` ([#114](https://github.com/cbochs/grapple.nvim/issues/114)) ([fbacb20](https://github.com/cbochs/grapple.nvim/commit/fbacb204370594a1bc9d28677c179928adb0d834))
* make quick select configurable ([#112](https://github.com/cbochs/grapple.nvim/issues/112)) ([e2e7fea](https://github.com/cbochs/grapple.nvim/commit/e2e7feab1285e04da42f1af7d04627b5f65d0624))


### Bug Fixes

* **docs:** update link to grapple.tag ([ce47f12](https://github.com/cbochs/grapple.nvim/commit/ce47f12e47c00dd633af1168d25365bd60cb7df3))

## [0.17.2](https://github.com/cbochs/grapple.nvim/compare/v0.17.1...v0.17.2) (2024-03-09)


### Bug Fixes

* **ci:** only publish docs when README.md changes ([3bcbd2a](https://github.com/cbochs/grapple.nvim/commit/3bcbd2ae5b0a14f74271a20ad809ea27a008313a))
* **ci:** typo in ci.yml ([2c2adc9](https://github.com/cbochs/grapple.nvim/commit/2c2adc9888cb5e3d00f6e5fd67a84479ab170f67))
* **style:** format telescope extension ([03030c4](https://github.com/cbochs/grapple.nvim/commit/03030c43567672b18dadc9c053a51060a043ed7d))
* **test:** replace vim.fs.joinpath in testing until nvim-0.10 is released ([582b2be](https://github.com/cbochs/grapple.nvim/commit/582b2beb68a115bf3609beb8456777e8f0f3303d))
