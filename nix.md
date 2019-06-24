**nix-instantiate**  
`nix-instantiate`
- Convert nix expression to store derivation (i.e. build description).

`--attr/-A attrPath`  
`--expr/-E` interpret expression on CLI instead of list of file names with expressions

example:
`nix-instantiate -E --eval --json --strict "import ./gpio.nix {}" | jq`
* Take expression that imports a function and calls the empty set.
* Evaluate (print), recursively print with strict, convert to json
* Pipe to pretty JSON.

*GCS*  
```
# configs/drone.nix depends on gcs
./circleci.hs gcs
```

**Build store derivation**  
`nix-store --realise`

**Build (= Instantiate + Realise)**  
Builds the derivations in `path`. Creates a local symlink called `result` that points to the `nix-store`.  

`nix-build -A anduril.snkWithoutCuda`  
OR  
`nix-build -E "with import ./default.nix {}; anduril.snkWithoutCuda"`
