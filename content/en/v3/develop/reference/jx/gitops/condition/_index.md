---
title: jx gitops condition
linktitle: condition
type: docs
description: "Runs a command if the condition is true"
aliases:
  - jx-gitops_condition
---

### Usage

```
jx gitops condition [flags] command arguments...
```

### Synopsis

Runs a command if the condition is true

### Examples

  ```bash
  # runs a command if the last commit messsage has a given prefix
  jx-gitops condition --last-commit-msg-prefix 'Merge pull request' -- make all commit push
  
  you can use ! in front of a filter to be the equivalant of not matching the condition. e.g.
  
  # runs a command if the last commit message does not have a given prefix
  jx-gitops condition --last-commit-msg-prefix '!Merge pull request' -- make all commit push

  ```

### Options

```
  -d, --dir string                        the directory to run the git push command from
  -h, --help                              help for condition
      --last-commit-msg-contains string   matches if last-commit-msg contains the given text
      --last-commit-msg-prefix string     matches if last-commit-msg has the given prefix
      --last-commit-msg-suffix string     matches if last-commit-msg has the given suffix
```

### Source

[jenkins-x-plugins/jx-gitops](https://github.com/jenkins-x-plugins/jx-gitops)
