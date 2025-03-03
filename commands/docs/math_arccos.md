---
title: math arccos
categories: |
  math
version: 0.86.0
math: |
  Returns the arccosine of the number.
usage: |
  Returns the arccosine of the number.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# <code>{{ $frontmatter.title }}</code> for math

<div class='command-title'>{{ $frontmatter.math }}</div>

## Signature

```> math arccos {flags} ```

## Flags

 -  `--degrees, -d`: Return degrees instead of radians


## Input/output types:

| input        | output      |
| ------------ | ----------- |
| list\<number\> | list\<float\> |
| number       | float       |
## Examples

Get the arccosine of 1
```nu
> 1 | math arccos
0
```

Get the arccosine of -1 in degrees
```nu
> -1 | math arccos -d
180
```


**Tips:** Command `math arccos` was not included in the official binaries by default, you have to build it with `--features=extra` flag