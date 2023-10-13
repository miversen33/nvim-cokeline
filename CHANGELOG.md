# Changelog

## 1.0.0 (2023-10-13)


### ⚠ BREAKING CHANGES

* only hide tabline based on opts.show_if_buffers_are_at_least
* don't delete buffer when falling back to history
* remove `utils.get_hex` - use `hlgroups.get_hl_attr`
* support for more highlight attrs ([#150](https://github.com/miversen33/nvim-cokeline/issues/150))
* make scratch buffer if deleting last buffer
* use stream-based iterators where possible
* **pick:** retain pick char order when not using filename ([#132](https://github.com/miversen33/nvim-cokeline/issues/132))

### Features

* add fallback icon by filetype ([#121](https://github.com/miversen33/nvim-cokeline/issues/121)) ([fd154f9](https://github.com/miversen33/nvim-cokeline/commit/fd154f9a11fa6da61ce631968fa7e93455304fb4))
* add fill_hl config option ([7ec240f](https://github.com/miversen33/nvim-cokeline/commit/7ec240f60c0139206ee20ff46e67a131d50c785f))
* add index property to TabPage object ([4863677](https://github.com/miversen33/nvim-cokeline/commit/48636776059b5fb6de4b91a21655b06d16150ce6))
* add utility methods to Buffer ([caba2d1](https://github.com/miversen33/nvim-cokeline/commit/caba2d133fdd9cdcfb3ebafc27c20d1dd3271561))
* allow `fg` and `bg` to be set to hlgroup name ([c29c2a1](https://github.com/miversen33/nvim-cokeline/commit/c29c2a1bd95c9145c403d81bef47667009d5041b))
* allow multiple sidebar filetypes ([3353afc](https://github.com/miversen33/nvim-cokeline/commit/3353afc4f44741766d3d33d08ced65045445554d))
* allow multiple vert splits in sidebar ([03944cf](https://github.com/miversen33/nvim-cokeline/commit/03944cf50cfb599f589a958a864aae15f8725a4a))
* allow passing function to mapping funcs ([1a25aee](https://github.com/miversen33/nvim-cokeline/commit/1a25aee3e63d2b745df6ba0b35b607117edf4306))
* buffer history ringbuffer ([#131](https://github.com/miversen33/nvim-cokeline/issues/131)) ([492408b](https://github.com/miversen33/nvim-cokeline/commit/492408b2ad8c47898f11143403fde46f7c8e7761))
* **buffers:** config options for pick ([d179cda](https://github.com/miversen33/nvim-cokeline/commit/d179cdaf46e7287078888505ab1f405bd36321ea))
* close by step and by index ([852fd38](https://github.com/miversen33/nvim-cokeline/commit/852fd38a29bb213c559ad61da4188ac523ecc72a)), closes [#90](https://github.com/miversen33/nvim-cokeline/issues/90)
* custom components on right side of tabline ([631f225](https://github.com/miversen33/nvim-cokeline/commit/631f2252412afa6fb58211fa826604a75531fbab))
* custom sorting functions ([befa096](https://github.com/miversen33/nvim-cokeline/commit/befa096b2a7b17c2298123e7dbe6a89a07404038))
* fallback to history for focus by step ([02284b9](https://github.com/miversen33/nvim-cokeline/commit/02284b9987af8bc48f45d5090ca593c09773e74d))
* global (per buffer/tab/etc) hover events ([709a379](https://github.com/miversen33/nvim-cokeline/commit/709a379255157520f29aee6bfb3d33c92b0e019a))
* handle click events with Lua, fix bufdelete ([#103](https://github.com/miversen33/nvim-cokeline/issues/103)) ([6748abd](https://github.com/miversen33/nvim-cokeline/commit/6748abd0a1e79f51d6bee0fc91a633a22ea05e92))
* **history:** persist history with `resession` extension ([#174](https://github.com/miversen33/nvim-cokeline/issues/174)) ([96255ec](https://github.com/miversen33/nvim-cokeline/commit/96255ecf86ef7beb232c6b18d847c87c0e386166))
* hover events ([93c7dbb](https://github.com/miversen33/nvim-cokeline/commit/93c7dbb81dca7bf379e63b08efdcc29ae9425503))
* legacy mouse mappings ([0143682](https://github.com/miversen33/nvim-cokeline/commit/0143682247c90da1fa1f9359aada5d77e8c3d029))
* more tabpage props ([391f872](https://github.com/miversen33/nvim-cokeline/commit/391f8724e804d699f21297bf97f3e29c81e00fa7))
* native tab support ([b6f7281](https://github.com/miversen33/nvim-cokeline/commit/b6f7281bb64546cb6ebfea6d3d6a5ade6e89c37b))
* per-component click handlers ([5f0e978](https://github.com/miversen33/nvim-cokeline/commit/5f0e978afd9ed37cfa00c72e2f0fb39b88407924))
* **pick:** release taken letters when deleting buffers ([dce9f06](https://github.com/miversen33/nvim-cokeline/commit/dce9f06d939b85abb5222939874343e3100a4c0d))
* **pick:** retain pick char order when not using filename ([#132](https://github.com/miversen33/nvim-cokeline/issues/132)) ([9da5427](https://github.com/miversen33/nvim-cokeline/commit/9da5427ecb6e60cd26a381b93fae93907a45129a))
* rearrange buffers with mouse drag ([#113](https://github.com/miversen33/nvim-cokeline/issues/113)) ([198dd0a](https://github.com/miversen33/nvim-cokeline/commit/198dd0ab12bc421723fd152e5fe92f1fccb0e550))
* sidebar.get_width() utility function ([5c46b21](https://github.com/miversen33/nvim-cokeline/commit/5c46b213b234308fb93119a6ce0bab0a1f176b5e))
* sidebars on rhs of editor ([c76d23b](https://github.com/miversen33/nvim-cokeline/commit/c76d23b42aa5ab30d6049544b12033919acc35a4))
* sorting by bufnr ([eee6a10](https://github.com/miversen33/nvim-cokeline/commit/eee6a101a579f6dcfa37d7dc92a1e807adf870d3))
* sorting by directory ([a293d86](https://github.com/miversen33/nvim-cokeline/commit/a293d86e0f47ec69ded4c8ae8ef1c18dc91b1b29))
* support for more highlight attrs ([#150](https://github.com/miversen33/nvim-cokeline/issues/150)) ([e0db489](https://github.com/miversen33/nvim-cokeline/commit/e0db4891c8ce35428463269184ba01f8f4169efe))
* support for passing highlight group names ([#130](https://github.com/miversen33/nvim-cokeline/issues/130)) ([4463ba2](https://github.com/miversen33/nvim-cokeline/commit/4463ba2ee15c552e39392acf071297c9f6517071))
* tab placement config ([27aec2f](https://github.com/miversen33/nvim-cokeline/commit/27aec2f833b2849473bc102c1af9ad28dae0168a))
* update default config ([da7f4c9](https://github.com/miversen33/nvim-cokeline/commit/da7f4c9effe1f1f8538ff00d8648386bb24172e8))
* use ui-select for prompt ([28b9ed6](https://github.com/miversen33/nvim-cokeline/commit/28b9ed6ef2afe8632557953be920543403965546))


### Bug Fixes

* Allow focusing a buffer from a non-valid buffer ([eb89773](https://github.com/miversen33/nvim-cokeline/commit/eb89773bb9ca97b1c5f44d3c7a7151ae78ad33fc))
* allow multibyte characters on buffer picker ([4698004](https://github.com/miversen33/nvim-cokeline/commit/469800429c6e71cd46ee226c40035c31bc6a6ba1))
* **bufdel:** ignore first retval of ui.select, prompt for filename if empty ([2f80eeb](https://github.com/miversen33/nvim-cokeline/commit/2f80eebe5296f7eddc7abec2c4f14ec523c6df30))
* **buffers:** ensure current_valid_index is non-nil ([52e050a](https://github.com/miversen33/nvim-cokeline/commit/52e050a319f37a5f752fe8f461db209ab03a3188)), closes [#76](https://github.com/miversen33/nvim-cokeline/issues/76)
* check for both on_key and keycode fns ([0085781](https://github.com/miversen33/nvim-cokeline/commit/0085781014834feecf10ef9d4c7ea89739914074))
* check for Windows always fails when computing `unique_prefix` ([8bb3fb3](https://github.com/miversen33/nvim-cokeline/commit/8bb3fb35d12f98659258f707e012f211146d3baa))
* check hlgroup with hlexists ([d1a9655](https://github.com/miversen33/nvim-cokeline/commit/d1a9655f785239c2fccab95356f1972ee6d84dcc))
* **ci:** use sudo for apt in commitlint ([afd9dc6](https://github.com/miversen33/nvim-cokeline/commit/afd9dc6e3f8d177d28f331dd8c7751d2f88a76fb))
* closing terminal tabs ([#66](https://github.com/miversen33/nvim-cokeline/issues/66)) ([28b9ed6](https://github.com/miversen33/nvim-cokeline/commit/28b9ed6ef2afe8632557953be920543403965546))
* cokeline-pick-close ([bf5e58a](https://github.com/miversen33/nvim-cokeline/commit/bf5e58a2f1e9c3bd2a9b9c97e6a9b9d53a6e7661))
* correct error in readme.md ([3bc1750](https://github.com/miversen33/nvim-cokeline/commit/3bc1750e667c1c19c48f81127c4737fb769d4ca5))
* disable warning for default_hl keys ([f9a9d8c](https://github.com/miversen33/nvim-cokeline/commit/f9a9d8cd12e5cb4467b38a7def766b1b43d715c2))
* **docs:** Replace `focused` with `fg` in default_hl in readme ([#152](https://github.com/miversen33/nvim-cokeline/issues/152)) ([73a6a52](https://github.com/miversen33/nvim-cokeline/commit/73a6a52001aad42ada57acba875f110661aea01d))
* don't check mousemoveevent unless needed ([a7efa64](https://github.com/miversen33/nvim-cokeline/commit/a7efa64386467114e386a0f19f4a6086a5650010))
* ensure tabs are always updated on TabNew and TabClosed ([68b915a](https://github.com/miversen33/nvim-cokeline/commit/68b915ac0e389f4c094ec3d9284b2d73f9c7ac96))
* error when window is extremely small ([45d7c85](https://github.com/miversen33/nvim-cokeline/commit/45d7c85ea37bbf7745e9637243a1a4d9320886a5))
* errors when rendering with no buffers visible ([89be4de](https://github.com/miversen33/nvim-cokeline/commit/89be4de2e67ec3951452ec05b5f8ed6717796323))
* fallback to char from list, then ? ([8e8f9f9](https://github.com/miversen33/nvim-cokeline/commit/8e8f9f9c4d4fa756b3f7f116e10df8756c8177a9))
* get config before checking deps ([dc00262](https://github.com/miversen33/nvim-cokeline/commit/dc0026200d290a19ab595c0cc2d41fe2bcd22271))
* highlight caching ([0d2988c](https://github.com/miversen33/nvim-cokeline/commit/0d2988c6eff6c58dfc04b08639ae5ff04a21b32c))
* **history:** iter() should not return an infinite iterator ([a2217b1](https://github.com/miversen33/nvim-cokeline/commit/a2217b14ad034894fa1aff5197def3fb04aaafc7))
* hover events for sidebar ([631f225](https://github.com/miversen33/nvim-cokeline/commit/631f2252412afa6fb58211fa826604a75531fbab))
* hover position after truncation ([896508f](https://github.com/miversen33/nvim-cokeline/commit/896508fc71a198d523099d06f632d8075313a2a9))
* incorrect function name in sidebar ([c2842a5](https://github.com/miversen33/nvim-cokeline/commit/c2842a51df781d357cd3408c411a7bec147b57ae))
* index update value ([cb4bbdf](https://github.com/miversen33/nvim-cokeline/commit/cb4bbdf9bb6c8a070a655f04842bb86a101e040d))
* make sure component is non-nil in hover handler ([461c12b](https://github.com/miversen33/nvim-cokeline/commit/461c12b511a0e0286c2efea72487901d9edd59d1))
* **mapping:** handle gracefully keyboard interrupt on buffer pick. ([0edbbd7](https://github.com/miversen33/nvim-cokeline/commit/0edbbd78eee9c54a123f0085e9ce9b941f5840a7))
* **mappings:** attempt to get next buffer when using history fallback ([2bf44ee](https://github.com/miversen33/nvim-cokeline/commit/2bf44ee9096e488d0b84b5f364c05a282ed227f1))
* nil checks for `last_removed_component` ([cf8580e](https://github.com/miversen33/nvim-cokeline/commit/cf8580ecae80ba07b1f2c0c164a2f77edab64b20))
* on_mouse_leave when moving within bar ([b790802](https://github.com/miversen33/nvim-cokeline/commit/b7908029fa885ecb108e8394ff8fd7b572bc81cc))
* pass width properly to `string.rep` ([e965cbd](https://github.com/miversen33/nvim-cokeline/commit/e965cbdb48ebcc2792b57cdebd92458565bdc214))
* preserve hover handlers on reorder ([7fb6753](https://github.com/miversen33/nvim-cokeline/commit/7fb6753c8fb90eebb6b56f86fc6e65468a23c81c))
* remove unused import in config.lua ([9d2ec14](https://github.com/miversen33/nvim-cokeline/commit/9d2ec147adae611118c21dc03630f4952f5ae419))
* reset hlgroup to `TabLine` after buffers ([b4ab430](https://github.com/miversen33/nvim-cokeline/commit/b4ab430516ec6b87ed7d1eac3b93a4195d55a1c5))
* set current_index in rendering.lua ([62b2b69](https://github.com/miversen33/nvim-cokeline/commit/62b2b69d97ab17cddf6381b4a2d37a441a7b9fd0))
* update default close icon ([acf1047](https://github.com/miversen33/nvim-cokeline/commit/acf104756543fd7d53a68ccd32bbdec31b946227)), closes [#148](https://github.com/miversen33/nvim-cokeline/issues/148)
* use `buf_is_valid` for both `delete` and `wipeout` in `bufdelete` ([999a483](https://github.com/miversen33/nvim-cokeline/commit/999a483f637779b248459cfc100299a42bb459d4))
* use `utils.buf_delete` in mappings ([bba40cd](https://github.com/miversen33/nvim-cokeline/commit/bba40cdfe4942c4f5871417d2f1d2f8b9be7e7ec))
* use cx.provider.number for sidebar bufnr ([4cbf54f](https://github.com/miversen33/nvim-cokeline/commit/4cbf54f10d2d746f1a72fd7e6715738d5e3602f8))
* use dot in require instead of slash ([b64d130](https://github.com/miversen33/nvim-cokeline/commit/b64d130810e5348d986af8ea4686c7767519d3ed)), closes [#153](https://github.com/miversen33/nvim-cokeline/issues/153)


### Performance Improvements

* bufnr to Buffer lookup table ([fbdacfe](https://github.com/miversen33/nvim-cokeline/commit/fbdacfef6372b7ba2b8bfacbc662bd05a9942736))
* cache tabs and update with autocmds ([c582990](https://github.com/miversen33/nvim-cokeline/commit/c5829906fb2f5faa9c0f4455323953eebdfc65a7))
* use stream-based iterators where possible ([8b877a9](https://github.com/miversen33/nvim-cokeline/commit/8b877a972337623f3f28f85a71611b2a08911b3a))
* use vim.iter when available ([fbdacfe](https://github.com/miversen33/nvim-cokeline/commit/fbdacfef6372b7ba2b8bfacbc662bd05a9942736))


### Code Refactoring

* don't delete buffer when falling back to history ([652ac5f](https://github.com/miversen33/nvim-cokeline/commit/652ac5f6ab2ccf162ad74b2618cd86f9ce1f4c70))
* make scratch buffer if deleting last buffer ([368cd3e](https://github.com/miversen33/nvim-cokeline/commit/368cd3ebd2395405c2e333d6aa05d8d509ed99d2))
* only hide tabline based on opts.show_if_buffers_are_at_least ([aa25d8d](https://github.com/miversen33/nvim-cokeline/commit/aa25d8dccd3c48ec12e007dc424e2ea86b14fd2b))
* remove `utils.get_hex` - use `hlgroups.get_hl_attr` ([b56f12b](https://github.com/miversen33/nvim-cokeline/commit/b56f12b9a72e96b1103accd6dd05b6e9f5cf44e4))

## [Unreleased](https://github.com/willothy/nvim-cokeline/tree/HEAD)

[Full Changelog](https://github.com/willothy/nvim-cokeline/compare/v0.4.0...HEAD)

**Merged pull requests:**

- refactor: use modules, lazy requires [\#157](https://github.com/willothy/nvim-cokeline/pull/157) ([willothy](https://github.com/willothy))
- fixup: \(3682c78e\): README: Replace `focused` with `fg` in default_hl [\#152](https://github.com/willothy/nvim-cokeline/pull/152) ([UtsavBalar1231](https://github.com/UtsavBalar1231))
- feat!: support for more highlight attrs [\#150](https://github.com/willothy/nvim-cokeline/pull/150) ([willothy](https://github.com/willothy))
- Update README.md [\#146](https://github.com/willothy/nvim-cokeline/pull/146) ([sashalikesplanes](https://github.com/sashalikesplanes))
- feat: custom sorting functions [\#145](https://github.com/willothy/nvim-cokeline/pull/145) ([willothy](https://github.com/willothy))
- feat: provide require\("cokeline.sidebar"\).get_width\(\) and cache sidebar widths [\#143](https://github.com/willothy/nvim-cokeline/pull/143) ([willothy](https://github.com/willothy))
- refactor!: make scratch buffer if deleting last buffer [\#142](https://github.com/willothy/nvim-cokeline/pull/142) ([willothy](https://github.com/willothy))
- feat: global \(per buffer/tab/etc\) hover events [\#140](https://github.com/willothy/nvim-cokeline/pull/140) ([willothy](https://github.com/willothy))

## [v0.4.0](https://github.com/willothy/nvim-cokeline/tree/v0.4.0) (2023-07-02)

[Full Changelog](https://github.com/willothy/nvim-cokeline/compare/v0.3.0...v0.4.0)

**Merged pull requests:**

- feat: sidebars on rhs of editor [\#138](https://github.com/willothy/nvim-cokeline/pull/138) ([willothy](https://github.com/willothy))
- feat: native tab support [\#136](https://github.com/willothy/nvim-cokeline/pull/136) ([willothy](https://github.com/willothy))
- perf: use stream-based iterators where possible [\#135](https://github.com/willothy/nvim-cokeline/pull/135) ([willothy](https://github.com/willothy))
- Use named color names [\#134](https://github.com/willothy/nvim-cokeline/pull/134) ([lucassperez](https://github.com/lucassperez))
- feat\(pick\): retain pick char order when not using filename [\#132](https://github.com/willothy/nvim-cokeline/pull/132) ([willothy](https://github.com/willothy))
- feat: buffer history ringbuffer [\#131](https://github.com/willothy/nvim-cokeline/pull/131) ([willothy](https://github.com/willothy))
- feat: support for passing highlight group names [\#130](https://github.com/willothy/nvim-cokeline/pull/130) ([nenikitov](https://github.com/nenikitov))
- feat: allow multiple vert splits in sidebar [\#129](https://github.com/willothy/nvim-cokeline/pull/129) ([willothy](https://github.com/willothy))
- fix: allow multibyte characters on buffer picker [\#123](https://github.com/willothy/nvim-cokeline/pull/123) ([lucassperez](https://github.com/lucassperez))
- feat: add fallback icon by filetype [\#121](https://github.com/willothy/nvim-cokeline/pull/121) ([Webblitchy](https://github.com/Webblitchy))
- fix: index update value [\#118](https://github.com/willothy/nvim-cokeline/pull/118) ([Equilibris](https://github.com/Equilibris))
- feat: add fill_hl config option [\#114](https://github.com/willothy/nvim-cokeline/pull/114) ([FollieHiyuki](https://github.com/FollieHiyuki))
- feat: Rearrange buffers with mouse drag [\#113](https://github.com/willothy/nvim-cokeline/pull/113) ([willothy](https://github.com/willothy))
- feat\(pick\): release taken letters when deleting buffers [\#112](https://github.com/willothy/nvim-cokeline/pull/112) ([soifou](https://github.com/soifou))
- feat: hover events [\#111](https://github.com/willothy/nvim-cokeline/pull/111) ([willothy](https://github.com/willothy))
- feat: per-component click handlers [\#106](https://github.com/willothy/nvim-cokeline/pull/106) ([willothy](https://github.com/willothy))
- feat: close by step and by index [\#104](https://github.com/willothy/nvim-cokeline/pull/104) ([willothy](https://github.com/willothy))
- feat: handle click events with Lua, add bufdelete util [\#103](https://github.com/willothy/nvim-cokeline/pull/103) ([willothy](https://github.com/willothy))
- Proposal: Add sorting by directory [\#97](https://github.com/willothy/nvim-cokeline/pull/97) ([ewok](https://github.com/ewok))
- feat: `pick.use_filename` and `pick.letters` config options [\#88](https://github.com/willothy/nvim-cokeline/pull/88) ([ProspectPyxis](https://github.com/ProspectPyxis))
- fix\(mapping\): handle gracefully keyboard interrupt on buffer pick. [\#81](https://github.com/willothy/nvim-cokeline/pull/81) ([soifou](https://github.com/soifou))
- Update README.md [\#70](https://github.com/willothy/nvim-cokeline/pull/70) ([crivotz](https://github.com/crivotz))
- Adding is_last and is_first to buffer return [\#69](https://github.com/willothy/nvim-cokeline/pull/69) ([miversen33](https://github.com/miversen33))
- Add new configuration [\#68](https://github.com/willothy/nvim-cokeline/pull/68) ([danielnieto](https://github.com/danielnieto))
- fix: check for Windows always fails when computing `unique_prefix` [\#65](https://github.com/willothy/nvim-cokeline/pull/65) ([EtiamNullam](https://github.com/EtiamNullam))
- fix: cokeline-pick-close and cokeline-pick-focus in v0.7 [\#53](https://github.com/willothy/nvim-cokeline/pull/53) ([matt-riley](https://github.com/matt-riley))

## [v0.3.0](https://github.com/willothy/nvim-cokeline/tree/v0.3.0) (2022-03-06)

[Full Changelog](https://github.com/willothy/nvim-cokeline/compare/v0.2.0...v0.3.0)

**Merged pull requests:**

- fix: Allow focusing a buffer from a non-valid buffer [\#40](https://github.com/willothy/nvim-cokeline/pull/40) ([tamirzb](https://github.com/tamirzb))

## [v0.2.0](https://github.com/willothy/nvim-cokeline/tree/v0.2.0) (2022-01-01)

[Full Changelog](https://github.com/willothy/nvim-cokeline/compare/v0.1.0...v0.2.0)

## [v0.1.0](https://github.com/willothy/nvim-cokeline/tree/v0.1.0) (2021-12-07)

[Full Changelog](https://github.com/willothy/nvim-cokeline/compare/68b23cb77e2bf76df92a8043612e655e04507ed6...v0.1.0)

**Merged pull requests:**

- Update README.md [\#27](https://github.com/willothy/nvim-cokeline/pull/27) ([KadoBOT](https://github.com/KadoBOT))
- Add author links to readme [\#20](https://github.com/willothy/nvim-cokeline/pull/20) ([alex-popov-tech](https://github.com/alex-popov-tech))
- fix: correct error in readme.md [\#7](https://github.com/willothy/nvim-cokeline/pull/7) ([olimorris](https://github.com/olimorris))
- :bug: fix: `unique_prefix` on windows [\#3](https://github.com/willothy/nvim-cokeline/pull/3) ([Neelfrost](https://github.com/Neelfrost))
- :bug: fix: use correct path separators for unique_prefix depending on OS [\#2](https://github.com/willothy/nvim-cokeline/pull/2) ([Neelfrost](https://github.com/Neelfrost))

\* _This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)_
