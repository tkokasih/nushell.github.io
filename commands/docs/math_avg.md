---
title: math avg
categories: |
  math
version: 0.86.0
math: |
  Returns the average of a list of numbers.
usage: |
  Returns the average of a list of numbers.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for math

<div class='command-title'>{{ $frontmatter.math }}</div>

## Signature

```> math avg {flags} ```


## Input/output types:

| input          | output   |
| -------------- | -------- |
| list\<duration\> | duration |
| list\<filesize\> | filesize |
| list\<number\>   | number   |
## Examples

Compute the average of a list of numbers
```nu
> [-50 100.0 25] | math avg
25
```
