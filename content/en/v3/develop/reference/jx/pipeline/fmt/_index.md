---
title: jx pipeline fmt
linktitle: fmt
type: docs
description: "Formats the local pipeline files"
aliases:
  - jx-pipeline_fmt
---

### Usage

```
jx pipeline fmt
```

### Synopsis

Formats the local pipeline files

* removes any unnecessary parameters  
* converts any shell commands to use 'script:' notation

### Examples

  ```bash
  # Formats the local pipeline files
  jx pipeline fmt

  ```

### Options

```
  -d, --dir string   The directory to look for the tekton YAML files (default ".lighthouse")
  -h, --help         help for fmt
      --sha string   The git commit SHA of the pipeline catalog repository https://github.com/jenkins-x/jx3-pipeline-catalog. If not specified we clone git and find it
```

### Source

[jenkins-x-plugins/jx-pipeline](https://github.com/jenkins-x-plugins/jx-pipeline)
