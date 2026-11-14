# lineageos-xun-ota

Update channel for the LineageOS 22.2 port to the Xiaomi Redmi Pad SE (`xun`).

`xun.json` is the API v2 update JSON the Updater reads through
`lineage.updater.uri`. It lists the newest build only: the file name, size,
SHA-256, ROM type, version and the download URL. The packages live as GitHub
Release assets because the JSON host is static and the artifacts are too large
for Pages.

A publish replaces the single entry and adds a release. The previous release is
kept as a rollback path until the next build is proven. The JSON is served with
a 300 second cache, so the repository API is the authoritative check right
after a publish.
