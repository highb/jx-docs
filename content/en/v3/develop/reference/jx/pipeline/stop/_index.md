---
title: jx pipeline stop
linktitle: stop
type: docs
description: "Stops one or more pipelines ***Aliases**: kill*"
aliases:
  - jx-pipeline_stop
---

### Usage

```
jx pipeline stop
```

### Synopsis

Stops the pipeline build.

### Examples

  ```bash
  # Select the pipeline to stop
  jx pipeline stop
  
  # Stop a pipeline with a filter and a build number
  jx pipeline stop -f myapp -n 2
  
  # Stop a pipeline for a specific org/repo/branch
  jx pipeline stop myorg/myrepo/main
  
  # Stop a pipeline for a specific context and branch
  jx pipeline stop --context pr --branch PR-456

  ```

### Options

```
  -b, --batch-mode         Runs in batch mode without prompting for user input
  -r, --branch string      The branch to filter by
  -n, --build string       The build number to stop
  -c, --context string     The context to filter by
  -f, --filter string      Filters all the available pipeline names
  -h, --help               help for stop
      --log-level string   Sets the logging level. If not specified defaults to $JX_LOG_LEVEL
      --verbose            Enables verbose output. The environment variable JX_LOG_LEVEL has precedence over this flag and allows setting the logging level to any value of: panic, fatal, error, warn, info, debug, trace
```

### Source

[jenkins-x-plugins/jx-pipeline](https://github.com/jenkins-x-plugins/jx-pipeline)
