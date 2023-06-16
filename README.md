# sdcore-cos-config

Configuration files for SD-Core's integration with Canonical's Observability Stack.

## Usage

```console
juju deploy cos-configuration-k8s \
  --config git_repo=https://github.com/canonical/sdcore-cos-configuration \
  --config git_branch=main \
  --config git_depth=1 \
  --config grafana_dashboards_path=grafana_dashboards/sdcore/
juju integrate cos-configuration-k8s grafana
```
