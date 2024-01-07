SourcePlugin fails to get command line arguments in a workspace.

```
pnpm install
pnpm typedoc --disableGit
```

Expected: failed because sourceLinkTemplate is not set
Actual: success as `--disableGit` has not been set

The problem does not occur when removing typedoc.json or using entryPointStrategy other than `packages`.
