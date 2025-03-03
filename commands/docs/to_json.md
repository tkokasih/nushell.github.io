---
title: to json
categories: |
  formats
version: 0.86.0
formats: |
  Converts table data into JSON text.
usage: |
  Converts table data into JSON text.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for formats

<div class='command-title'>{{ $frontmatter.formats }}</div>

## Signature

```> to json {flags} ```

## Flags

 -  `--raw, -r`: remove all of the whitespace
 -  `--indent, -i {number}`: specify indentation width
 -  `--tabs, -t {number}`: specify indentation tab quantity


## Input/output types:

| input | output |
| ----- | ------ |
| any   | string |

## Examples

Outputs a JSON string, with default indentation, representing the contents of this table
```nu
> [a b c] | to json
[
  "a",
  "b",
  "c"
]
```

Outputs a JSON string, with 4-space indentation, representing the contents of this table
```nu
> [Joe Bob Sam] | to json --indent 4
[
    "Joe",
    "Bob",
    "Sam"
]
```

Outputs an unformatted JSON string representing the contents of this table
```nu
> [1 2 3] | to json -r
[1,2,3]
```
