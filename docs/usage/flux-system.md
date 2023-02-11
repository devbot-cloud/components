


## Optimized Git clones.

Optimized Git clones decreases resource utilization for GitRepository reconciliations.

When enabled, it avoids full Git clone operations by first checking whether the revision of the last stored artifact is still the head of the remote repository and none of the other factors that contribute to a change in the artifact, like ignore rules and included repositories, have changed. If that is so, the reconciliation is skipped. Else, a full reconciliation is performed as usual.

This feature is enabled by default. It can be disabled by starting the controller with the argument `--feature-gates=OptimizedGitClones=false`

NB: GitRepository objects configured for SemVer or Commit clones are not affected by this functionality.


