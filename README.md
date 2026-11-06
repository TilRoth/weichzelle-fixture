# weichzelle-fixture

Test fixture for [weichzelle](https://github.com/TilRoth/weichzelle)'s VM
tests (`cargo vmtest`). Keep it tiny: every test run clones it.

- `mise.toml`: a small project toolchain, installed by provisioning.
- `Dockerfile`: fetches over HTTPS in a build step, through the
  interception CA that `wz-runc` hands to containers.
