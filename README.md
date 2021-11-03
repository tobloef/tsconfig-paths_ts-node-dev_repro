# Bug repro for inconsistency between `ts-node` and `dev-ts-node`, when using `tsconfig-paths`

When using `ts-node` (`yarn working`), the custom location for the `tsconfig.json`, specified with `--project`, is laoded. But when using `ts-node-dev` (`yarn broken`) it does not work.

To me, this seems like a bug in `ts-node-dev`, as I would expect it to behave the same as `ts-node`. But perhaps not, it may be something with `tsconfig-paths`.
