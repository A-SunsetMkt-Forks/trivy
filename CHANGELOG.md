# Changelog

## [0.65.0](https://github.com/aquasecurity/trivy/compare/v0.64.0...v0.65.0) (2025-07-30)


### Features

* add graceful shutdown with signal handling ([#9242](https://github.com/aquasecurity/trivy/issues/9242)) ([2c05882](https://github.com/aquasecurity/trivy/commit/2c05882f45071928c14d8212ef6c4f0f7048245d))
* add HTTP request/response tracing support ([#9125](https://github.com/aquasecurity/trivy/issues/9125)) ([aa5b32a](https://github.com/aquasecurity/trivy/commit/aa5b32a19f4d61d0df72c11fd314c5a0b7284202))
* **alma:** add AlmaLinux 10 support ([#9207](https://github.com/aquasecurity/trivy/issues/9207)) ([861d51e](https://github.com/aquasecurity/trivy/commit/861d51e99a45ee448f86fe195dedcaefb811c919))
* **flag:** add schema validation for `--server` flag ([#9270](https://github.com/aquasecurity/trivy/issues/9270)) ([ed4640e](https://github.com/aquasecurity/trivy/commit/ed4640ec27f2575a50d7e6d516c9e2e45a59bb7f))
* **image:** add Docker context resolution ([#9166](https://github.com/aquasecurity/trivy/issues/9166)) ([99cd4e7](https://github.com/aquasecurity/trivy/commit/99cd4e776c0c6cc689126e53fa86ee6333ba6277))
* **license:** observe pkg types option in license scanner ([#9091](https://github.com/aquasecurity/trivy/issues/9091)) ([d44af8c](https://github.com/aquasecurity/trivy/commit/d44af8cfa21a145d14ca6e5e1ed4742d892f2dc5))
* **misconf:** add private ip google access attribute to subnetwork ([#9199](https://github.com/aquasecurity/trivy/issues/9199)) ([263845c](https://github.com/aquasecurity/trivy/commit/263845cfc1419401f24adc8bc6316f3ea0caacad))
* **misconf:** added logging and versioning to the gcp storage bucket ([#9226](https://github.com/aquasecurity/trivy/issues/9226)) ([110f80e](https://github.com/aquasecurity/trivy/commit/110f80ea29951863997dd5a1c48fe14eb81e230b))
* **repo:** add git repository metadata to reports ([#9252](https://github.com/aquasecurity/trivy/issues/9252)) ([f4b2cf1](https://github.com/aquasecurity/trivy/commit/f4b2cf10e917d58c0840f789e083bd3f268a8af1))
* **report:** add CVSS vectors in sarif report ([#9157](https://github.com/aquasecurity/trivy/issues/9157)) ([60723e6](https://github.com/aquasecurity/trivy/commit/60723e6cfce82ede2863cf545a189c581246f4e9))
* **sbom:** add SHA-512 hash support for CycloneDX SBOM ([#9126](https://github.com/aquasecurity/trivy/issues/9126)) ([12d6706](https://github.com/aquasecurity/trivy/commit/12d6706961423acb12430c8b3d986b4aa4671d04))


### Bug Fixes

* **alma:** parse epochs from rpmqa file ([#9101](https://github.com/aquasecurity/trivy/issues/9101)) ([82db2fc](https://github.com/aquasecurity/trivy/commit/82db2fcc8034c911cc7a67f5a82d2f081d9c1fdf))
* also check `filepath` when removing duplicate packages ([#9142](https://github.com/aquasecurity/trivy/issues/9142)) ([4d10a81](https://github.com/aquasecurity/trivy/commit/4d10a815dde53f5e128366f1dd0837a1dc29c17b))
* **aws:** update amazon linux 2 EOL date ([#9176](https://github.com/aquasecurity/trivy/issues/9176)) ([0ecfed6](https://github.com/aquasecurity/trivy/commit/0ecfed6ea75cfe33e0f436a9015ac72a679e754e))
* **cli:** Add more non-sensitive flags to telemetry ([#9110](https://github.com/aquasecurity/trivy/issues/9110)) ([7041a39](https://github.com/aquasecurity/trivy/commit/7041a39bdcf21c5b3114137d9a931f529eac2566))
* **cli:** ensure correct command is picked by telemetry ([#9260](https://github.com/aquasecurity/trivy/issues/9260)) ([b4ad00f](https://github.com/aquasecurity/trivy/commit/b4ad00f301a5fd7326060a567871c6f4a9711696))
* **cli:** panic: attempt to get os.Args[1] when len(os.Args) &lt; 2 ([#9206](https://github.com/aquasecurity/trivy/issues/9206)) ([adfa879](https://github.com/aquasecurity/trivy/commit/adfa879e4e8ab88f211222a13d2b89013ae9a853))
* **license:** add missed `GFDL-NIV-1.1` and `GFDL-NIV-1.2` into Trivy mapping ([#9116](https://github.com/aquasecurity/trivy/issues/9116)) ([a692f29](https://github.com/aquasecurity/trivy/commit/a692f296d15f7241ba5ff082e4e69926b1c728a8))
* **license:** handle WITH operator for `LaxSplitLicenses` ([#9232](https://github.com/aquasecurity/trivy/issues/9232)) ([b4193d0](https://github.com/aquasecurity/trivy/commit/b4193d0d31a167aafdcd9d9ccd89f3f124eef7ee))
* migrate from `*.list` to `*.md5sums` files for `dpkg` ([#9131](https://github.com/aquasecurity/trivy/issues/9131)) ([f224de3](https://github.com/aquasecurity/trivy/commit/f224de3e39b08672212ec0f94660c36bef77bc30))
* **misconf:** correctly adapt azure storage account ([#9138](https://github.com/aquasecurity/trivy/issues/9138)) ([51aa022](https://github.com/aquasecurity/trivy/commit/51aa0222604829706193eb2ff3a6886742bb42b4))
* **misconf:** correctly parse empty port ranges in google_compute_firewall ([#9237](https://github.com/aquasecurity/trivy/issues/9237)) ([77bab7b](https://github.com/aquasecurity/trivy/commit/77bab7b6d25c712e2db7dc53956985c2721728e9))
* **misconf:** fix log bucket in schema ([#9235](https://github.com/aquasecurity/trivy/issues/9235)) ([7ebc129](https://github.com/aquasecurity/trivy/commit/7ebc129ab726f3133d940708837b7edda2621105))
* **misconf:** skip rewriting expr if attr is nil ([#9113](https://github.com/aquasecurity/trivy/issues/9113)) ([42ccd3d](https://github.com/aquasecurity/trivy/commit/42ccd3df9a7c838a99facb8248e1a68eaf47a999))
* **nodejs:** don't use prerelease logic for compare npm constraints  ([#9208](https://github.com/aquasecurity/trivy/issues/9208)) ([fe96436](https://github.com/aquasecurity/trivy/commit/fe96436b99bae3bbfc7498d2ad222d4acccdfcf1))
* prevent graceful shutdown message on normal exit ([#9244](https://github.com/aquasecurity/trivy/issues/9244)) ([6095984](https://github.com/aquasecurity/trivy/commit/6095984d5340633740204a7a40f002a5643802b9))
* **rootio:** check full version to detect `root.io` packages ([#9117](https://github.com/aquasecurity/trivy/issues/9117)) ([c2ddd44](https://github.com/aquasecurity/trivy/commit/c2ddd44d98594a2066cb5b5acbb9ad2aaad8fd96))
* **rootio:** fix severity selection ([#9181](https://github.com/aquasecurity/trivy/issues/9181)) ([6fafbeb](https://github.com/aquasecurity/trivy/commit/6fafbeb60609a020b47266743250ea847234cbbd))
* **sbom:** merge in-graph and out-of-graph OS packages in scan results ([#9194](https://github.com/aquasecurity/trivy/issues/9194)) ([aa944cc](https://github.com/aquasecurity/trivy/commit/aa944cc6da43e2035f74e9d842f487c0d2f993f4))
* **sbom:** use correct field for licenses in CycloneDX reports ([#9057](https://github.com/aquasecurity/trivy/issues/9057)) ([143da88](https://github.com/aquasecurity/trivy/commit/143da88dd82dfbe204f4c2afe46af3b01701675d))
* **secret:** add UTF-8 validation in secret scanner to prevent protobuf marshalling errors ([#9253](https://github.com/aquasecurity/trivy/issues/9253)) ([54832a7](https://github.com/aquasecurity/trivy/commit/54832a77b50e2da3a3ceacbb6ce1b13e45605cde))
* **secret:** fix line numbers for multiple-line secrets ([#9104](https://github.com/aquasecurity/trivy/issues/9104)) ([e579746](https://github.com/aquasecurity/trivy/commit/e57974649e4a3a275b9cf02db191b3f6bf10340f))
* **server:** add HTTP transport setup to server mode ([#9217](https://github.com/aquasecurity/trivy/issues/9217)) ([1163b04](https://github.com/aquasecurity/trivy/commit/1163b044c7e91a81bba3a862cc4a38e90182f0b4))
* supporting .egg-info/METADATA in python.Packaging analyzer ([#9151](https://github.com/aquasecurity/trivy/issues/9151)) ([e306e2d](https://github.com/aquasecurity/trivy/commit/e306e2dc5275c0e75f056c8c7ee9ff9261c78e7f))
* **terraform:** `for_each` on a map returns a resource for every key ([#9156](https://github.com/aquasecurity/trivy/issues/9156)) ([153318f](https://github.com/aquasecurity/trivy/commit/153318f65f7e5059bcc064bd2cd651cc720791a9))

## [0.64.0](https://github.com/aquasecurity/trivy/compare/v0.63.0...v0.64.0) (2025-06-30)


### Features

* **cli:** add version constraints to annoucements ([#9023](https://github.com/aquasecurity/trivy/issues/9023)) ([19efa9f](https://github.com/aquasecurity/trivy/commit/19efa9fd372242d2ec582a248e9e6573d2caef00))
* **java:** dereference all maven settings.xml env placeholders ([#9024](https://github.com/aquasecurity/trivy/issues/9024)) ([5aade69](https://github.com/aquasecurity/trivy/commit/5aade698c71450badf8db028be61e12ec85c6248))
* **misconf:** add OpenTofu file extension support ([#8747](https://github.com/aquasecurity/trivy/issues/8747)) ([57801d0](https://github.com/aquasecurity/trivy/commit/57801d0324384d990889ba39d856c881e5b8b070))
* **misconf:** normalize CreatedBy for buildah and legacy docker builder ([#8953](https://github.com/aquasecurity/trivy/issues/8953)) ([65e155f](https://github.com/aquasecurity/trivy/commit/65e155fdaf0ad02ec82f00a004427f126faf65ed))
* **redhat:** Add EOL date for RHEL 10. ([#8910](https://github.com/aquasecurity/trivy/issues/8910)) ([48258a7](https://github.com/aquasecurity/trivy/commit/48258a701a7adb210c433310de52f48568ccee19))
* reject unsupported artifact types in remote image retrieval ([#9052](https://github.com/aquasecurity/trivy/issues/9052)) ([1e1e1b5](https://github.com/aquasecurity/trivy/commit/1e1e1b5fa6a884da978fe1ed4c222d613d6eafbd))
* **sbom:** add manufacturer field to CycloneDX tools metadata ([#9019](https://github.com/aquasecurity/trivy/issues/9019)) ([41d0f94](https://github.com/aquasecurity/trivy/commit/41d0f949c874609641c08fa2620fa10bf4ceef78))
* **terraform:** add partial evaluation for policy templates ([#8967](https://github.com/aquasecurity/trivy/issues/8967)) ([a9f7dcd](https://github.com/aquasecurity/trivy/commit/a9f7dcdb9c5973746c3737f2bbc3306a74be5408))
* **ubuntu:** add end of life date for Ubuntu 25.04 ([#9077](https://github.com/aquasecurity/trivy/issues/9077)) ([367564a](https://github.com/aquasecurity/trivy/commit/367564a3bec0c202566c59598dcff087bf50a23d))
* **ubuntu:** add eol date for 20.04-ESM ([#8981](https://github.com/aquasecurity/trivy/issues/8981)) ([87118a0](https://github.com/aquasecurity/trivy/commit/87118a0ec4a6ae492523b7bac9834c2b93a14557))
* **vuln:** add Root.io support for container image scanning ([#9073](https://github.com/aquasecurity/trivy/issues/9073)) ([3a0ec0f](https://github.com/aquasecurity/trivy/commit/3a0ec0f2acff6a13ed6ab348b6b220d49e14a298))


### Bug Fixes

* Add missing version check flags ([#8951](https://github.com/aquasecurity/trivy/issues/8951)) ([ef5f8de](https://github.com/aquasecurity/trivy/commit/ef5f8de8dadf5534a2c965aecca01c7067e5baca))
* **cli:** add some values to the telemetry call ([#9056](https://github.com/aquasecurity/trivy/issues/9056)) ([fd2bc91](https://github.com/aquasecurity/trivy/commit/fd2bc91e133f846bc9f0910c19ac3be3fbfe4009))
* Correctly check for semver versions for trivy version check ([#8948](https://github.com/aquasecurity/trivy/issues/8948)) ([b813527](https://github.com/aquasecurity/trivy/commit/b813527449c4604f5afad71ae82b13399bb48680))
* don't show corrupted trivy-db warning for first run ([#8991](https://github.com/aquasecurity/trivy/issues/8991)) ([4ed78e3](https://github.com/aquasecurity/trivy/commit/4ed78e39afe57e81c12482fef9102dc3f85d1493))
* **misconf:** .Config.User always takes precedence over USER in .History ([#9050](https://github.com/aquasecurity/trivy/issues/9050)) ([371b8cc](https://github.com/aquasecurity/trivy/commit/371b8cc02f2ffa3f42534a437ce8727519e7b9b9))
* **misconf:** correct Azure value-to-time conversion in AsTimeValue ([#9015](https://github.com/aquasecurity/trivy/issues/9015)) ([40d017b](https://github.com/aquasecurity/trivy/commit/40d017b67da38131734eab90c42ad945ac3b5013))
* **misconf:** move disabled checks filtering after analyzer scan ([#9002](https://github.com/aquasecurity/trivy/issues/9002)) ([a58c36d](https://github.com/aquasecurity/trivy/commit/a58c36de124cba7250e1a5ae0cc32d83018391fe))
* **misconf:** reduce log noise on incompatible check ([#9029](https://github.com/aquasecurity/trivy/issues/9029)) ([99c5151](https://github.com/aquasecurity/trivy/commit/99c5151d6ea1dabe85cce75ff9bb91166532b11f))
* **nodejs:** correctly parse `packages` array of `bun.lock` file ([#8998](https://github.com/aquasecurity/trivy/issues/8998)) ([875ec3a](https://github.com/aquasecurity/trivy/commit/875ec3a9d2568e15a6824c8f84ad6a59f03eb212))
* **report:** don't panic when report contains vulns, but doesn't contain packages for `table` format ([#8549](https://github.com/aquasecurity/trivy/issues/8549)) ([87fda76](https://github.com/aquasecurity/trivy/commit/87fda76f38a3a6939a87828c3df0c5ac2cf7fce3))
* **sbom:** remove unnecessary OS detection check in SBOM decoding ([#9034](https://github.com/aquasecurity/trivy/issues/9034)) ([198789a](https://github.com/aquasecurity/trivy/commit/198789a07b857b053c73f8fcd1f508902fac344d))

## [0.63.0](https://github.com/aquasecurity/trivy/compare/v0.62.0...v0.63.0) (2025-05-29)


### Features

* add Bottlerocket OS package analyzer ([#8653](https://github.com/aquasecurity/trivy/issues/8653)) ([07ef63b](https://github.com/aquasecurity/trivy/commit/07ef63b4830f9f3d791a07433287a99118d7590a))
* add JSONC support for comments and trailing commas ([#8862](https://github.com/aquasecurity/trivy/issues/8862)) ([0b0e406](https://github.com/aquasecurity/trivy/commit/0b0e4061ef955efc0f94280d2d390f11ff6e2409))
* **alpine:** add maintainer field extraction for APK packages ([#8930](https://github.com/aquasecurity/trivy/issues/8930)) ([104bbc1](https://github.com/aquasecurity/trivy/commit/104bbc18ea85caec17125296dc4fe2dea9c49826))
* **cli:** Add available version checking ([#8553](https://github.com/aquasecurity/trivy/issues/8553)) ([5a0bf9e](https://github.com/aquasecurity/trivy/commit/5a0bf9ed31ad34248895e69231da602935e66785))
* **echo:** Add Echo Support ([#8833](https://github.com/aquasecurity/trivy/issues/8833)) ([c7b8cc3](https://github.com/aquasecurity/trivy/commit/c7b8cc392eb28eb63e10561cf1ff7991e5e3c548))
* **go:** support license scanning in both GOPATH and vendor ([#8843](https://github.com/aquasecurity/trivy/issues/8843)) ([26437be](https://github.com/aquasecurity/trivy/commit/26437be083960d17bee8b1b37b8a6780eff07981))
* **k8s:** get components from namespaced resources ([#8918](https://github.com/aquasecurity/trivy/issues/8918)) ([4f1ab23](https://github.com/aquasecurity/trivy/commit/4f1ab238693919772a65450de9fb9fb2f873c0d6))
* **license:** improve work text licenses with custom classification ([#8888](https://github.com/aquasecurity/trivy/issues/8888)) ([ee52230](https://github.com/aquasecurity/trivy/commit/ee522300b73a2afc72829fc2fa7ff419712fc89a))
* **license:** improve work with custom classification of licenses from config file ([#8861](https://github.com/aquasecurity/trivy/issues/8861)) ([c321fdf](https://github.com/aquasecurity/trivy/commit/c321fdfcdd58f34d076fc730e2b63fdd13e426a9))
* **license:** scan vendor directory for license for go.mod files ([#8689](https://github.com/aquasecurity/trivy/issues/8689)) ([dd6a6e5](https://github.com/aquasecurity/trivy/commit/dd6a6e50a44b7b543fd9dba634da599a76650acb))
* **license:** Support compound licenses (licenses using SPDX operators) ([#8816](https://github.com/aquasecurity/trivy/issues/8816)) ([39f9ed1](https://github.com/aquasecurity/trivy/commit/39f9ed128b2c0fb599ad9092a3cf5675106bffdc))
* **minimos:** Add support for MinimOS ([#8792](https://github.com/aquasecurity/trivy/issues/8792)) ([c2dde33](https://github.com/aquasecurity/trivy/commit/c2dde33c3f19d499258a7089d7658a9f90722acf))
* **misconf:** add misconfiguration location to junit template ([#8793](https://github.com/aquasecurity/trivy/issues/8793)) ([a516775](https://github.com/aquasecurity/trivy/commit/a516775da6fda92a55a62418a081561127a1d5ca))
* **misconf:** Add support for `Minimum Trivy Version` ([#8880](https://github.com/aquasecurity/trivy/issues/8880)) ([3b2a397](https://github.com/aquasecurity/trivy/commit/3b2a3976ac7e7785828655903b132e84ebd9d727))
* **misconf:** export raw Terraform data to Rego ([#8741](https://github.com/aquasecurity/trivy/issues/8741)) ([aaecc29](https://github.com/aquasecurity/trivy/commit/aaecc29e909db4d5dac03caa0daf223035bfb877))
* **nodejs:** add a bun.lock analyzer ([#8897](https://github.com/aquasecurity/trivy/issues/8897)) ([7ca656d](https://github.com/aquasecurity/trivy/commit/7ca656d54b99346253fc6ac6422eecaca169514e))
* **nodejs:** add bun.lock parser ([#8851](https://github.com/aquasecurity/trivy/issues/8851)) ([1dcf816](https://github.com/aquasecurity/trivy/commit/1dcf81666f1c814600702b9ab603b4070da0b940))
* terraform parser option to set current working directory ([#8909](https://github.com/aquasecurity/trivy/issues/8909)) ([8939451](https://github.com/aquasecurity/trivy/commit/893945117464bf6e090a55e3822f8299825f26d4))


### Bug Fixes

* check post-analyzers for StaticPaths ([#8904](https://github.com/aquasecurity/trivy/issues/8904)) ([93e6680](https://github.com/aquasecurity/trivy/commit/93e6680b1c6bbb590157f521c667c0f611775143))
* **cli:** disable `--skip-dir` and `--skip-files` flags for `sbom` command ([#8886](https://github.com/aquasecurity/trivy/issues/8886)) ([69a5fa1](https://github.com/aquasecurity/trivy/commit/69a5fa18ca86ff7e5206abacf98732d46c000c7a))
* **cli:** don't use allow values for `--compliance` flag ([#8881](https://github.com/aquasecurity/trivy/issues/8881)) ([35e8889](https://github.com/aquasecurity/trivy/commit/35e88890c3c201b3eb11f95376172e57bf44df4b))
* filter all files when processing files installed from package managers ([#8842](https://github.com/aquasecurity/trivy/issues/8842)) ([6ebde88](https://github.com/aquasecurity/trivy/commit/6ebde88dbcaf22f25932bad4844b3c9eaca90560))
* **java:** exclude dev dependencies in gradle lockfile ([#8803](https://github.com/aquasecurity/trivy/issues/8803)) ([8995838](https://github.com/aquasecurity/trivy/commit/8995838e8d184ee9178d5b52d2d3fa9b4e403015))
* julia parser panicing ([#8883](https://github.com/aquasecurity/trivy/issues/8883)) ([be8c7b7](https://github.com/aquasecurity/trivy/commit/be8c7b796dbe36d8dc3889e0bdea23336de9a1ab))
* **julia:** add `Relationship` field support ([#8939](https://github.com/aquasecurity/trivy/issues/8939)) ([22f040f](https://github.com/aquasecurity/trivy/commit/22f040f94790060132c7b0a635f44c35d5a35fb6))
* **k8s:** use in-memory cache backend during misconfig scanning ([#8873](https://github.com/aquasecurity/trivy/issues/8873)) ([fe12771](https://github.com/aquasecurity/trivy/commit/fe127715e505d753e0d878d52c5f280cdc326b76))
* **misconf:** check if for-each is known when expanding dyn block ([#8808](https://github.com/aquasecurity/trivy/issues/8808)) ([5706603](https://github.com/aquasecurity/trivy/commit/570660314698472ab831a7e0d55044e0b1e9c6c0))
* **misconf:** use argument value in WithIncludeDeprecatedChecks ([#8942](https://github.com/aquasecurity/trivy/issues/8942)) ([7e9a54c](https://github.com/aquasecurity/trivy/commit/7e9a54cd6bf4bc15e485c6233d140b389e432fe5))
* more revive rules ([#8814](https://github.com/aquasecurity/trivy/issues/8814)) ([3ab459e](https://github.com/aquasecurity/trivy/commit/3ab459e3b674f319bf349d478917a531a69754c0))
* octalLiteral from go-critic ([#8811](https://github.com/aquasecurity/trivy/issues/8811)) ([a19e0aa](https://github.com/aquasecurity/trivy/commit/a19e0aa1ba0350198c898fd57c9405fbf38fa432))
* **redhat:** Also try to find buildinfo in root layer (layer 0) ([#8924](https://github.com/aquasecurity/trivy/issues/8924)) ([906b037](https://github.com/aquasecurity/trivy/commit/906b037cff97060267d20f8947f429e078419d66))
* **redhat:** save contentSets for OS packages in fs/vm modes ([#8820](https://github.com/aquasecurity/trivy/issues/8820)) ([9256804](https://github.com/aquasecurity/trivy/commit/9256804df8577d8a746fb8b97c508c247ab82f8f))
* **redhat:** trim invalid suffix from content_sets in manifest parsing ([#8818](https://github.com/aquasecurity/trivy/issues/8818)) ([fa1077b](https://github.com/aquasecurity/trivy/commit/fa1077bbf5863a519f6f180a600afe5e2d6180d8))
* **server:** add missed Relationship field for `rpc` ([#8872](https://github.com/aquasecurity/trivy/issues/8872)) ([38f17c9](https://github.com/aquasecurity/trivy/commit/38f17c945e3ef7784607037c0457fb1e06a99959))
* use-any from revive ([#8810](https://github.com/aquasecurity/trivy/issues/8810)) ([883c63b](https://github.com/aquasecurity/trivy/commit/883c63bf29568f0feab37e5d36ae1c417eef88f5))
* **vex:** use `lo.IsNil` to check `VEX` from OCI artifact ([#8858](https://github.com/aquasecurity/trivy/issues/8858)) ([e97af98](https://github.com/aquasecurity/trivy/commit/e97af9806ab13e1ec8b792e0586b486c4982c170))
* **wolfi:** support new APK database location ([#8937](https://github.com/aquasecurity/trivy/issues/8937)) ([b15d9a6](https://github.com/aquasecurity/trivy/commit/b15d9a60e6a3ed40811d5ca6387082266ae92ea7))


### Performance Improvements

* **secret:** only match secrets of meaningful length, allow example strings to not be matched ([#8602](https://github.com/aquasecurity/trivy/issues/8602)) ([60fef1b](https://github.com/aquasecurity/trivy/commit/60fef1b615a765248c5870b814ba0c4345220c0e))

## [0.62.0](https://github.com/aquasecurity/trivy/compare/v0.61.0...v0.62.0) (2025-04-30)


### Features

* **image:** save layers metadata into report ([#8394](https://github.com/aquasecurity/trivy/issues/8394)) ([a95cab0](https://github.com/aquasecurity/trivy/commit/a95cab0eab0fcaab57eb554e74e17da71bc4809f))
* **misconf:** add option to pass Rego scanner to IaC scanner ([#8369](https://github.com/aquasecurity/trivy/issues/8369)) ([890a360](https://github.com/aquasecurity/trivy/commit/890a3602444ad2e5320044c9b8cc79ca883d17ec))
* **misconf:** convert AWS managed policy to document ([#8757](https://github.com/aquasecurity/trivy/issues/8757)) ([7abf5f0](https://github.com/aquasecurity/trivy/commit/7abf5f0199ec65c40056d4f9addc3d27e373725a))
* **misconf:** support auto_provisioning_defaults in google_container_cluster ([#8705](https://github.com/aquasecurity/trivy/issues/8705)) ([9792611](https://github.com/aquasecurity/trivy/commit/9792611b36271efbf79f635deebae7e51f497b70))
* **nodejs:** add root and workspace for `yarn` packages ([#8535](https://github.com/aquasecurity/trivy/issues/8535)) ([bf4cd4f](https://github.com/aquasecurity/trivy/commit/bf4cd4f2d2dda0bb3a7018606db9a6c1e56e4f38))
* **rust:** add root and workspace relationships/package for `cargo` lock files ([#8676](https://github.com/aquasecurity/trivy/issues/8676)) ([93efe07](https://github.com/aquasecurity/trivy/commit/93efe0789ed9d9a71e04e93d87be63032ad9cae7))


### Bug Fixes

* early-return, indent-error-flow and superfluous-else rules from revive  ([#8796](https://github.com/aquasecurity/trivy/issues/8796)) ([43350dd](https://github.com/aquasecurity/trivy/commit/43350dd9b487b39d7d19bd0875274c90262dbed9))
* **k8s:** correct compare artifact versions ([#8682](https://github.com/aquasecurity/trivy/issues/8682)) ([cc47711](https://github.com/aquasecurity/trivy/commit/cc4771158b72b88258057fa379deba9f39190994))
* **k8s:** remove using `last-applied-configuration` ([#8791](https://github.com/aquasecurity/trivy/issues/8791)) ([7a58ccb](https://github.com/aquasecurity/trivy/commit/7a58ccbc7fffdfb1e5ccff9fd4cb6ca08c03a9ea))
* **k8s:** skip passed misconfigs for the summary report ([#8684](https://github.com/aquasecurity/trivy/issues/8684)) ([bff0e9b](https://github.com/aquasecurity/trivy/commit/bff0e9b034f39d0d1ca02457558b1f89847009ac))
* **misconf:** add missing variable as unknown ([#8683](https://github.com/aquasecurity/trivy/issues/8683)) ([9dcd06f](https://github.com/aquasecurity/trivy/commit/9dcd06fda717347eab1ac8ef0710687a3bfd8588))
* **misconf:** check if metadata is not nil ([#8647](https://github.com/aquasecurity/trivy/issues/8647)) ([b7dfd64](https://github.com/aquasecurity/trivy/commit/b7dfd64987b94b4bdd8b7c5a68ba2b8f1a0a9198))
* **misconf:** filter null nodes when parsing json manifest ([#8785](https://github.com/aquasecurity/trivy/issues/8785)) ([e10929a](https://github.com/aquasecurity/trivy/commit/e10929a669f43861bae80652bdfc9f39fad7225f))
* **misconf:** perform operations on attribute safely ([#8774](https://github.com/aquasecurity/trivy/issues/8774)) ([3ce7d59](https://github.com/aquasecurity/trivy/commit/3ce7d59bb16553ab487762a5a660a046bcd63334))
* **misconf:** populate context correctly for module instances ([#8656](https://github.com/aquasecurity/trivy/issues/8656)) ([efd177b](https://github.com/aquasecurity/trivy/commit/efd177b300950d82e381992e1dea39308cc39bc3))
* **report:** clean buffer after flushing ([#8725](https://github.com/aquasecurity/trivy/issues/8725)) ([9a5383e](https://github.com/aquasecurity/trivy/commit/9a5383e993222d919d63f8d9934729cf4e291c06))
* **secret:** ignore .dist-info directories during secret scanning ([#8646](https://github.com/aquasecurity/trivy/issues/8646)) ([a032ad6](https://github.com/aquasecurity/trivy/commit/a032ad696aa58850b9576d889128559149282ad3))
* **server:** fix redis key when trying to delete blob ([#8649](https://github.com/aquasecurity/trivy/issues/8649)) ([36f8d0f](https://github.com/aquasecurity/trivy/commit/36f8d0fd6705bb0da5b43507128c772b153dafec))
* **terraform:** `evaluateStep` to correctly set `EvalContext` for multiple instances of blocks ([#8555](https://github.com/aquasecurity/trivy/issues/8555)) ([e25de25](https://github.com/aquasecurity/trivy/commit/e25de25262fd1cd559879dee07bb2db2747eedd4))
* **terraform:** hcl object expressions to return references ([#8271](https://github.com/aquasecurity/trivy/issues/8271)) ([0d3efa5](https://github.com/aquasecurity/trivy/commit/0d3efa5dc150dba437d975a2f8335de8786f94d6))
* testifylint last issues ([#8768](https://github.com/aquasecurity/trivy/issues/8768)) ([ee4f7dc](https://github.com/aquasecurity/trivy/commit/ee4f7dc6b4be437666e91383406bba8443eec199))
* unused-parameter rule from revive ([#8794](https://github.com/aquasecurity/trivy/issues/8794)) ([6562082](https://github.com/aquasecurity/trivy/commit/6562082e280a9df6199892927f2e3f7dc8f0c8ce))

## [0.61.0](https://github.com/aquasecurity/trivy/compare/v0.60.0...v0.61.0) (2025-03-28)


### Features

* **fs:** optimize scanning performance by direct file access for known paths ([#8525](https://github.com/aquasecurity/trivy/issues/8525)) ([8bf6caf](https://github.com/aquasecurity/trivy/commit/8bf6caf98e2b1eff7bd16987f6791122d827747c))
* **k8s:** add support for controllers ([#8614](https://github.com/aquasecurity/trivy/issues/8614)) ([1bf0117](https://github.com/aquasecurity/trivy/commit/1bf0117f776953bbfe67cf32e4231360010fdf33))
* **misconf:** adapt aws_default_security_group ([#8538](https://github.com/aquasecurity/trivy/issues/8538)) ([b57eccb](https://github.com/aquasecurity/trivy/commit/b57eccb09c33df4ad0423fb148ddeaa292028401))
* **misconf:** adapt aws_opensearch_domain ([#8550](https://github.com/aquasecurity/trivy/issues/8550)) ([9913465](https://github.com/aquasecurity/trivy/commit/9913465a535c29b377bd2f2563163ccf7cbcd6a4))
* **misconf:** adapt AWS::DynamoDB::Table ([#8529](https://github.com/aquasecurity/trivy/issues/8529)) ([8112cdf](https://github.com/aquasecurity/trivy/commit/8112cdf8d638fa2bf57e5687e32f54b704c7e6b7))
* **misconf:** adapt AWS::EC2::VPC ([#8534](https://github.com/aquasecurity/trivy/issues/8534)) ([0d9865f](https://github.com/aquasecurity/trivy/commit/0d9865f48f46e85595af40140faa5ff6f02b9a02))
* **misconf:** Add support for aws_ami ([#8499](https://github.com/aquasecurity/trivy/issues/8499)) ([573502e](https://github.com/aquasecurity/trivy/commit/573502e2e83ff18020d5e7dcad498468a548733e))
* replace TinyGo with standard Go for WebAssembly modules ([#8496](https://github.com/aquasecurity/trivy/issues/8496)) ([529957e](https://github.com/aquasecurity/trivy/commit/529957eac1fc790c57fa3d93524a901ce842a9f5))


### Bug Fixes

* **debian:** don't include empty licenses for `dpkgs` ([#8623](https://github.com/aquasecurity/trivy/issues/8623)) ([346f5b3](https://github.com/aquasecurity/trivy/commit/346f5b3553b9247f99f89d859d4f835e955d34e9))
* **fs:** check postAnalyzers for StaticPaths ([#8543](https://github.com/aquasecurity/trivy/issues/8543)) ([c228307](https://github.com/aquasecurity/trivy/commit/c22830766e8cf1532f20198864757161eed6fda4))
* **k8s:** show report for `--report all` ([#8613](https://github.com/aquasecurity/trivy/issues/8613)) ([dbb6f28](https://github.com/aquasecurity/trivy/commit/dbb6f288712240ef5dec59952e33b73e3a6d5b06))
* **misconf:** add ephemeral block type to config schema ([#8513](https://github.com/aquasecurity/trivy/issues/8513)) ([41512f8](https://github.com/aquasecurity/trivy/commit/41512f846e75bae73984138ad7b3d03284a53f19))
* **misconf:** Check values wholly prior to evalution ([#8604](https://github.com/aquasecurity/trivy/issues/8604)) ([ad58cf4](https://github.com/aquasecurity/trivy/commit/ad58cf4457ebef80ff0bc4c113d4ab4c86a9fe56))
* **misconf:** do not skip loading documents from subdirectories ([#8526](https://github.com/aquasecurity/trivy/issues/8526)) ([de7eb13](https://github.com/aquasecurity/trivy/commit/de7eb13938f2709983a27ab3f59dbfac3fb74651))
* **misconf:** do not use cty.NilVal for non-nil values ([#8567](https://github.com/aquasecurity/trivy/issues/8567)) ([400a79c](https://github.com/aquasecurity/trivy/commit/400a79c2c693e462ad2e1cfc21305ef13d2ec224))
* **misconf:** identify the chart file exactly by name ([#8590](https://github.com/aquasecurity/trivy/issues/8590)) ([ba77dbe](https://github.com/aquasecurity/trivy/commit/ba77dbe5f952d67bbbbc0f43543d5f34135bc280))
* **misconf:** Improve logging for unsupported checks ([#8634](https://github.com/aquasecurity/trivy/issues/8634)) ([5b7704d](https://github.com/aquasecurity/trivy/commit/5b7704d1d091a12822df060ee7a679135185f2ae))
* **misconf:** set default values for AWS::EKS::Cluster.ResourcesVpcConfig ([#8548](https://github.com/aquasecurity/trivy/issues/8548)) ([1f05b45](https://github.com/aquasecurity/trivy/commit/1f05b4545d8f1de3ee703de66a7b3df2baaa07a7))
* **misconf:** skip Azure CreateUiDefinition ([#8503](https://github.com/aquasecurity/trivy/issues/8503)) ([c7814f1](https://github.com/aquasecurity/trivy/commit/c7814f1401b0cc66a557292fe07da24d0ea7b5cc))
* **spdx:** save text licenses into `otherLicenses` without normalize ([#8502](https://github.com/aquasecurity/trivy/issues/8502)) ([e5072f1](https://github.com/aquasecurity/trivy/commit/e5072f1eef8f3a78f4db48b4ac3f7c48aeec5e92))
* use `--file-patterns` flag for all post analyzers ([#7365](https://github.com/aquasecurity/trivy/issues/7365)) ([8b88238](https://github.com/aquasecurity/trivy/commit/8b88238f07e389cc32e2478f84aceaf860e421ef))


### Performance Improvements

* **misconf:** parse input for Rego once ([#8483](https://github.com/aquasecurity/trivy/issues/8483)) ([0e5e909](https://github.com/aquasecurity/trivy/commit/0e5e9097650f60bc54f47a21ecc937a66e66e225))
* **misconf:** retrieve check metadata from annotations once ([#8478](https://github.com/aquasecurity/trivy/issues/8478)) ([7b96351](https://github.com/aquasecurity/trivy/commit/7b96351c32d264d136978fe8fd9e113ada69bb2b))

## [0.60.0](https://github.com/aquasecurity/trivy/compare/v0.59.0...v0.60.0) (2025-03-05)


### Features

* add `--vuln-severity-source` flag ([#8269](https://github.com/aquasecurity/trivy/issues/8269)) ([d464807](https://github.com/aquasecurity/trivy/commit/d4648073211e8451d66e4c0399e9441250b60a76))
* add report summary table ([#8177](https://github.com/aquasecurity/trivy/issues/8177)) ([dd54f80](https://github.com/aquasecurity/trivy/commit/dd54f80d3fda7821dba13553480e9893ba8b4cb3))
* **cyclonedx:** Add initial support for loading external VEX files from SBOM references ([#8254](https://github.com/aquasecurity/trivy/issues/8254)) ([4820eb7](https://github.com/aquasecurity/trivy/commit/4820eb70fc926a35d759c373112dbbdca890fd46))
* **go:** fix parsing main module version for go &gt;= 1.24 ([#8433](https://github.com/aquasecurity/trivy/issues/8433)) ([e58dcfc](https://github.com/aquasecurity/trivy/commit/e58dcfcf9f102c12825d5343ebbcc12a2d6c05c5))
* **misconf:** render causes for Terraform ([#8360](https://github.com/aquasecurity/trivy/issues/8360)) ([a99498c](https://github.com/aquasecurity/trivy/commit/a99498cdd9b7bdac000140af6654bfe30135242d))


### Bug Fixes

* **db:** fix case when 2 trivy-db were copied at the same time ([#8452](https://github.com/aquasecurity/trivy/issues/8452)) ([bb3cca6](https://github.com/aquasecurity/trivy/commit/bb3cca6018551e96fdd357563dc177215ca29bd4))
* don't use `scope` for `trivy registry login` command ([#8393](https://github.com/aquasecurity/trivy/issues/8393)) ([8715e5d](https://github.com/aquasecurity/trivy/commit/8715e5d14a727667c2e62d6f7a4b5308a0323386))
* **go:** merge nested flags into string for ldflags for Go binaries ([#8368](https://github.com/aquasecurity/trivy/issues/8368)) ([b675b06](https://github.com/aquasecurity/trivy/commit/b675b06e897aaf374e7b1262d4323060a8a62edb))
* **image:** disable AVD-DS-0007 for history scanning ([#8366](https://github.com/aquasecurity/trivy/issues/8366)) ([a3cd693](https://github.com/aquasecurity/trivy/commit/a3cd693a5ea88def2f9057df6178b0c0e7a6bdb0))
* **k8s:** add missed option `PkgRelationships` ([#8442](https://github.com/aquasecurity/trivy/issues/8442)) ([f987e41](https://github.com/aquasecurity/trivy/commit/f987e4157494434f6e4e4566fedfedda92167565))
* **misconf:** do not log scanners when misconfig scanning is disabled ([#8345](https://github.com/aquasecurity/trivy/issues/8345)) ([5695eb2](https://github.com/aquasecurity/trivy/commit/5695eb22dfed672eafacb64a71da8e9bdfbaab87))
* **misconf:** ecs include enhanced for container insights ([#8326](https://github.com/aquasecurity/trivy/issues/8326)) ([39789ff](https://github.com/aquasecurity/trivy/commit/39789fff438d11bc6eccd254b3b890beb68c240b))
* **misconf:** fix incorrect k8s locations due to JSON to YAML conversion ([#8073](https://github.com/aquasecurity/trivy/issues/8073)) ([a994453](https://github.com/aquasecurity/trivy/commit/a994453a7d0f543fe30c4dc8adbc92ad0c21bcbc))
* **os:** add mapping OS aliases ([#8466](https://github.com/aquasecurity/trivy/issues/8466)) ([6b4cebe](https://github.com/aquasecurity/trivy/commit/6b4cebe9592f3a06bd91aa58ba6d65869afebbee))
* **python:** add `poetry` v2 support ([#8323](https://github.com/aquasecurity/trivy/issues/8323)) ([10cd98c](https://github.com/aquasecurity/trivy/commit/10cd98cf55263749cb2583063a2e9e9953c7371a))
* **report:** remove html escaping for `shortDescription` and `fullDescription` fields for sarif reports ([#8344](https://github.com/aquasecurity/trivy/issues/8344)) ([3eb0b03](https://github.com/aquasecurity/trivy/commit/3eb0b03f7c9ee462daccfacb291b2c463d848ff5))
* **sbom:** add SBOM file's filePath as Application FilePath if we can't detect its path ([#8346](https://github.com/aquasecurity/trivy/issues/8346)) ([ecc01bb](https://github.com/aquasecurity/trivy/commit/ecc01bb3fb876fd0cc503cb38efa23e4fb9484b4))
* **sbom:** improve logic for binding direct dependency to parent component ([#8489](https://github.com/aquasecurity/trivy/issues/8489)) ([85cca8c](https://github.com/aquasecurity/trivy/commit/85cca8c07affee4ded5c232efb45b05dacf22242))
* **sbom:** preserve OS packages from multiple SBOMs ([#8325](https://github.com/aquasecurity/trivy/issues/8325)) ([bd5baaf](https://github.com/aquasecurity/trivy/commit/bd5baaf93054d71223e0721c7547a0567dea3b02))
* **server:** secrets inspectation for the config analyzer in client server mode ([#8418](https://github.com/aquasecurity/trivy/issues/8418)) ([a1c4bd7](https://github.com/aquasecurity/trivy/commit/a1c4bd746f5f901e2a8f09f48f58b973b9103165))
* **spdx:** init `pkgFilePaths` map for all formats ([#8380](https://github.com/aquasecurity/trivy/issues/8380)) ([72ea4b0](https://github.com/aquasecurity/trivy/commit/72ea4b0632308bd6150aaf2f1549a3f10b60dc23))
* **terraform:** apply parser options to submodule parsing ([#8377](https://github.com/aquasecurity/trivy/issues/8377)) ([398620b](https://github.com/aquasecurity/trivy/commit/398620b471c25e467018bc23df53a3a1c2aa661c))
* update all documentation links ([#8045](https://github.com/aquasecurity/trivy/issues/8045)) ([49456ba](https://github.com/aquasecurity/trivy/commit/49456ba8410e0e4cc1756906ccea1fdd60006d2d))

## [0.59.0](https://github.com/aquasecurity/trivy/compare/v0.58.0...v0.59.0) (2025-01-30)


### Features

* add `--distro` flag to manually specify OS distribution for vulnerability scanning ([#8070](https://github.com/aquasecurity/trivy/issues/8070)) ([da17dc7](https://github.com/aquasecurity/trivy/commit/da17dc72782cd68b5d2c4314a67936343462b75e))
* add a examples field to check metadata ([#8068](https://github.com/aquasecurity/trivy/issues/8068)) ([6d84e0c](https://github.com/aquasecurity/trivy/commit/6d84e0cc0d48ae5c490cad868bb4e5e76392241c))
* add support for registry mirrors ([#8244](https://github.com/aquasecurity/trivy/issues/8244)) ([4316bcb](https://github.com/aquasecurity/trivy/commit/4316bcbc5b9038eed21214a826981c49696bb27f))
* **fs:** use git commit hash as cache key for clean repositories ([#8278](https://github.com/aquasecurity/trivy/issues/8278)) ([b5062f3](https://github.com/aquasecurity/trivy/commit/b5062f3ae20044d1452bf293f210a24cd1d419b3))
* **image:** prevent scanning oversized container images ([#8178](https://github.com/aquasecurity/trivy/issues/8178)) ([509e030](https://github.com/aquasecurity/trivy/commit/509e03030c36d17f9427ab50a4e99fb1846ba65a))
* **image:** return error early if total size of layers exceeds limit ([#8294](https://github.com/aquasecurity/trivy/issues/8294)) ([73bd20d](https://github.com/aquasecurity/trivy/commit/73bd20d6199a777d1ed7eb560e0184d8f1b4b550))
* **k8s:** improve artifact selections for specific namespaces ([#8248](https://github.com/aquasecurity/trivy/issues/8248)) ([db9e57a](https://github.com/aquasecurity/trivy/commit/db9e57a34e460ac6934ee21dffaa2322db9fd56b))
* **misconf:** generate placeholders for random provider resources ([#8051](https://github.com/aquasecurity/trivy/issues/8051)) ([ffe24e1](https://github.com/aquasecurity/trivy/commit/ffe24e18dc3dca816ec9ce5ccf66d5d7b5ea70d6))
* **misconf:** support for ignoring by inline comments for Dockerfile ([#8115](https://github.com/aquasecurity/trivy/issues/8115)) ([c002327](https://github.com/aquasecurity/trivy/commit/c00232720a89df659c6cd0b56d99304d5ffea1a7))
* **misconf:** support for ignoring by inline comments for Helm ([#8138](https://github.com/aquasecurity/trivy/issues/8138)) ([a0429f7](https://github.com/aquasecurity/trivy/commit/a0429f773b4f696fc613d91f1600cd0da38fb2c8))
* **nodejs:** respect peer dependencies for dependency tree ([#7989](https://github.com/aquasecurity/trivy/issues/7989)) ([7389961](https://github.com/aquasecurity/trivy/commit/73899610e8eece670d2e5ddc1478fcc0a2a5760d))
* **python:** add support for poetry dev dependencies ([#8152](https://github.com/aquasecurity/trivy/issues/8152)) ([774e04d](https://github.com/aquasecurity/trivy/commit/774e04d19dc2067725ac2e18ca871872f74082ab))
* **python:** add support for uv ([#8080](https://github.com/aquasecurity/trivy/issues/8080)) ([c4a4a5f](https://github.com/aquasecurity/trivy/commit/c4a4a5fa971d73ae924afcf2259631f15e96e520))
* **python:** add support for uv dev and optional dependencies ([#8134](https://github.com/aquasecurity/trivy/issues/8134)) ([49c54b4](https://github.com/aquasecurity/trivy/commit/49c54b49c6563590dd82007d52e425a7a4e07ac0))


### Bug Fixes

* CVE-2024-45337: Misuse of ServerConfig.PublicKeyCallback may cause authorization bypass ([#8088](https://github.com/aquasecurity/trivy/issues/8088)) ([d7ac286](https://github.com/aquasecurity/trivy/commit/d7ac286085077c969734225a789e6cc056d5c5f5))
* CVE-2025-21613 and CVE-2025-21614 : go-git: argument injection via the URL field ([#8207](https://github.com/aquasecurity/trivy/issues/8207)) ([670fbf2](https://github.com/aquasecurity/trivy/commit/670fbf2d81ea20ea691a86e4ed25a7454baf08e5))
* de-duplicate same `dpkg` packages with different filePaths from different layers ([#8298](https://github.com/aquasecurity/trivy/issues/8298)) ([846498d](https://github.com/aquasecurity/trivy/commit/846498dd23a80531881f803147077eee19004a50))
* enable err-error and errorf rules from perfsprint linter ([#7859](https://github.com/aquasecurity/trivy/issues/7859)) ([156a2aa](https://github.com/aquasecurity/trivy/commit/156a2aa4c49386828c0446f8978473c8da7a8754))
* **flag:** skip hidden flags for `--generate-default-config` command ([#8046](https://github.com/aquasecurity/trivy/issues/8046)) ([5e68bdc](https://github.com/aquasecurity/trivy/commit/5e68bdc9d08f96d22451d7b5dd93e79ca576eeb7))
* **fs:** fix cache key generation to use UUID ([#8275](https://github.com/aquasecurity/trivy/issues/8275)) ([eafd810](https://github.com/aquasecurity/trivy/commit/eafd810d7cb366215efbd0ab3b72c4651d31c6a6))
* handle `BLOW_UNKNOWN` error to download DBs ([#8060](https://github.com/aquasecurity/trivy/issues/8060)) ([51f2123](https://github.com/aquasecurity/trivy/commit/51f2123c5ccc4f7a37d1068830b6670b4ccf9ac8))
* improve conversion of image config to Dockerfile ([#8308](https://github.com/aquasecurity/trivy/issues/8308)) ([2e8e38a](https://github.com/aquasecurity/trivy/commit/2e8e38a8c094f3392893693ab15a605ab0d378f9))
* **java:** correctly overwrite version from depManagement if dependency uses `project.*` props ([#8050](https://github.com/aquasecurity/trivy/issues/8050)) ([9d9f80d](https://github.com/aquasecurity/trivy/commit/9d9f80d9791f38a0b4c727152166ae4d237a83a9))
* **license:** always trim leading and trailing spaces for licenses ([#8095](https://github.com/aquasecurity/trivy/issues/8095)) ([f5e4291](https://github.com/aquasecurity/trivy/commit/f5e429179df1637de96962ab9c19e4336056bb5d))
* **misconf:** allow null values only for tf variables ([#8112](https://github.com/aquasecurity/trivy/issues/8112)) ([23dc3a6](https://github.com/aquasecurity/trivy/commit/23dc3a67535b7458728b2939514a96bd3de3aa81))
* **misconf:** correctly handle all YAML tags in K8S templates ([#8259](https://github.com/aquasecurity/trivy/issues/8259)) ([f12054e](https://github.com/aquasecurity/trivy/commit/f12054e669f9df93c6322ba2755036dbccacaa83))
* **misconf:** disable git terminal prompt on tf module load ([#8026](https://github.com/aquasecurity/trivy/issues/8026)) ([bbc5a85](https://github.com/aquasecurity/trivy/commit/bbc5a85444ec86b7bb26d6db27803d199431a8e6))
* **misconf:** handle heredocs in dockerfile instructions ([#8284](https://github.com/aquasecurity/trivy/issues/8284)) ([0a3887c](https://github.com/aquasecurity/trivy/commit/0a3887ca0350d7dabf5db7e08aaf8152201fdf0d))
* **misconf:** use log instead of fmt for logging ([#8033](https://github.com/aquasecurity/trivy/issues/8033)) ([07b2d7f](https://github.com/aquasecurity/trivy/commit/07b2d7fbd7f8ef5473c2438c560fffc8bdadf913))
* **oracle:** add architectures support for advisories ([#4809](https://github.com/aquasecurity/trivy/issues/4809)) ([90f1d8d](https://github.com/aquasecurity/trivy/commit/90f1d8d78aa20b47fafab2c8ecb07247f075ef45))
* **python:** skip dev group's deps for poetry ([#8106](https://github.com/aquasecurity/trivy/issues/8106)) ([a034d26](https://github.com/aquasecurity/trivy/commit/a034d26443704601c1fe330a5cc1f019f6974524))
* **redhat:** check `usr/share/buildinfo/` dir to detect content sets ([#8222](https://github.com/aquasecurity/trivy/issues/8222)) ([f352f6b](https://github.com/aquasecurity/trivy/commit/f352f6b66355fe3636c9e4e9f3edd089c551a81c))
* **redhat:** correct rewriting of recommendations for the same vulnerability ([#8063](https://github.com/aquasecurity/trivy/issues/8063)) ([4202c4b](https://github.com/aquasecurity/trivy/commit/4202c4ba0d8fcff4b89499fe03050ef4efd37330))
* respect GITHUB_TOKEN to download artifacts from GHCR ([#7580](https://github.com/aquasecurity/trivy/issues/7580)) ([21b68e1](https://github.com/aquasecurity/trivy/commit/21b68e18188f91935ac1055a78ee97a7f35a110d))
* **sbom:** attach nested packages to Application ([#8144](https://github.com/aquasecurity/trivy/issues/8144)) ([735335f](https://github.com/aquasecurity/trivy/commit/735335f08f84936f3928cbbc3eb71af3a3a4918d))
* **sbom:** fix wrong overwriting of applications obtained from different sbom files but having same app type ([#8052](https://github.com/aquasecurity/trivy/issues/8052)) ([fd07074](https://github.com/aquasecurity/trivy/commit/fd07074e8033530eee2732193b00e59f27c73096))
* **sbom:** scan results of SBOMs generated from container images are missing layers ([#7635](https://github.com/aquasecurity/trivy/issues/7635)) ([f9fceb5](https://github.com/aquasecurity/trivy/commit/f9fceb58bf64657dee92302df1ed97e597e474c9))
* **sbom:** use root package for `unknown` dependencies (if exists) ([#8104](https://github.com/aquasecurity/trivy/issues/8104)) ([7558df7](https://github.com/aquasecurity/trivy/commit/7558df7c227c769235e5441fbdd3f9f7efb1ff84))
* **spdx:** use the `hasExtractedLicensingInfos` field for licenses that are not listed in the SPDX ([#8077](https://github.com/aquasecurity/trivy/issues/8077)) ([aec8885](https://github.com/aquasecurity/trivy/commit/aec8885bc7f7e3c5a2a68214dca9aff28accd122))
* **suse:** SUSE - update OSType constants and references for compatility ([#8236](https://github.com/aquasecurity/trivy/issues/8236)) ([ae28398](https://github.com/aquasecurity/trivy/commit/ae283985c926ca828b25b69ad0338008be31e5fe))
* Updated twitter icon ([#7772](https://github.com/aquasecurity/trivy/issues/7772)) ([2c41ac8](https://github.com/aquasecurity/trivy/commit/2c41ac83a95e9347605d36f483171a60ffce0fa2))
* wasm module test ([#8099](https://github.com/aquasecurity/trivy/issues/8099)) ([2200f38](https://github.com/aquasecurity/trivy/commit/2200f3846d675c64ab9302af43224d663a67c944))


### Performance Improvements

* avoid heap allocation in applier findPackage ([#7883](https://github.com/aquasecurity/trivy/issues/7883)) ([9bd6ed7](https://github.com/aquasecurity/trivy/commit/9bd6ed73e5d49d52856c76124e84c268475c5456))

## [0.58.0](https://github.com/aquasecurity/trivy/compare/v0.57.0...v0.58.0) (2024-12-02)


### Features

* add `workspaceRelationship` ([#7889](https://github.com/aquasecurity/trivy/issues/7889)) ([d622ca2](https://github.com/aquasecurity/trivy/commit/d622ca2b1fe40a0eb588478ba9e15d3bd8471a78))
* add cvss v4 score and vector in scan response ([#7968](https://github.com/aquasecurity/trivy/issues/7968)) ([e0f2054](https://github.com/aquasecurity/trivy/commit/e0f2054f9d12dce87e8a0226350f6317f7167195))
* **go:** construct dependencies in the parser ([#7973](https://github.com/aquasecurity/trivy/issues/7973)) ([bcdc0bb](https://github.com/aquasecurity/trivy/commit/bcdc0bbf1f63777ff79d3ecadb8d4f916f376b7d))
* **go:** construct dependencies of `go.mod` main module in the parser ([#7977](https://github.com/aquasecurity/trivy/issues/7977)) ([5448ba2](https://github.com/aquasecurity/trivy/commit/5448ba2a5c1ee36cbcf74ee1c2e83409092c5715))
* **k8s:** add default commands for unknown platform ([#7863](https://github.com/aquasecurity/trivy/issues/7863)) ([b1c7f55](https://github.com/aquasecurity/trivy/commit/b1c7f5516fc39c6cbb76cbeae5c8677ccc9ce5dd))
* **misconf:** log causes of HCL file parsing errors ([#7634](https://github.com/aquasecurity/trivy/issues/7634)) ([e9a899a](https://github.com/aquasecurity/trivy/commit/e9a899a3cfe41a622202808a0241b7f40b54d338))
* **oracle:** add `flavors` support ([#7858](https://github.com/aquasecurity/trivy/issues/7858)) ([b9b383e](https://github.com/aquasecurity/trivy/commit/b9b383eb2714e88357af75900c856db2900b83ec))
* **secret:** Add built-in secrets rules for Private Packagist ([#7826](https://github.com/aquasecurity/trivy/issues/7826)) ([132d9df](https://github.com/aquasecurity/trivy/commit/132d9dfa19a8835c94f332c6939ab7f64641ee5f))
* **suse:** Align SUSE/OpenSUSE OS Identifiers ([#7965](https://github.com/aquasecurity/trivy/issues/7965)) ([45d3b40](https://github.com/aquasecurity/trivy/commit/45d3b40044202dec91384847ce2b50a7271f5977))
* Update registry fallbacks ([#7679](https://github.com/aquasecurity/trivy/issues/7679)) ([5ba9a83](https://github.com/aquasecurity/trivy/commit/5ba9a83a447c4f9e577ae6235c315df71f50b452))


### Bug Fixes

* **alpine:** add `UID` for removed packages ([#7887](https://github.com/aquasecurity/trivy/issues/7887)) ([07915da](https://github.com/aquasecurity/trivy/commit/07915da4816d4d9ec8a6c5e4cba17be2a0f4ad65))
* **aws:** change CPU and Memory type of ContainerDefinition to a string ([#7995](https://github.com/aquasecurity/trivy/issues/7995)) ([aeeba70](https://github.com/aquasecurity/trivy/commit/aeeba70d15c11443d9fe7c26f90fc7d9dcc7f92c))
* **cli:** Handle empty ignore files more gracefully ([#7962](https://github.com/aquasecurity/trivy/issues/7962)) ([4cfb2a9](https://github.com/aquasecurity/trivy/commit/4cfb2a97b27923182ab45c178544542ec65981d4))
* **debian:** infinite loop ([#7928](https://github.com/aquasecurity/trivy/issues/7928)) ([d982e6a](https://github.com/aquasecurity/trivy/commit/d982e6ab89967629f71ec09100cdc61e30a27c63))
* **fs:** add missing defered Cleanup() call to post analyzer fs ([#7882](https://github.com/aquasecurity/trivy/issues/7882)) ([ab32297](https://github.com/aquasecurity/trivy/commit/ab32297e0a8220a427fa330025f8625281e02275))
* Improve version comparisons when build identifiers are present ([#7873](https://github.com/aquasecurity/trivy/issues/7873)) ([eda4d76](https://github.com/aquasecurity/trivy/commit/eda4d7660d8908705bc08a6edc55d8144d02806a))
* **k8s:** check all results for vulnerabilities ([#7946](https://github.com/aquasecurity/trivy/issues/7946)) ([797b36f](https://github.com/aquasecurity/trivy/commit/797b36fbad90b8e7f04e16e2cf08d6bdc0255ac7))
* **misconf:** do not erase variable type for child modules ([#7941](https://github.com/aquasecurity/trivy/issues/7941)) ([de3b7ea](https://github.com/aquasecurity/trivy/commit/de3b7ea24c282bce22ce9cacb49a43d8d90e2bde))
* **misconf:** handle null properties in CloudFormation templates ([#7813](https://github.com/aquasecurity/trivy/issues/7813)) ([99b2db3](https://github.com/aquasecurity/trivy/commit/99b2db3978562689cef956a71281abb84ff0ce47))
* **misconf:** load full Terraform module ([#7925](https://github.com/aquasecurity/trivy/issues/7925)) ([fbc42a0](https://github.com/aquasecurity/trivy/commit/fbc42a04ea24e2246f81491434a965846d55ed69))
* **misconf:** properly resolve local Terraform cache ([#7983](https://github.com/aquasecurity/trivy/issues/7983)) ([fe3a897](https://github.com/aquasecurity/trivy/commit/fe3a8971b6697d896c1ec30b5326a10c20349d14))
* **misconf:** Update trivy-checks default repo to `mirror.gcr.io` ([#7953](https://github.com/aquasecurity/trivy/issues/7953)) ([9988147](https://github.com/aquasecurity/trivy/commit/9988147b8b0e463464fe494122bfcc66ccdf04e0))
* **misconf:** wrap AWS EnvVar to iac types ([#7407](https://github.com/aquasecurity/trivy/issues/7407)) ([54130dc](https://github.com/aquasecurity/trivy/commit/54130dcc1d775506d34b83a558952176fc549914))
* **redhat:** don't return error if `root/buildinfo/content_manifests/` contains files that are not `contentSets` files ([#7912](https://github.com/aquasecurity/trivy/issues/7912)) ([38775a5](https://github.com/aquasecurity/trivy/commit/38775a5ed985eefe2b410e72407c454cdad3d075))
* **report:** handle `git@github.com` schema for misconfigs in `sarif` report ([#7898](https://github.com/aquasecurity/trivy/issues/7898)) ([19aea4b](https://github.com/aquasecurity/trivy/commit/19aea4b01f3ce5a3cd05d5a1091da5b0b3ba4af6))
* **sbom:** Fixes for Programming Language Vulnerabilities and SBOM Package Maintainer Details ([#7871](https://github.com/aquasecurity/trivy/issues/7871)) ([461a68a](https://github.com/aquasecurity/trivy/commit/461a68afd60b77dd67e91047b3b4d558fa5bd2ec))
* **terraform:** set null value as fallback for missing variables ([#7669](https://github.com/aquasecurity/trivy/issues/7669)) ([611558e](https://github.com/aquasecurity/trivy/commit/611558e4ce61818330118684274534f26b1fda99))

## [0.57.0](https://github.com/aquasecurity/trivy/compare/v0.56.0...v0.57.0) (2024-10-31)


### ⚠ BREAKING CHANGES

* **k8s:** support k8s multi container ([#7444](https://github.com/aquasecurity/trivy/issues/7444))

### Features

* add end of life date for Ubuntu 24.10 ([#7787](https://github.com/aquasecurity/trivy/issues/7787)) ([ad3c09e](https://github.com/aquasecurity/trivy/commit/ad3c09e006e134f3c5b879ffc34ce9895a8c860f))
* **cli:** add `trivy auth` ([#7664](https://github.com/aquasecurity/trivy/issues/7664)) ([27117f8](https://github.com/aquasecurity/trivy/commit/27117f81d52483c3ceec56fe56ac298e242fbc9a))
* **cli:** error out when ignore file cannot be found ([#7624](https://github.com/aquasecurity/trivy/issues/7624)) ([cb0b3a9](https://github.com/aquasecurity/trivy/commit/cb0b3a9279b31810ecd686a385e5140e567ce86f))
* **cli:** rename `trivy auth` to `trivy registry` ([#7727](https://github.com/aquasecurity/trivy/issues/7727)) ([633a7ab](https://github.com/aquasecurity/trivy/commit/633a7abeea4287899392a24f2705f96dfeb7e312))
* **cyclonedx:** add file checksums to `CycloneDX` reports ([#7507](https://github.com/aquasecurity/trivy/issues/7507)) ([c225883](https://github.com/aquasecurity/trivy/commit/c225883649f58128a99fa2c1cef327d0e57940be))
* **db:** append errors ([#7843](https://github.com/aquasecurity/trivy/issues/7843)) ([5e78b6c](https://github.com/aquasecurity/trivy/commit/5e78b6c12fb5740c12dedeea3d335d48ec2f752b))
* **misconf:** export unresolvable field of IaC types to Rego ([#7765](https://github.com/aquasecurity/trivy/issues/7765)) ([9514148](https://github.com/aquasecurity/trivy/commit/9514148767865baddd73a49245385574927f7a74))
* **misconf:** public network support for Azure Storage Account ([#7601](https://github.com/aquasecurity/trivy/issues/7601)) ([ad91412](https://github.com/aquasecurity/trivy/commit/ad914123c4d203af1e1da6b7e2d3e49d9d3831d8))
* **misconf:** Show misconfig ID in output ([#7762](https://github.com/aquasecurity/trivy/issues/7762)) ([f75c0d1](https://github.com/aquasecurity/trivy/commit/f75c0d1f0069d4856cb4826d6049f32c5b9409d9))
* **misconf:** ssl_mode support for GCP SQL DB instance ([#7564](https://github.com/aquasecurity/trivy/issues/7564)) ([2eaa17e](https://github.com/aquasecurity/trivy/commit/2eaa17e0717940b27a79050e2efd9213b71178c9))
* **parser:** ignore white space in pom.xml files ([#7747](https://github.com/aquasecurity/trivy/issues/7747)) ([a7baa93](https://github.com/aquasecurity/trivy/commit/a7baa93b00b8636aa097e64cdb8eed97dbd68511))
* **report:** update gitlab template to populate operating_system value ([#7735](https://github.com/aquasecurity/trivy/issues/7735)) ([c0d79fa](https://github.com/aquasecurity/trivy/commit/c0d79fa09e645f3a3dbff878e393b8631fb17b64))


### Bug Fixes

* **cli:** `clean --all` deletes only relevant dirs ([#7704](https://github.com/aquasecurity/trivy/issues/7704)) ([672e886](https://github.com/aquasecurity/trivy/commit/672e886aed152ae0f09a16941706746f3053ca94))
* **cli:** add config name to skip-policy-update alias ([#7820](https://github.com/aquasecurity/trivy/issues/7820)) ([b661d68](https://github.com/aquasecurity/trivy/commit/b661d680ff0372c8e4beea0db13bf69d6a2203a8))
* **db:** fix javadb downloading error handling ([#7642](https://github.com/aquasecurity/trivy/issues/7642)) ([2c87f0c](https://github.com/aquasecurity/trivy/commit/2c87f0cb794acd77446a273582ba1a45b9f18980))
* enable usestdlibvars linter ([#7770](https://github.com/aquasecurity/trivy/issues/7770)) ([57e24aa](https://github.com/aquasecurity/trivy/commit/57e24aa85382f749df7f673e241caaf3fcbb45cb))
* **go:** Do not trim v prefix from versions in Go Mod Analyzer ([#7733](https://github.com/aquasecurity/trivy/issues/7733)) ([e872ec0](https://github.com/aquasecurity/trivy/commit/e872ec006c0745a5a142728af0096c6d6bb9ddf3))
* **helm:** properly handle multiple archived dependencies ([#7782](https://github.com/aquasecurity/trivy/issues/7782)) ([6fab88d](https://github.com/aquasecurity/trivy/commit/6fab88dd56c257ef2cc63b617c2a5decb1c4cf98))
* **java:** correctly inherit `version` and `scope` from upper/root `depManagement` and `dependencies` into parents ([#7541](https://github.com/aquasecurity/trivy/issues/7541)) ([778df82](https://github.com/aquasecurity/trivy/commit/778df828eaad9827cb833c6285058a33aa2b83ca))
* **k8s:** skip resources without misconfigs ([#7797](https://github.com/aquasecurity/trivy/issues/7797)) ([7882776](https://github.com/aquasecurity/trivy/commit/78827768a612ab305bf9c55409ce76d6774302a5))
* **k8s:** support k8s multi container ([#7444](https://github.com/aquasecurity/trivy/issues/7444)) ([c434775](https://github.com/aquasecurity/trivy/commit/c4347759234dcb5f372b07f92fb4230ef391d710))
* **k8s:** support kubernetes v1.31 ([#7810](https://github.com/aquasecurity/trivy/issues/7810)) ([7a4f4d8](https://github.com/aquasecurity/trivy/commit/7a4f4d8b12996687f3095a2042cdf2f5985332c9))
* **license:** fix license normalization for Universal Permissive License ([#7766](https://github.com/aquasecurity/trivy/issues/7766)) ([f6acdf7](https://github.com/aquasecurity/trivy/commit/f6acdf713991f8ffdbe765178fcb8a9cde433cba))
* **misconf:** change default ACL of digitalocean_spaces_bucket to private ([#7577](https://github.com/aquasecurity/trivy/issues/7577)) ([9da84f5](https://github.com/aquasecurity/trivy/commit/9da84f54fadbe6ad0d73983952e945ed63b666f3))
* **misconf:** check if property is not nil before conversion ([#7578](https://github.com/aquasecurity/trivy/issues/7578)) ([c8c14d3](https://github.com/aquasecurity/trivy/commit/c8c14d36245623019f29d258f813d2325f7490f7))
* **misconf:** fix for Azure Storage Account network acls adaptation ([#7602](https://github.com/aquasecurity/trivy/issues/7602)) ([35fd018](https://github.com/aquasecurity/trivy/commit/35fd018ae7ad86823f114f0ac2f1376726aee444))
* **misconf:** properly expand dynamic blocks ([#7612](https://github.com/aquasecurity/trivy/issues/7612)) ([8d5dbc9](https://github.com/aquasecurity/trivy/commit/8d5dbc9fec3569b22ed81a03c40eaf732768718b))
* **redhat:** include arch in PURL qualifiers ([#7654](https://github.com/aquasecurity/trivy/issues/7654)) ([a585e95](https://github.com/aquasecurity/trivy/commit/a585e95f3398631d9ad10505c5ff642fde21aef7))
* **repo:** `git clone` output to Stderr ([#7561](https://github.com/aquasecurity/trivy/issues/7561)) ([fdf203c](https://github.com/aquasecurity/trivy/commit/fdf203cd209aeb40f454bd12d121a54d6ed7a542))
* **report:** Fix invalid URI in SARIF report ([#7645](https://github.com/aquasecurity/trivy/issues/7645)) ([015bb88](https://github.com/aquasecurity/trivy/commit/015bb885ac414b91201fa9791eead395d878149c))
* **sbom:** add options for DBs in private registries ([#7660](https://github.com/aquasecurity/trivy/issues/7660)) ([1f2e91b](https://github.com/aquasecurity/trivy/commit/1f2e91b02b3606dd11963002a8cfac7962f3478f))
* **sbom:** use `Annotation` instead of `AttributionTexts` for `SPDX` formats ([#7811](https://github.com/aquasecurity/trivy/issues/7811)) ([f2bb9c6](https://github.com/aquasecurity/trivy/commit/f2bb9c6227743dd61f44eb591d4b15192fe110c6))

## [0.56.0](https://github.com/aquasecurity/trivy/compare/v0.55.0...v0.56.0) (2024-10-03)


### Features

* **java:** add empty versions if `pom.xml` dependency versions can't be detected ([#7520](https://github.com/aquasecurity/trivy/issues/7520)) ([b836232](https://github.com/aquasecurity/trivy/commit/b8362321adb2af220830c5de31c29978423d47da))
* **license:** improve license normalization ([#7131](https://github.com/aquasecurity/trivy/issues/7131)) ([6472e3c](https://github.com/aquasecurity/trivy/commit/6472e3c9da2a8e7ba41598a45c80df8f18e57d4c))
* **misconf:** add ability to disable checks by ID ([#7536](https://github.com/aquasecurity/trivy/issues/7536)) ([ef0a27d](https://github.com/aquasecurity/trivy/commit/ef0a27d515ff80762bf1959d44a8bde017ae06ec))
* **misconf:** Register checks only when needed ([#7435](https://github.com/aquasecurity/trivy/issues/7435)) ([f768d3a](https://github.com/aquasecurity/trivy/commit/f768d3a767a99a86b0372f19d9f49a2de35dbe59))
* **misconf:** Support `--skip-*` for all included modules  ([#7579](https://github.com/aquasecurity/trivy/issues/7579)) ([c0e8da3](https://github.com/aquasecurity/trivy/commit/c0e8da3828e9d3a0b30d1f6568037db8dc827765))
* **secret:** enhance secret scanning for python binary files ([#7223](https://github.com/aquasecurity/trivy/issues/7223)) ([60725f8](https://github.com/aquasecurity/trivy/commit/60725f879ba014c5c57583db6afc290b78facae8))
* support multiple DB repositories for vulnerability and Java DB ([#7605](https://github.com/aquasecurity/trivy/issues/7605)) ([3562529](https://github.com/aquasecurity/trivy/commit/3562529ddfb26d301311ed450c192e17011353df))
* support RPM archives ([#7628](https://github.com/aquasecurity/trivy/issues/7628)) ([69bf7e0](https://github.com/aquasecurity/trivy/commit/69bf7e00ea5ab483692db830fdded26a31f03183))
* **suse:** added SUSE Linux Enterprise Micro support ([#7294](https://github.com/aquasecurity/trivy/issues/7294)) ([efdb68d](https://github.com/aquasecurity/trivy/commit/efdb68d3b9ddf9dfaf45ea5855b31c43a4366bab))


### Bug Fixes

* allow access to '..' in mapfs ([#7575](https://github.com/aquasecurity/trivy/issues/7575)) ([a8fbe46](https://github.com/aquasecurity/trivy/commit/a8fbe46119adbd89f827a75c75b9e97d392f1842))
* **db:** check `DownloadedAt` for `trivy-java-db` ([#7592](https://github.com/aquasecurity/trivy/issues/7592)) ([13ef3e7](https://github.com/aquasecurity/trivy/commit/13ef3e7d62ba2bcb3a04d7b44f79b1299674b480))
* **java:** use `dependencyManagement` from root/child pom's for dependencies from parents ([#7497](https://github.com/aquasecurity/trivy/issues/7497)) ([5442949](https://github.com/aquasecurity/trivy/commit/54429497e7d6a87eac236771d4efb8a5a7faaac5))
* **license:** stop spliting a long license text ([#7336](https://github.com/aquasecurity/trivy/issues/7336)) ([4926da7](https://github.com/aquasecurity/trivy/commit/4926da79de901fba73819d71845ec0355b68ae0f))
* **misconf:** Disable deprecated checks by default ([#7632](https://github.com/aquasecurity/trivy/issues/7632)) ([82e2adc](https://github.com/aquasecurity/trivy/commit/82e2adc6f8e68d0cc0021031170c2adb60d213ba))
* **misconf:** disable DS016 check for image history analyzer ([#7540](https://github.com/aquasecurity/trivy/issues/7540)) ([de40df9](https://github.com/aquasecurity/trivy/commit/de40df9408d6d856a3ad384ec9f086edce3aa382))
* **misconf:** escape all special sequences ([#7558](https://github.com/aquasecurity/trivy/issues/7558)) ([ea0cf03](https://github.com/aquasecurity/trivy/commit/ea0cf0379aff0348fde87356dab37947800fc1b6))
* **misconf:** Fix logging typo ([#7473](https://github.com/aquasecurity/trivy/issues/7473)) ([56db43c](https://github.com/aquasecurity/trivy/commit/56db43c24f4f6be92891be85faaf9492cad516ac))
* **misconf:** Fixed scope for China Cloud ([#7560](https://github.com/aquasecurity/trivy/issues/7560)) ([37d549e](https://github.com/aquasecurity/trivy/commit/37d549e5b86a1c5dce6710fbfd2310aec9abe949))
* **misconf:** not to warn about missing selectors of libraries ([#7638](https://github.com/aquasecurity/trivy/issues/7638)) ([fcaea74](https://github.com/aquasecurity/trivy/commit/fcaea740808d5784c120e5c5d65f5f94e1d931d4))
* **oracle:** Update EOL date for Oracle 7 ([#7480](https://github.com/aquasecurity/trivy/issues/7480)) ([dd0a64a](https://github.com/aquasecurity/trivy/commit/dd0a64a1cf0cd76e6f81e3ff55fa6ccb95ce3c3d))
* **report:** change a receiver of MarshalJSON ([#7483](https://github.com/aquasecurity/trivy/issues/7483)) ([927c6e0](https://github.com/aquasecurity/trivy/commit/927c6e0c9d4d4a3f1be00f0f661c1d18325d9440))
* **report:** fix error with unmarshal of `ExperimentalModifiedFindings` ([#7463](https://github.com/aquasecurity/trivy/issues/7463)) ([7ff9aff](https://github.com/aquasecurity/trivy/commit/7ff9aff2739b2eee4a98175b98914795e4077060))
* **sbom:** export bom-ref when converting a package to a component ([#7340](https://github.com/aquasecurity/trivy/issues/7340)) ([5dd94eb](https://github.com/aquasecurity/trivy/commit/5dd94ebc1ffe3f1df511dee6381f92a5daefadf2))
* **sbom:** parse type `framework` as `library` when unmarshalling `CycloneDX` files ([#7527](https://github.com/aquasecurity/trivy/issues/7527)) ([aeb7039](https://github.com/aquasecurity/trivy/commit/aeb7039d7ce090e243d29f0bf16c9e4e24252a01))
* **secret:** change grafana token regex to find them without unquoted ([#7627](https://github.com/aquasecurity/trivy/issues/7627)) ([3e1fa21](https://github.com/aquasecurity/trivy/commit/3e1fa2100074e840bacdd65947425b08750b7d9a))


### Performance Improvements

* **misconf:** use port ranges instead of enumeration ([#7549](https://github.com/aquasecurity/trivy/issues/7549)) ([1f9fc13](https://github.com/aquasecurity/trivy/commit/1f9fc13da4a1e7c76c978e4f8e119bfd61a0480e))


### Reverts

* **java:** stop supporting of `test` scope for `pom.xml` files ([#7488](https://github.com/aquasecurity/trivy/issues/7488)) ([b0222fe](https://github.com/aquasecurity/trivy/commit/b0222feeb586ec59904bb321fda8f3f22496d07b))

## [0.55.0](https://github.com/aquasecurity/trivy/compare/v0.54.0...v0.55.0) (2024-09-03)


### ⚠ BREAKING CHANGES

* **cli:** delete deprecated SBOM flags ([#7266](https://github.com/aquasecurity/trivy/issues/7266))

### Features

* **cli:** delete deprecated SBOM flags ([#7266](https://github.com/aquasecurity/trivy/issues/7266)) ([7024572](https://github.com/aquasecurity/trivy/commit/70245721372720027b7089bd61c693df48add865))
* **go:** use `toolchain` as `stdlib` version for `go.mod` files ([#7163](https://github.com/aquasecurity/trivy/issues/7163)) ([2d80769](https://github.com/aquasecurity/trivy/commit/2d80769c34b118851640411fff9dac0b3e353e82))
* **java:** add `test` scope support for `pom.xml` files ([#7414](https://github.com/aquasecurity/trivy/issues/7414)) ([2d97700](https://github.com/aquasecurity/trivy/commit/2d97700d10665142d2f66d7910202bec82116209))
* **misconf:** Add support for using spec from on-disk bundle ([#7179](https://github.com/aquasecurity/trivy/issues/7179)) ([be86126](https://github.com/aquasecurity/trivy/commit/be861265cafc89787fda09c59b2ef175e3d04204))
* **misconf:** ignore duplicate checks ([#7317](https://github.com/aquasecurity/trivy/issues/7317)) ([9ef05fc](https://github.com/aquasecurity/trivy/commit/9ef05fc6b171a264516a025b0b0bcbbc8cff10bc))
* **misconf:** iterator argument support for dynamic blocks ([#7236](https://github.com/aquasecurity/trivy/issues/7236)) ([fe92072](https://github.com/aquasecurity/trivy/commit/fe9207255a4f7f984ec1447f8a9219ae60e560c4))
* **misconf:** port and protocol support for EC2 networks ([#7146](https://github.com/aquasecurity/trivy/issues/7146)) ([98e136e](https://github.com/aquasecurity/trivy/commit/98e136eb7baa2b66f4233d96875c1490144e1594))
* **misconf:** scanning support for YAML and JSON ([#7311](https://github.com/aquasecurity/trivy/issues/7311)) ([efdbd8f](https://github.com/aquasecurity/trivy/commit/efdbd8f19ab0ab0c3b48293d43e51c81b7b03b89))
* **misconf:** support for ignore by nested attributes ([#7205](https://github.com/aquasecurity/trivy/issues/7205)) ([44e4686](https://github.com/aquasecurity/trivy/commit/44e468603d44b077cc4606327fb3e7d7ca435e05))
* **misconf:** support for policy and bucket grants ([#7284](https://github.com/aquasecurity/trivy/issues/7284)) ([a817fae](https://github.com/aquasecurity/trivy/commit/a817fae85b7272b391b737ec86673a7cab722bae))
* **misconf:** variable support for Terraform Plan ([#7228](https://github.com/aquasecurity/trivy/issues/7228)) ([db2c955](https://github.com/aquasecurity/trivy/commit/db2c95598da098ca610825089eb4ab63b789b215))
* **python:** use minimum version for pip packages ([#7348](https://github.com/aquasecurity/trivy/issues/7348)) ([e9b43f8](https://github.com/aquasecurity/trivy/commit/e9b43f81e67789b067352fcb6aa55bc9478bc518))
* **report:** export modified findings in JSON ([#7383](https://github.com/aquasecurity/trivy/issues/7383)) ([7aea79d](https://github.com/aquasecurity/trivy/commit/7aea79dd93cfb61453766dbbb2e3fc0fbd317852))
* **sbom:** set User-Agent header on requests to Rekor ([#7396](https://github.com/aquasecurity/trivy/issues/7396)) ([af1d257](https://github.com/aquasecurity/trivy/commit/af1d257730422d238871beb674767f8f83c5d06a))
* **server:** add internal `--path-prefix` flag for client/server mode ([#7321](https://github.com/aquasecurity/trivy/issues/7321)) ([24a4563](https://github.com/aquasecurity/trivy/commit/24a45636867b893ff54c5ce07197f3b5c6db1d9b))
* **server:** Make Trivy Server Multiplexer Exported ([#7389](https://github.com/aquasecurity/trivy/issues/7389)) ([4c6e8ca](https://github.com/aquasecurity/trivy/commit/4c6e8ca9cc9591799907cc73075f2d740e303b8f))
* **vm:** Support direct filesystem ([#7058](https://github.com/aquasecurity/trivy/issues/7058)) ([45b3f34](https://github.com/aquasecurity/trivy/commit/45b3f344042bcd90ca63ab696b69bff0e9ab4e36))
* **vm:** support the Ext2/Ext3 filesystems ([#6983](https://github.com/aquasecurity/trivy/issues/6983)) ([35c60f0](https://github.com/aquasecurity/trivy/commit/35c60f030fa48de8d8e57958e5ba379814126831))
* **vuln:** Add `--detection-priority` flag for accuracy tuning ([#7288](https://github.com/aquasecurity/trivy/issues/7288)) ([fd8348d](https://github.com/aquasecurity/trivy/commit/fd8348d610f20c6c33da81cd7b0e7d5504ce26be))


### Bug Fixes

* **aws:** handle ECR repositories in different regions ([#6217](https://github.com/aquasecurity/trivy/issues/6217)) ([feaef96](https://github.com/aquasecurity/trivy/commit/feaef9699df5d8ca399770e701a59d7c0ff979a3))
* **flag:** incorrect behavior for deprected flag `--clear-cache` ([#7281](https://github.com/aquasecurity/trivy/issues/7281)) ([2a0e529](https://github.com/aquasecurity/trivy/commit/2a0e529c36057b572119815af59c28e4790034ca))
* **helm:** explicitly define `kind` and `apiVersion` of `volumeClaimTemplate` element ([#7362](https://github.com/aquasecurity/trivy/issues/7362)) ([da4ebfa](https://github.com/aquasecurity/trivy/commit/da4ebfa1a741f3f8b0b43289b4028afe763f7d43))
* **java:** Return error when trying to find a remote pom to avoid segfault ([#7275](https://github.com/aquasecurity/trivy/issues/7275)) ([49d5270](https://github.com/aquasecurity/trivy/commit/49d5270163e305f88fedcf50412973736e69dc69))
* **license:** add license handling to JUnit template ([#7409](https://github.com/aquasecurity/trivy/issues/7409)) ([f80183c](https://github.com/aquasecurity/trivy/commit/f80183c1139b21bb95bc64e216358f4a76001a65))
* logger initialization before flags parsing ([#7372](https://github.com/aquasecurity/trivy/issues/7372)) ([c929290](https://github.com/aquasecurity/trivy/commit/c929290c3c0e4e91337264d69e75ccb60522bc65))
* **misconf:** change default TLS values for the Azure storage account ([#7345](https://github.com/aquasecurity/trivy/issues/7345)) ([aadb090](https://github.com/aquasecurity/trivy/commit/aadb09078843250c66087f46db9a2aa48094a118))
* **misconf:** do not filter Terraform plan JSON by name ([#7406](https://github.com/aquasecurity/trivy/issues/7406)) ([9d7264a](https://github.com/aquasecurity/trivy/commit/9d7264af8e85bcc0dba600b8366d0470d455251c))
* **misconf:** do not recreate filesystem map ([#7416](https://github.com/aquasecurity/trivy/issues/7416)) ([3a5d091](https://github.com/aquasecurity/trivy/commit/3a5d091759564496992a83fb2015a21c84a22213))
* **misconf:** do not register Rego libs in checks registry ([#7420](https://github.com/aquasecurity/trivy/issues/7420)) ([a5aa63e](https://github.com/aquasecurity/trivy/commit/a5aa63eff7e229744090f9ad300c1bec3259397e))
* **misconf:** do not set default value for default_cache_behavior ([#7234](https://github.com/aquasecurity/trivy/issues/7234)) ([f0ed5e4](https://github.com/aquasecurity/trivy/commit/f0ed5e4ced7e60af35c88d5d084aa4b7237f4973))
* **misconf:** fix infer type for null value ([#7424](https://github.com/aquasecurity/trivy/issues/7424)) ([0cac3ac](https://github.com/aquasecurity/trivy/commit/0cac3ac7075017628a21a7990941df04cbc16dbe))
* **misconf:** init frameworks before updating them ([#7376](https://github.com/aquasecurity/trivy/issues/7376)) ([b65b32d](https://github.com/aquasecurity/trivy/commit/b65b32ddfa6fc62ac81ad9fa580e1f5a327864f5))
* **misconf:** load only submodule if it is specified in source ([#7112](https://github.com/aquasecurity/trivy/issues/7112)) ([a4180bd](https://github.com/aquasecurity/trivy/commit/a4180bddd43d86e479edf0afe0c362021d071482))
* **misconf:** support deprecating for Go checks ([#7377](https://github.com/aquasecurity/trivy/issues/7377)) ([2a6c7ab](https://github.com/aquasecurity/trivy/commit/2a6c7ab3b338ce4a8f99d6ac3508c2531dcbe812))
* **misconf:** use module to log when metadata retrieval fails ([#7405](https://github.com/aquasecurity/trivy/issues/7405)) ([0799770](https://github.com/aquasecurity/trivy/commit/0799770b8827a8276ad0d6d9ac7e0381c286757c))
* **misconf:** wrap Azure PortRange in iac types ([#7357](https://github.com/aquasecurity/trivy/issues/7357)) ([c5c62d5](https://github.com/aquasecurity/trivy/commit/c5c62d5ff05420321f9cdbfb93e2591e0866a342))
* **nodejs:** check all `importers` to detect dev deps from pnpm-lock.yaml file ([#7387](https://github.com/aquasecurity/trivy/issues/7387)) ([fd9ed3a](https://github.com/aquasecurity/trivy/commit/fd9ed3a330bc66e229bcbdc262dc296a3bf01f54))
* **plugin:** do not call GitHub content API for releases and tags ([#7274](https://github.com/aquasecurity/trivy/issues/7274)) ([b3ee6da](https://github.com/aquasecurity/trivy/commit/b3ee6dac269bd7847674f3ce985a5ff7f8f0ba38))
* **report:** escape `Message` field in `asff.tpl` template ([#7401](https://github.com/aquasecurity/trivy/issues/7401)) ([dd9733e](https://github.com/aquasecurity/trivy/commit/dd9733e950d3127aa2ac90c45ec7e2b88a2b47ca))
* safely check if the directory exists ([#7353](https://github.com/aquasecurity/trivy/issues/7353)) ([05a8297](https://github.com/aquasecurity/trivy/commit/05a829715f99cd90b122c64cd2f40157854e467b))
* **sbom:** use `NOASSERTION` for licenses fields in SPDX formats ([#7403](https://github.com/aquasecurity/trivy/issues/7403)) ([c96dcdd](https://github.com/aquasecurity/trivy/commit/c96dcdd440a14cdd1b01ac473b2c15e4698e387b))
* **secret:** use `.eyJ` keyword for JWT secret ([#7410](https://github.com/aquasecurity/trivy/issues/7410)) ([bf64003](https://github.com/aquasecurity/trivy/commit/bf64003ac8b209f34b88f228918a96d4f9dac5e0))
* **secret:** use only line with secret for long secret lines ([#7412](https://github.com/aquasecurity/trivy/issues/7412)) ([391448a](https://github.com/aquasecurity/trivy/commit/391448aba9fcb0a4138225e5ab305e4e6707c603))
* **terraform:** add aws_region name to presets ([#7184](https://github.com/aquasecurity/trivy/issues/7184)) ([bb2e26a](https://github.com/aquasecurity/trivy/commit/bb2e26a0ab707b718f6a890cbc87e2492298b6e5))


### Performance Improvements

* **misconf:** do not convert contents of a YAML file to string ([#7292](https://github.com/aquasecurity/trivy/issues/7292)) ([85dadf5](https://github.com/aquasecurity/trivy/commit/85dadf56265647c000191561db10b08a4948c140))
* **misconf:** optimize work with context ([#6968](https://github.com/aquasecurity/trivy/issues/6968)) ([2b6d8d9](https://github.com/aquasecurity/trivy/commit/2b6d8d9227fb6ecc9386a14333964c23c0370a52))
* **misconf:** use json.Valid to check validity of JSON ([#7308](https://github.com/aquasecurity/trivy/issues/7308)) ([c766831](https://github.com/aquasecurity/trivy/commit/c766831069e188226efafeec184e41498685ed85))

## [0.54.0](https://github.com/aquasecurity/trivy/compare/v0.53.0...v0.54.0) (2024-07-30)


### Features

* add `log.FilePath()` function for logger ([#7080](https://github.com/aquasecurity/trivy/issues/7080)) ([1f5f348](https://github.com/aquasecurity/trivy/commit/1f5f34895823fae81bf521fc939bee743a50e304))
* add openSUSE tumbleweed detection and scanning ([#6965](https://github.com/aquasecurity/trivy/issues/6965)) ([17b5dbf](https://github.com/aquasecurity/trivy/commit/17b5dbfa12180414b87859c6c46bfe6cc5ecf7ba))
* **cli:** rename `--vuln-type` flag to `--pkg-types` flag ([#7104](https://github.com/aquasecurity/trivy/issues/7104)) ([7cbdb0a](https://github.com/aquasecurity/trivy/commit/7cbdb0a0b5dff33e506e1c1f3119951fa241b432))
* **mariner:** Add support for Azure Linux ([#7186](https://github.com/aquasecurity/trivy/issues/7186)) ([5cbc452](https://github.com/aquasecurity/trivy/commit/5cbc452a09822d1bf300ead88f0d613d4cf0349a))
* **misconf:** enabled China configuration for ACRs ([#7156](https://github.com/aquasecurity/trivy/issues/7156)) ([d1ec89d](https://github.com/aquasecurity/trivy/commit/d1ec89d1db4b039f0e31076ccd1ca969fb15628e))
* **nodejs:** add license parser to pnpm analyser ([#7036](https://github.com/aquasecurity/trivy/issues/7036)) ([03ac93d](https://github.com/aquasecurity/trivy/commit/03ac93dc208f1b40896f3fa11fa1d45293176dca))
* **sbom:** add image labels into `SPDX` and `CycloneDX` reports ([#7257](https://github.com/aquasecurity/trivy/issues/7257)) ([4a2f492](https://github.com/aquasecurity/trivy/commit/4a2f492c6e685ff577fb96a7006cd0c43755baf4))
* **sbom:** add vulnerability support for SPDX formats ([#7213](https://github.com/aquasecurity/trivy/issues/7213)) ([efb1f69](https://github.com/aquasecurity/trivy/commit/efb1f6938321eec3529ef4fea6608261f6771ae0))
* share build-in rules ([#7207](https://github.com/aquasecurity/trivy/issues/7207)) ([bff317c](https://github.com/aquasecurity/trivy/commit/bff317c77bf4a5f615a80d9875d129213bd52f6d))
* **vex:** retrieve VEX attestations from OCI registries ([#7249](https://github.com/aquasecurity/trivy/issues/7249)) ([c2fd2e0](https://github.com/aquasecurity/trivy/commit/c2fd2e0d89567a0ccd996dda8790f3c3305ea6f7))
* **vex:** VEX Repository support ([#7206](https://github.com/aquasecurity/trivy/issues/7206)) ([88ba460](https://github.com/aquasecurity/trivy/commit/88ba46047c93e6046292523ae701de774dfdc4dc))
* **vuln:** add `--pkg-relationships` ([#7237](https://github.com/aquasecurity/trivy/issues/7237)) ([5c37361](https://github.com/aquasecurity/trivy/commit/5c37361600d922db27dd594b2a80c010a19b3a6e))


### Bug Fixes

* Add dependencyManagement exclusions to the child exclusions ([#6969](https://github.com/aquasecurity/trivy/issues/6969)) ([dc68a66](https://github.com/aquasecurity/trivy/commit/dc68a662a701980d6529f61a65006f1e4728a3e5))
* add missing platform and type to spec ([#7149](https://github.com/aquasecurity/trivy/issues/7149)) ([c8a7abd](https://github.com/aquasecurity/trivy/commit/c8a7abd3b508975fcf10c254d13d1a2cd42da657))
* **cli:** error on missing config file ([#7154](https://github.com/aquasecurity/trivy/issues/7154)) ([7fa5e7d](https://github.com/aquasecurity/trivy/commit/7fa5e7d0ab67f20d434b2922725988695e32e6af))
* close file when failed to open gzip ([#7164](https://github.com/aquasecurity/trivy/issues/7164)) ([2a577a7](https://github.com/aquasecurity/trivy/commit/2a577a7bae37e5731dceaea8740683573b6b70a5))
* **dotnet:** don't include non-runtime libraries into report for `*.deps.json` files ([#7039](https://github.com/aquasecurity/trivy/issues/7039)) ([5bc662b](https://github.com/aquasecurity/trivy/commit/5bc662be9a8f072599f90abfd3b400c8ab055ed6))
* **dotnet:** show `nuget package dir not found` log only when checking `nuget` packages ([#7194](https://github.com/aquasecurity/trivy/issues/7194)) ([d76feba](https://github.com/aquasecurity/trivy/commit/d76febaee107c645e864da0f4d74a8f6ae4ad232))
* ignore nodes when listing permission is not allowed ([#7107](https://github.com/aquasecurity/trivy/issues/7107)) ([25f8143](https://github.com/aquasecurity/trivy/commit/25f8143f120965c636c5ea8386398b211b082398))
* **java:** avoid panic if deps from `pom` in `it` dir are not found ([#7245](https://github.com/aquasecurity/trivy/issues/7245)) ([4e54a7e](https://github.com/aquasecurity/trivy/commit/4e54a7e84c33c1be80c52c6db78c634bc3911715))
* **java:** use `go-mvn-version` to remove `Package` duplicates ([#7088](https://github.com/aquasecurity/trivy/issues/7088)) ([a7a304d](https://github.com/aquasecurity/trivy/commit/a7a304d53e1ce230f881c28c4f35885774cf3b9a))
* **misconf:** do not evaluate TF when a load error occurs ([#7109](https://github.com/aquasecurity/trivy/issues/7109)) ([f27c236](https://github.com/aquasecurity/trivy/commit/f27c236d6e155cb366aeef619b6ea96d20fb93da))
* **nodejs:** detect direct dependencies when using `latest` version for files `yarn.lock` + `package.json` ([#7110](https://github.com/aquasecurity/trivy/issues/7110)) ([54bb8bd](https://github.com/aquasecurity/trivy/commit/54bb8bdfb934d114b5570005853bf4bc0d40c609))
* **report:** hide empty table when all secrets/license/misconfigs are ignored ([#7171](https://github.com/aquasecurity/trivy/issues/7171)) ([c3036de](https://github.com/aquasecurity/trivy/commit/c3036de6d7719323d306a9666ccc8d928d936f9a))
* **secret:** skip regular strings contain secret patterns ([#7182](https://github.com/aquasecurity/trivy/issues/7182)) ([174b1e3](https://github.com/aquasecurity/trivy/commit/174b1e3515a6394cf8d523216d6267c1aefb820a))
* **secret:** trim excessively long lines ([#7192](https://github.com/aquasecurity/trivy/issues/7192)) ([92b13be](https://github.com/aquasecurity/trivy/commit/92b13be668bd20f8e9dac2f0cb8e5a2708b9b3b5))
* **secret:** update length of `hugging-face-access-token` ([#7216](https://github.com/aquasecurity/trivy/issues/7216)) ([8c87194](https://github.com/aquasecurity/trivy/commit/8c87194f0a6b194bc5d340c8a65bd99a3132d973))
* **server:** pass license categories to options ([#7203](https://github.com/aquasecurity/trivy/issues/7203)) ([9d52018](https://github.com/aquasecurity/trivy/commit/9d5201808da89607ae43570bdf1f335b482a6b79))


### Performance Improvements

* **debian:** use `bytes.Index` in `emptyLineSplit` to cut allocation ([#7065](https://github.com/aquasecurity/trivy/issues/7065)) ([acbec05](https://github.com/aquasecurity/trivy/commit/acbec053c985388a26d899e73b4b7f5a6d1fa210))

## [0.53.0](https://github.com/aquasecurity/trivy/compare/v0.52.0...v0.53.0) (2024-07-01)


### ⚠ BREAKING CHANGES

* **k8s:** node-collector dynamic commands support ([#6861](https://github.com/aquasecurity/trivy/issues/6861))
* add clean subcommand ([#6993](https://github.com/aquasecurity/trivy/issues/6993))
* **aws:** Remove aws subcommand ([#6995](https://github.com/aquasecurity/trivy/issues/6995))

### Features

* add clean subcommand ([#6993](https://github.com/aquasecurity/trivy/issues/6993)) ([8d0ae1f](https://github.com/aquasecurity/trivy/commit/8d0ae1f5de72d92a043dcd6b7c164d30e51b6047))
* Add local ImageID to SARIF metadata ([#6522](https://github.com/aquasecurity/trivy/issues/6522)) ([f144e91](https://github.com/aquasecurity/trivy/commit/f144e912d34234f00b5a13b7a11a0019fa978b27))
* add memory cache backend ([#7048](https://github.com/aquasecurity/trivy/issues/7048)) ([55ccd06](https://github.com/aquasecurity/trivy/commit/55ccd06df43f6ff28685f46d215ccb70f55916d2))
* **aws:** Remove aws subcommand ([#6995](https://github.com/aquasecurity/trivy/issues/6995)) ([979e118](https://github.com/aquasecurity/trivy/commit/979e118a9e0ca8943bef9143f492d7eb1fd4d863))
* **conda:** add licenses support for `environment.yml` files ([#6953](https://github.com/aquasecurity/trivy/issues/6953)) ([654217a](https://github.com/aquasecurity/trivy/commit/654217a65485ca0a07771ea61071977894eb4920))
* **dart:** use first version of constraint for dependencies using SDK version ([#6239](https://github.com/aquasecurity/trivy/issues/6239)) ([042d6b0](https://github.com/aquasecurity/trivy/commit/042d6b08c283105c258a3dda98983b345a5305c3))
* **image:** Set User-Agent header for Trivy container registry requests ([#6868](https://github.com/aquasecurity/trivy/issues/6868)) ([9b31697](https://github.com/aquasecurity/trivy/commit/9b31697274c8743d6e5a8f7a1a05daf60cd15910))
* **java:** add support for `maven-metadata.xml` files for remote snapshot repositories. ([#6950](https://github.com/aquasecurity/trivy/issues/6950)) ([1f8fca1](https://github.com/aquasecurity/trivy/commit/1f8fca1fc77b989bb4e3ba820b297464dbdd825f))
* **java:** add support for sbt projects using sbt-dependency-lock ([#6882](https://github.com/aquasecurity/trivy/issues/6882)) ([f18d035](https://github.com/aquasecurity/trivy/commit/f18d035ae13b281c96aa4ed69ca32e507d336e66))
* **k8s:** node-collector dynamic commands support ([#6861](https://github.com/aquasecurity/trivy/issues/6861)) ([8d618e4](https://github.com/aquasecurity/trivy/commit/8d618e48a2f1b60c2e4c49cdd9deb8eb45c972b0))
* **misconf:** add metadata to Cloud schema ([#6831](https://github.com/aquasecurity/trivy/issues/6831)) ([02d5404](https://github.com/aquasecurity/trivy/commit/02d540478d495416b50d7e8b187ff9f5bba41f45))
* **misconf:** add support for AWS::EC2::SecurityGroupIngress/Egress ([#6755](https://github.com/aquasecurity/trivy/issues/6755)) ([55fa610](https://github.com/aquasecurity/trivy/commit/55fa6109cd0463fd3221aae41ca7b1d8c44ad430))
* **misconf:** API Gateway V1 support for CloudFormation ([#6874](https://github.com/aquasecurity/trivy/issues/6874)) ([8491469](https://github.com/aquasecurity/trivy/commit/8491469f0b35bd9df706a433669f5b62239d4ef3))
* **misconf:** support of selectors for all providers for Rego ([#6905](https://github.com/aquasecurity/trivy/issues/6905)) ([bc3741a](https://github.com/aquasecurity/trivy/commit/bc3741ae2c68cdd00fc0aef7e51985568b2eb78a))
* **php:** add installed.json file support ([#4865](https://github.com/aquasecurity/trivy/issues/4865)) ([edc556b](https://github.com/aquasecurity/trivy/commit/edc556b85e3554c31e19b1ece189effb9ba2be12))
* **plugin:** add support for nested archives ([#6845](https://github.com/aquasecurity/trivy/issues/6845)) ([622c67b](https://github.com/aquasecurity/trivy/commit/622c67b7647f94d0a0ca3acf711d8f847cdd8d98))
* **sbom:** migrate to `CycloneDX v1.6` ([#6903](https://github.com/aquasecurity/trivy/issues/6903)) ([09e50ce](https://github.com/aquasecurity/trivy/commit/09e50ce6a82073ba62f1732d5aa0cd2701578693))


### Bug Fixes

* **c:** don't skip conan files from `file-patterns` and scan `.conan2` cache dir ([#6949](https://github.com/aquasecurity/trivy/issues/6949)) ([38b35dd](https://github.com/aquasecurity/trivy/commit/38b35dd3c804027e7a6e6a9d3c87b7ac333896c5))
* **cli:** show info message only when --scanners is available ([#7032](https://github.com/aquasecurity/trivy/issues/7032)) ([e9fc3e3](https://github.com/aquasecurity/trivy/commit/e9fc3e3397564512038ddeca2adce0efcb3f93c5))
* **cyclonedx:** trim non-URL info for `advisory.url` ([#6952](https://github.com/aquasecurity/trivy/issues/6952)) ([417212e](https://github.com/aquasecurity/trivy/commit/417212e0930aa52a27ebdc1b9370d2943ce0f8fa))
* **debian:** take installed files from the origin layer ([#6849](https://github.com/aquasecurity/trivy/issues/6849)) ([089b953](https://github.com/aquasecurity/trivy/commit/089b953462260f01c40bdf588b2568ae0ef658bc))
* **image:** parse `image.inspect.Created` field only for non-empty values ([#6948](https://github.com/aquasecurity/trivy/issues/6948)) ([0af5730](https://github.com/aquasecurity/trivy/commit/0af5730cbe56686417389c2fad643c1bdbb33999))
* **license:** return license separation using separators  `,`, `or`, etc. ([#6916](https://github.com/aquasecurity/trivy/issues/6916)) ([52f7aa5](https://github.com/aquasecurity/trivy/commit/52f7aa54b520a90a19736703f8ea63cc20fab104))
* **misconf:** fix caching of modules in subdirectories ([#6814](https://github.com/aquasecurity/trivy/issues/6814)) ([0bcfedb](https://github.com/aquasecurity/trivy/commit/0bcfedbcaa9bbe30ee5ecade5b98e9ce3cc54c9b))
* **misconf:** fix parsing of engine links and frameworks ([#6937](https://github.com/aquasecurity/trivy/issues/6937)) ([ec68c9a](https://github.com/aquasecurity/trivy/commit/ec68c9ab4580d057720179173d58734402c92af4))
* **misconf:** handle source prefix to ignore ([#6945](https://github.com/aquasecurity/trivy/issues/6945)) ([c3192f0](https://github.com/aquasecurity/trivy/commit/c3192f061d7e84eaf38df8df7c879dc00b4ca137))
* **misconf:** parsing numbers without fraction as int ([#6834](https://github.com/aquasecurity/trivy/issues/6834)) ([8141a13](https://github.com/aquasecurity/trivy/commit/8141a137ba50b553a9da877d95c7ccb491d041c6))
* **nodejs:** fix infinite loop when package link from `package-lock.json` file is broken ([#6858](https://github.com/aquasecurity/trivy/issues/6858)) ([cf5aa33](https://github.com/aquasecurity/trivy/commit/cf5aa336e660e4c98481ebf8d15dd4e54c38581e))
* **nodejs:** fix infinity loops for `pnpm` with cyclic imports ([#6857](https://github.com/aquasecurity/trivy/issues/6857)) ([7d083bc](https://github.com/aquasecurity/trivy/commit/7d083bc890eccc3bf32765c6d7e922cab2e2ef94))
* **plugin:** respect `--insecure` ([#7022](https://github.com/aquasecurity/trivy/issues/7022)) ([3d02a31](https://github.com/aquasecurity/trivy/commit/3d02a31b44924f9e2495aae087f7ca9de3314db4))
* **purl:** add missed os types ([#6955](https://github.com/aquasecurity/trivy/issues/6955)) ([2d85a00](https://github.com/aquasecurity/trivy/commit/2d85a003b22298d1101f84559f7c6b470f2b3909))
* **python:** compare pkg names from `poetry.lock` and `pyproject.toml` in lowercase ([#6852](https://github.com/aquasecurity/trivy/issues/6852)) ([faa9d92](https://github.com/aquasecurity/trivy/commit/faa9d92cfeb8d924deda2dac583b6c97099c08d9))
* **sbom:** don't overwrite `srcEpoch` when decoding SBOM files ([#6866](https://github.com/aquasecurity/trivy/issues/6866)) ([04af59c](https://github.com/aquasecurity/trivy/commit/04af59c2906bcfc7f7970b4e8f45a90f04313170))
* **sbom:** fix panic when scanning SBOM file without root component into SBOM format ([#7051](https://github.com/aquasecurity/trivy/issues/7051)) ([3d4ae8b](https://github.com/aquasecurity/trivy/commit/3d4ae8b5be94cd9b00badeece8d86c2258b2cd90))
* **sbom:** take pkg name from `purl` for maven pkgs ([#7008](https://github.com/aquasecurity/trivy/issues/7008)) ([a76e328](https://github.com/aquasecurity/trivy/commit/a76e3286c413de3dec55394fb41dd627dfee37ae))
* **sbom:** use `purl` for `bitnami` pkg names ([#6982](https://github.com/aquasecurity/trivy/issues/6982)) ([7eabb92](https://github.com/aquasecurity/trivy/commit/7eabb92ec2e617300433445718be07ac74956454))
* **sbom:** use package UIDs for uniqueness ([#7042](https://github.com/aquasecurity/trivy/issues/7042)) ([14d71ba](https://github.com/aquasecurity/trivy/commit/14d71ba63c39e51dd4179ba2d6002b46e1816e90))
* **secret:** `Asymmetric Private Key` shouldn't start with space ([#6867](https://github.com/aquasecurity/trivy/issues/6867)) ([bb26445](https://github.com/aquasecurity/trivy/commit/bb26445e3df198df77930329f532ac5ab7a67af2))
* **suse:** Add SLES 15.6 and Leap 15.6 ([#6964](https://github.com/aquasecurity/trivy/issues/6964)) ([5ee4e9d](https://github.com/aquasecurity/trivy/commit/5ee4e9d30ea814f60fd5705361cabf2e83a47a78))
* use embedded when command path not found ([#7037](https://github.com/aquasecurity/trivy/issues/7037)) ([137c916](https://github.com/aquasecurity/trivy/commit/137c9164238ffd989a0c5ed24f23a55bbf341f6e))

## [0.52.0](https://github.com/aquasecurity/trivy/compare/v0.51.1...v0.52.0) (2024-06-03)


### Features

* Add Julia language analyzer support ([#5635](https://github.com/aquasecurity/trivy/issues/5635)) ([fecafb1](https://github.com/aquasecurity/trivy/commit/fecafb1fc5bb129c7485342a0775f0dd8bedd28e))
* add support for plugin index ([#6674](https://github.com/aquasecurity/trivy/issues/6674)) ([26faf8f](https://github.com/aquasecurity/trivy/commit/26faf8f3f04b1c5f9f81c03ffc6b2008732207e2))
* **misconf:** Add support for deprecating a check ([#6664](https://github.com/aquasecurity/trivy/issues/6664)) ([88702cf](https://github.com/aquasecurity/trivy/commit/88702cfd5918b093defc5b5580f7cbf16f5f2417))
* **misconf:** add Terraform 'removed' block to schema ([#6640](https://github.com/aquasecurity/trivy/issues/6640)) ([b7a0a13](https://github.com/aquasecurity/trivy/commit/b7a0a131a03ed49c08d3b0d481bc9284934fd6e1))
* **misconf:** register builtin Rego funcs from trivy-checks ([#6616](https://github.com/aquasecurity/trivy/issues/6616)) ([7c22ee3](https://github.com/aquasecurity/trivy/commit/7c22ee3df5ee51beb90e44428a99541b3d19ab98))
* **misconf:** resolve tf module from OpenTofu compatible registry ([#6743](https://github.com/aquasecurity/trivy/issues/6743)) ([ac74520](https://github.com/aquasecurity/trivy/commit/ac7452009bf7ca0fa8ee1de8807c792eabad405a))
* **misconf:** support for VPC resources for inbound/outbound rules ([#6779](https://github.com/aquasecurity/trivy/issues/6779)) ([349caf9](https://github.com/aquasecurity/trivy/commit/349caf96bc3dd81551d488044f1adfdb947f39fb))
* **misconf:** support symlinks inside of Helm archives ([#6621](https://github.com/aquasecurity/trivy/issues/6621)) ([4eae37c](https://github.com/aquasecurity/trivy/commit/4eae37c52b035b3576361c12f70d3d9517d0a73c))
* **nodejs:** add v9 pnpm lock file support ([#6617](https://github.com/aquasecurity/trivy/issues/6617)) ([1e08648](https://github.com/aquasecurity/trivy/commit/1e0864842e32a709941d4b4e8f521602bcee684d))
* **plugin:** specify plugin version ([#6683](https://github.com/aquasecurity/trivy/issues/6683)) ([d6dc567](https://github.com/aquasecurity/trivy/commit/d6dc56732babbc9d7f788c280a768d8648aa093d))
* **python:** add license support for `requirement.txt` files ([#6782](https://github.com/aquasecurity/trivy/issues/6782)) ([29615be](https://github.com/aquasecurity/trivy/commit/29615be85e8bfeaf5a0cd51829b1898c55fa4274))
* **python:** add line number support for `requirement.txt` files ([#6729](https://github.com/aquasecurity/trivy/issues/6729)) ([2bc54ad](https://github.com/aquasecurity/trivy/commit/2bc54ad2752aba5de4380cb92c13b09c0abefd73))
* **report:** Include licenses and secrets filtered by rego to ModifiedFindings ([#6483](https://github.com/aquasecurity/trivy/issues/6483)) ([fa3cf99](https://github.com/aquasecurity/trivy/commit/fa3cf993eace4be793f85907b42365269c597b91))
* **vex:** improve relationship support in CSAF VEX ([#6735](https://github.com/aquasecurity/trivy/issues/6735)) ([a447f6b](https://github.com/aquasecurity/trivy/commit/a447f6ba94b6f8b14177dc5e4369a788e2020d90))
* **vex:** support non-root components for products in OpenVEX ([#6728](https://github.com/aquasecurity/trivy/issues/6728)) ([9515695](https://github.com/aquasecurity/trivy/commit/9515695d45e9b5c20890e27e21e3ab45bfd4ce5f))


### Bug Fixes

* clean up golangci lint configuration ([#6797](https://github.com/aquasecurity/trivy/issues/6797)) ([62de6f3](https://github.com/aquasecurity/trivy/commit/62de6f3feba6e4c56ad3922441d5b0f150c3d6b7))
* **cli:** always output fatal errors to stderr ([#6827](https://github.com/aquasecurity/trivy/issues/6827)) ([c2b9132](https://github.com/aquasecurity/trivy/commit/c2b9132a7e933a68df4cc0eb86aab23719ded1b5))
* close APKINDEX archive file ([#6672](https://github.com/aquasecurity/trivy/issues/6672)) ([5caf437](https://github.com/aquasecurity/trivy/commit/5caf4377f3a7fcb1f6e1a84c67136ae62d100be3))
* close settings.xml ([#6768](https://github.com/aquasecurity/trivy/issues/6768)) ([9c3e895](https://github.com/aquasecurity/trivy/commit/9c3e895fcb0852c00ac03ed21338768f76b5273b))
* close testfile ([#6830](https://github.com/aquasecurity/trivy/issues/6830)) ([aa0c413](https://github.com/aquasecurity/trivy/commit/aa0c413814e8915b38d2285c6a8ba5bc3f0705b4))
* **conda:** add support `pip` deps for `environment.yml` files ([#6675](https://github.com/aquasecurity/trivy/issues/6675)) ([150a773](https://github.com/aquasecurity/trivy/commit/150a77313e980cd63797a89a03afcbc97b285f38))
* **go:** add only non-empty root modules for `gobinaries` ([#6710](https://github.com/aquasecurity/trivy/issues/6710)) ([c96f2a5](https://github.com/aquasecurity/trivy/commit/c96f2a5b3de820da37e14594dd537c3b0949ae9c))
* **go:** include only `.version`|`.ver` (no prefixes) ldflags for `gobinaries` ([#6705](https://github.com/aquasecurity/trivy/issues/6705)) ([afb4f9d](https://github.com/aquasecurity/trivy/commit/afb4f9dc4730671ba004e1734fa66422c4c86dad))
* Golang version parsing from binaries w/GOEXPERIMENT ([#6696](https://github.com/aquasecurity/trivy/issues/6696)) ([696f2ae](https://github.com/aquasecurity/trivy/commit/696f2ae0ecdd4f90303f41249924a09ace70dd78))
* include packages unless it is not needed ([#6765](https://github.com/aquasecurity/trivy/issues/6765)) ([56dbe1f](https://github.com/aquasecurity/trivy/commit/56dbe1f6768fe67fbc1153b74fde0f83eaa1b281))
* **misconf:** don't shift ignore rule related to code ([#6708](https://github.com/aquasecurity/trivy/issues/6708)) ([39a746c](https://github.com/aquasecurity/trivy/commit/39a746c77837f873e87b81be40676818030f44c5))
* **misconf:** skip Rego errors with a nil location ([#6638](https://github.com/aquasecurity/trivy/issues/6638)) ([a2c522d](https://github.com/aquasecurity/trivy/commit/a2c522ddb229f049999c4ce74ef75a0e0f9fdc62))
* **misconf:** skip Rego errors with a nil location ([#6666](https://github.com/aquasecurity/trivy/issues/6666)) ([a126e10](https://github.com/aquasecurity/trivy/commit/a126e1075a44ef0e40c0dc1e214d1c5955f80242))
* node-collector high and critical cves ([#6707](https://github.com/aquasecurity/trivy/issues/6707)) ([ff32deb](https://github.com/aquasecurity/trivy/commit/ff32deb7bf9163c06963f557228260b3b8c161ed))
* **plugin:** initialize logger ([#6836](https://github.com/aquasecurity/trivy/issues/6836)) ([728e77a](https://github.com/aquasecurity/trivy/commit/728e77a7261dc3fcda1e61e79be066c789bbba0c))
* **python:** add package name and version validation for `requirements.txt` files. ([#6804](https://github.com/aquasecurity/trivy/issues/6804)) ([ea3a124](https://github.com/aquasecurity/trivy/commit/ea3a124fc7162c30c7f1a59bdb28db0b3c8bb86d))
* **report:** hide empty tables if all vulns has been filtered ([#6352](https://github.com/aquasecurity/trivy/issues/6352)) ([3d388d8](https://github.com/aquasecurity/trivy/commit/3d388d8552ef42d4d54176309a38c1879008527b))
* **sbom:** fix panic for `convert` mode when scanning json file derived from sbom file ([#6808](https://github.com/aquasecurity/trivy/issues/6808)) ([f92ea09](https://github.com/aquasecurity/trivy/commit/f92ea096856c7c262b05bd4d31c62689ebafac82))
* use of specified context to obtain cluster name ([#6645](https://github.com/aquasecurity/trivy/issues/6645)) ([39ebed4](https://github.com/aquasecurity/trivy/commit/39ebed45f8c218509d264bd3f3ca548fc33d2b3a))


### Performance Improvements

* **misconf:** parse rego input once ([#6615](https://github.com/aquasecurity/trivy/issues/6615)) ([67c6b1d](https://github.com/aquasecurity/trivy/commit/67c6b1d473999003d682bdb42657bbf3a4a69a9c))
