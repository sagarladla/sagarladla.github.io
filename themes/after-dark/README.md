# After Dark

> A retro dark theme for [Hugo].

[![Latest NPM version](https://flat.badgen.net/npm/v/after-dark)](https://www.npmjs.com/after-dark)
[![Weekly downloads](https://flat.badgen.net/npm/dw/after-dark)](https://www.npmjs.com/after-dark)
[![Minimum Hugo version](https://flat.badgen.net/badge/hugo/>=0.51/FF4088)](https://gohugo.io)
[![AGPL licensed](https://img.shields.io/npm/l/after-dark.svg?style=flat-square&longCache=true)](https://codeberg.org/vhs/after-dark/src/branch/trunk/COPYING)

## Highlights

- **Developer Focused:** Cross-platform, 1 dependency, single-codebase.
- **Incredibly Fast:** ~0.615s average build time and decisecond page loads.
- **Privacy Aware:** No cookies, no trackers, no external requests.
- **Securely Designed:** Source-level integrity checking and strict content security policy.
- **Advanced Graphics:** BPG image support, PhotoSwipe support, aggressive lazy-loading.
- **Easily Customized:** Override any theme template to compose your own views.
- **Fuzzy Search:** Offline, automatic and no third-parties.
- **Batteries Included**: Integrates with Gitea, Kubernetes, Traefik and Fathom Analytics.
- **Extended Builds:** Add Sass support to your project and decrease built times.
- **Detailed Docs:** Includes example documentation website written using After Dark.

## Screenshot

[![](https://codeberg.org/vhs/after-dark/raw/branch/trunk/docs/static/images/screenshots/after-dark-v6.15.0-homepage-fs8.png)](https://codeberg.org/vhs/after-dark)

## Requirements

Hugo 0.51+ required. Run `make hugo` for [extended build](https://vhs.codeberg.page/after-dark/feature/extended-builds/), or visit [Install Hugo](https://gohugo.io/installation/) for official steps.

### Installation

The easiest installation method is to run the quick install script:

```sh
wget -qO- https://codeberg.org/vhs/after-dark/raw/branch/trunk/bin/install | sh
```

Quick Install will ensure the machine is running a supported Hugo version, download the latest signed `after-dark` release, download the latest signed `fractal-forest`, and configure a sample After Dark site with welcome post.

By convention After Dark may also be installed as a [Hugo Theme Component](https://gohugo.io/hugo-modules/theme-components/):

```sh
flying-toasters
├── static
└── themes
    └── after-dark # git clone or submodule
```

### Usage

Run the online help server after installing for After Dark usage instructions:

```sh
./themes/after-dark/bin/help
```

Also visit the [Hugo docs](https://gohugo.io/documentation/), the [Hugo community forum](https://discourse.gohugo.io/) and [Stack Overflow](https://stackoverflow.com/questions/tagged/hugo).

### Upgrading

Run the [Upgrade Script](https://vhs.codeberg.page/after-dark/feature/upgrade-script/) to check for updates and upgrade automatically:

```sh
./themes/after-dark/bin/upgrade
```

Upgrading replaces the file contents of the theme as a whole for security reasons. If you wish to modify the source please create a fork.

### Verifying

Use the [Release Validator](https://vhs.codeberg.page/after-dark/validate/) from `https://localhost:1414/validate/` while the online help server is running to verify you're running a PGP-signed and SHA-verified release. Integrity is checked at the source level and may be performed offline. See [Release Hashes](https://vhs.codeberg.page/after-dark/feature/release-hashes/) to learn more.

## Credits

Thanks to エゴイスト for [hack.css]; Dan Klammer for [bytesize icons]; Vincent Prouillet for creating a [Zola port of After Dark]; the author, maintainers and contributors to [hugo]; and thanks to the SiliconValley homesteaders on Geocities, and Berkeley Systems, for the design inspiration.

## Rights

After Dark - A retro dark theme for Hugo.<br>
Copyright (C) 2019&nbsp;&nbsp;VHS &lt;vhsdev@tutanota.com&gt; (https://vhs.codeberg.page)

After Dark is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

See file [COPYING](./COPYING) for warranty disclaimer and full license text.

[hack.css]: https://hackcss.egoist.dev/
[hugo]: https://gohugo.io/
[bytesize icons]: https://github.com/danklammer/bytesize-icons
[Zola port of After Dark]: https://www.getzola.org/themes/after-dark/
