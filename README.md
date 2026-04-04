# OpSystem.jl

Declarative dynamical system specification compiler — YAML to callable.

## Overview

`OpSystem.jl` is a Julia port of
[ACCIDDA/op_system](https://github.com/ACCIDDA/op_system) (Python). It provides
a declarative specification language for defining trait-structured dynamical
systems, compiling YAML definitions into callable operator-partitioned forms
suitable for numerical integration.

## Status

**Pre-alpha.** Port in progress.

## Related Packages

| Package | Description |
|---------|-------------|
| [op_system](https://github.com/ACCIDDA/op_system) | Original Python implementation |
| [OpEngine.jl](https://github.com/jcm-sci/OpEngine.jl) | Numerical solver (consumes OpSystem output) |
| [ModelCriticism.jl](https://github.com/jcm-sci/ModelCriticism.jl) | Model evaluation framework (downstream consumer) |

## Installation

```julia
using Pkg
Pkg.add("OpSystem")
```

## Development

```bash
julia --project=. -e 'using Pkg; Pkg.instantiate()'
just test
```

## License

MIT
