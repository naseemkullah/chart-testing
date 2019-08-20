To use on Google Cloud build, you will need to `git init` and `git remote add`, e.g.:

```
- name: gcr.io/cloud-builders/git
  args: [init]

- name: gcr.io/cloud-builders/git
  args: [remote, add, origin, <remote url>]

- name: quay.io/helmpack/chart-testing
  id: lint-charts
  entrypoint: ct
  args: [lint, --all]
```
