---
title: to text
categories: |
  formats
version: 0.86.0
formats: |
  Converts data into simple text.
usage: |
  Converts data into simple text.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for formats

<div class='command-title'>{{ $frontmatter.formats }}</div>

## Signature

```> to text {flags} ```


## Input/output types:

| input | output |
| ----- | ------ |
| any   | string |

## Examples

Outputs data as simple text
```nu
> 1 | to text
1
```

Outputs external data as simple text
```nu
> git help -a | lines | find -r '^ ' | to text

```

Outputs records as simple text
```nu
> ls | to text

```
