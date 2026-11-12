# dpoc-aldehyde.carbon

Platform repo for `aldehyde` — the identity platform (hosts Logto — lithium). `platform.yaml` holds the platform facts
(landscapes/stages per PLAN §8, maturity). `infra/app` renders a ConfigMap
`aldehyde-platform` into namespace `aldehyde`; `infra/primordial` is empty-but-valid
(service repos own the dependency records).

TEMPLATE note (argon): not pushed until the drill creates it.

## Release
Push a tag `vX.Y.Z` (needs `DPOC_REG_PASSWORD`): pushes charts
`reg.dpoc.specpenguin.dev/charts/dpoc-aldehyde:X.Y.Z` and `.../dpoc-aldehyde-primordial:X.Y.Z` (no image).
