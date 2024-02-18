# Change Log

All notable changes to the "action-setup-kube-tools" will be documented in this file.

## v0.10.0

- update action to node20

## v0.9.3

- Bump json5 from 2.1.3 to 2.2.3 - [#41](https://github.com/yokawasa/action-setup-kube-tools/pull/41)
- Bump undici from 5.11.0 to 5.19.1 - [#43](https://github.com/yokawasa/action-setup-kube-tools/pull/43)
- upgrade default tools version - [#44](https://github.com/yokawasa/action-setup-kube-tools/pull/44)
  - kubectl from 1.20.2 to  1.24.10
  - kustomize from 4.5.7 to 5.0.0
  - helm from 3.6.3 to 3.11.1
  - conftest from 0.19.0 to 0.39.0
  - yq from 4.7.1 to 4.30.7
  - rancher from 2.4.10 to 2.7.0
  - tilt from 0.18.11 to 0.31.2 
  - skaffold from 1.20.0 to 2.1.0
  - kube-score from 1.10.1 to 1.16.1

## v0.9.2

- upgrade kustomize 4.5.7 by @MichaelSp - [#39](https://github.com/yokawasa/action-setup-kube-tools/pull/39)

## v0.9.1

- Fix the issue : Using the action produces set-output deprecation warnings by @msg-freiheit - [#36](https://github.com/yokawasa/action-setup-kube-tools/issues/36)

## v0.9.0

- Support [kubeconform](https://github.com/yannh/kubeconform) - [#32](https://github.com/yokawasa/action-setup-kube-tools/issues/32)

## v0.8.3

- Upgrade to Node 16 and upgrade GitHub libs by @yhrn in [#31](https://github.com/yokawasa/action-setup-kube-tools/pull/31)

## v0.8.2

- Bump undici from 5.4.0 to 5.5.1 by @dependabot in [#26](https://github.com/yokawasa/action-setup-kube-tools/pull/26)

## v0.8.1

- Bump ajv from 6.10.2 to 6.12.6 by @dependabot in [#20](https://github.com/yokawasa/action-setup-kube-tools/pull/20)
- Bump minimist from 1.2.5 to 1.2.6 by @dependabot in [#21](https://github.com/yokawasa/action-setup-kube-tools/pull/21)
- Fix error in GHA workflow: prettier: not found by @yokawasa in [#25](https://github.com/yokawasa/action-setup-kube-tools/pull/25)

## v0.8.0

- remove `helmv3` parameter and install helm v3 with `helm` parameter - [#19](https://github.com/yokawasa/action-setup-kube-tools/pull/19)
- Instead add `helmv2` parameter to install helm v2

## v0.7.1

- fix: missing v prefix from kubeval and yq - [#16](https://github.com/yokawasa/action-setup-kube-tools/pull/16)
- changed default versions: yq v4.7.1, kubeval v0.16.1

## v0.7.0

- Add fail-fast parameter (fail-fast:true by default) that allows you to choose to fail fast immediately when it fails to download (say due to a bad version) - [#14](https://github.com/yokawasa/action-setup-kube-tools/issues/14)
- Support tool version 'v' prefix. Prior to this, the action only accept the tool version without 'v' prefix, but now the action automatically add/remove the prefix as necessary - [#13](https://github.com/yokawasa/action-setup-kube-tools/issues/13)

## v0.6.0

- add tools setup option to choose which tool to setup - [#8](https://github.com/yokawasa/action-setup-kube-tools/issues/8)
- up default tool versions
  - kubectl: 1.20.2
  - kustomize: 4.0.5
  - helm: 2.17.0
  - helmv3: 3.5.2

## v0.5.0

- Add kube-score - [#10](https://github.com/yokawasa/action-setup-kube-tools/pull/10)
  - https://github.com/zegl/kube-score

## v0.4.0

- Minor markdown cleanup
- Bump `actions/checkout` to v2 in tests and documentation
- Add Tilt and Skaffold - [#6](https://github.com/yokawasa/action-setup-kube-tools/pull/6)
  - https://tilt.dev
  - https://skaffold.dev

## v0.3.0

- Add Rancher CLI - [#4](https://github.com/yokawasa/action-setup-kube-tools/pull/4)
  - https://rancher.com/docs/rancher/v2.x/en/cli/

## v0.2.0

- Bumps @actions/core from 1.2.0 to 1.2.6 - [#2](https://github.com/yokawasa/action-setup-kube-tools/pull/2)

## v0.1.0

- Initial release

Default command versions:
- `kubectl`: `1.18.2`
- `kustomize`: `3.5.5`
- `helm`: `2.16.7`
- `helmv3`: `3.2.1`
- `kubeval`: `0.15.0`
- `conftest`: `0.19.0`
