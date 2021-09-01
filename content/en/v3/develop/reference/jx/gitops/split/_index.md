---
title: jx gitops split
linktitle: split
type: docs
description: "Splits any YAML files which define multiple resources into separate files"
aliases:
  - jx-gitops_split
---

### Usage

```
jx gitops split
```

### Synopsis

Splits any YAML files which define multiple resources into separate files

### Examples

  ```bash
  # splits any files containing multiple resources
  jx-gitops split --dir .

  ```

### Options

```
  -d, --dir string   the directory to recursively look for the *.yaml or *.yml files (default ".")
  -h, --help         help for split
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
