---
title: jx gitops rename
linktitle: rename
type: docs
description: "Renames yaml files to use canonical file names based on the resource name and kind"
aliases:
  - jx-gitops_rename
---

### Usage

```
jx gitops rename
```

### Synopsis

Renames yaml files to use canonical file names based on the resource name and kind

### Examples

  ```bash
  # renames files to use a canonical file name
  jx-gitops rename --dir .

  ```

### Options

```
  -d, --dir string   the directory to recursively look for the *.yaml or *.yml files (default ".")
  -h, --help         help for rename
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
