---
title: dfr dummies
categories: |
  dataframe
version: 0.86.0
dataframe: |
  Creates a new dataframe with dummy variables.
usage: |
  Creates a new dataframe with dummy variables.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>

## Signature

```> dfr dummies {flags} ```

## Flags

 -  `--drop-first, -d`: Drop first row


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Create new dataframe with dummy variables from a dataframe
```nu
> [[a b]; [1 2] [3 4]] | dfr into-df | dfr dummies
╭───┬─────┬─────┬─────┬─────╮
│ # │ a_1 │ a_3 │ b_2 │ b_4 │
├───┼─────┼─────┼─────┼─────┤
│ 0 │   1 │   0 │   1 │   0 │
│ 1 │   0 │   1 │   0 │   1 │
╰───┴─────┴─────┴─────┴─────╯

```

Create new dataframe with dummy variables from a series
```nu
> [1 2 2 3 3] | dfr into-df | dfr dummies
╭───┬─────┬─────┬─────╮
│ # │ 0_1 │ 0_2 │ 0_3 │
├───┼─────┼─────┼─────┤
│ 0 │   1 │   0 │   0 │
│ 1 │   0 │   1 │   0 │
│ 2 │   0 │   1 │   0 │
│ 3 │   0 │   0 │   1 │
│ 4 │   0 │   0 │   1 │
╰───┴─────┴─────┴─────╯

```


**Tips:** Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag