---
title: dfr to-jsonl
categories: |
  dataframe
version: 0.86.0
dataframe: |
  Saves dataframe to a JSON lines file.
usage: |
  Saves dataframe to a JSON lines file.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>

## Signature

```> dfr to-jsonl {flags} (file)```

## Parameters

 -  `file`: file path to save dataframe


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Saves dataframe to JSON lines file
```nu
> [[a b]; [1 2] [3 4]] | dfr into-df | dfr to-jsonl test.jsonl

```


**Tips:** Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag