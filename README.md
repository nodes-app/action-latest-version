[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/nodes-app/action-latest-version)

# action-latest-version

This action outputs the latest release version of a GitHub repository.

## Usage

```yml
- name: Get Latest Version
  id: latest-version
  uses: nodes-app/action-latest-version@v1
  with:
    repository: <user/org name>/<repository name>

- name: Output Latest Version
  run: |
    echo "Latest version: ${{ steps.latest-version.outputs.version }}"
```
