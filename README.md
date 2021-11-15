# HMM tests

Tests with a simple HMM models.

The model tries to infer the current position `x` and the observation noise `sigma2`.

## Requirements
- [Opam](https://opam.ocaml.org/) with Ocaml >= 4.10
- [ProbZelus](https://github.com/IBM/probzelus) with Zelus-libs

## Build and run

```
dune exec ./hmm_main.exe 
```

You can try other inference algorithms by changing the line `open Infer_ds_streaming` in the file `hmm.zls` with one of the following:

- `Infer_ds_streaming`
- `Infer_pf`
- `Infer_importance`
- `Infer_ds_naive`
