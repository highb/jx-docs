---
title: jx gitops gc activities
linktitle: activities
type: docs
description: "garbage collection for PipelineActivity resources ***Aliases**: pa,act,pr*"
aliases:
  - jx-gitops_gc_activities
---

### Usage

```
jx gitops gc activities
```

### Synopsis

Garbage collect the Jenkins X PipelineActivity resources

### Examples

  ```bash
  # garbage collect PipelineActivity resources
  jx gitops gc activities
  
  # dry run mode
  jx gitops gc pa --dry-run

  ```

### Options

```
  -d, --dry-run                     Dry run mode. If enabled just list the resources that would be removed
  -h, --help                        help for activities
      --pipelinerun-age duration    Maximum age to keep completed PipelineRuns for all pipelines (default 12h0m0s)
      --pr-history-limit int        Minimum number of PipelineActivities to keep around per repository Pull Request (default 2)
      --prowjob-age duration        Maximum age to keep completed ProwJobs for all pipelines (default 168h0m0s)
  -p, --pull-request-age duration   Maximum age to keep PipelineActivities for Pull Requests (default 48h0m0s)
  -r, --release-age duration        Maximum age to keep PipelineActivities for Releases (default 720h0m0s)
  -l, --release-history-limit int   Maximum number of PipelineActivities to keep around per repository release (default 5)
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
