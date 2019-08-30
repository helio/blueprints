# Helio Blueprints

[`schema/schema.yml`](schema/schema.yaml) contains a basic [json schema](https://json-schema.org) to validate the manifests against.
[`blueprints`](blueprints) contains the current blueprints.

## Run schema validation

`node.js` and `npm` needs to be installed. Searching for a go version of this is in progress..

Example:
```bash
$ npx pajv validate -s schema/schema.yaml -d blueprints/busybox/manifest.yaml
$ npx pajv validate -s schema/schema.yaml -d blueprints/docker/manifest.yaml
$ npx pajv validate -s schema/schema.yaml -d blueprints/ep85/manifest.yaml
$ npx pajv validate -s schema/schema.yaml -d blueprints/gitlab/manifest.yaml
$ npx pajv validate -s schema/schema.yaml -d blueprints/infinitebox/manifest.yaml
```