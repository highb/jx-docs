---
title: jx gitops versionstream
linktitle: versionstream
type: docs
description: "Administer the cluster version stream settings"
aliases:
  - jx-gitops_versionstream
---

### Usage

```
jx gitops versionstream
```

### Synopsis

Administer the cluster version stream settings

### Examples

  ```bash
  # switch to LTS (stable) version stream
  jx-gitops versionstream --lts
  
  # switch to latest version stream
  jx-gitops versionstream --latest
  
  # switch to a custom version stream
  jx-gitops versionstream --custom --url https://github.com/foo/bar.git --ref main

  ```

### Options

```
      --custom             Switch the cluster version stream to a custom version stream, requires url and ref flags set
      --directory string   The directory used in the versionstream, defaults to root (default "/")
  -h, --help               help for versionstream
      --latest             Switch the cluster version stream to the latest (latest releases) git repo, https://github.com/jenkins-x/jxr-versions
      --lts                Switch the cluster version stream to the LTS (long term support on monthly release cadence) git repo, https://github.com/jenkins-x/jx3-lts-versions
      --ref string         The kind of git server for the development environment
      --url string         The git URL to clone to fetch the initial set of files for a helm 3 / helmfile based git configuration if this command is not run inside a git clone or against a GitOps based cluster
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
