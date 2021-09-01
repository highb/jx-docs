---
title: jx gitops kustomize
linktitle: kustomize
type: docs
description: "Generates a kustomize layout by comparing a source and target directories"
aliases:
  - jx-gitops_kustomize
---

### Usage

```
jx gitops kustomize
```

### Synopsis

Generates a kustomize layout by comparing a source and target directories.
  
If you are using kpt to consume templates and you make lots of modifications and hit merge/upgrade issues this command lets you reverse engineer kustomize overlays from the changes you have made the to resources.

### Examples

  ```bash
  # reverse engineer kustomize overlays by comparing the source to the current target
  jx-gitops kustomize --source src/base --target config-root --output src/overlays/default

  ```

### Options

```
  -h, --help            help for kustomize
  -o, --output string   the output directory to store the overlays
  -s, --source string   the directory to recursively look for the source *.yaml or *.yml files (default ".")
  -t, --target string   the directory to recursively look for the target *.yaml or *.yml files
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
