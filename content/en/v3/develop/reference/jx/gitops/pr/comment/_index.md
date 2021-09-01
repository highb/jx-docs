---
title: jx gitops pr comment
linktitle: comment
type: docs
description: "Add comment to the pull request"
aliases:
  - jx-gitops_pr_comment
---

### Usage

```
jx gitops pr comment
```

### Synopsis

Adds a comment to the current pull request

### Examples

  ```bash
  # add comment
  jx-gitops pr comment -c "message from Jenkins X pipeline"

  ```

### Options

```
      --branch string       specifies the branch if not inside a git clone
  -c, --comment string      comment to add
      --dir string          the directory to search for the .git to discover the git source URL (default ".")
      --git-kind string     the kind of git server to connect to
      --git-server string   the git server URL to create the git provider client. If not specified its defaulted from the current source URL
      --git-token string    the git token used to operate on the git repository
  -h, --help                help for comment
      --pr int              the Pull Request number. If not specified we detect it via $PULL_NUMBER or $BRANCH_NAME environment variables
  -r, --repo string         the full git repository name of the form 'owner/name'
      --source-url string   the git source URL of the repository
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
