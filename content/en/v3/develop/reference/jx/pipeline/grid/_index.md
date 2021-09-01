---
title: jx pipeline grid
linktitle: grid
type: docs
description: "Watches pipeline activity in a table ***Aliases**: table,tbl*"
aliases:
  - jx-pipeline_grid
---

### Usage

```
jx pipeline grid
```

### Synopsis

Watches pipeline activity in a table

You can use the up/down cursor keys to select a pipeline then hit enter on the selected pipeline to view its log. When the pipeline is completed you can then go back to the pipeline grid and view other pipelines.

### Examples

  ```bash
  # Watches the current pipeline activities in a grid
  jx pipeline grid
  
  # Watches the current pipeline activities which have a name containing 'foo'
  jx pipeline grid -f foo

  ```

### Options

```
  -b, --batch-mode         Runs in batch mode without prompting for user input
      --fail-with-pod      Return an error if the pod fails
  -f, --filter string      Text to filter the pipeline names
  -h, --help               help for grid
      --log-level string   Sets the logging level. If not specified defaults to $JX_LOG_LEVEL
      --verbose            Enables verbose output. The environment variable JX_LOG_LEVEL has precedence over this flag and allows setting the logging level to any value of: panic, fatal, error, warn, info, debug, trace
```

### Source

[jenkins-x-plugins/jx-pipeline](https://github.com/jenkins-x-plugins/jx-pipeline)
