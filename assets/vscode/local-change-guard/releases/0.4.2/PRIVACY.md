# Privacy

Local Change Guard is designed to operate entirely on the machine where VS Code runs.

## Data handled

The extension reads repository-relative paths, Git diffs, branch/worktree information, and Local classification metadata required to render the change view. It stores:

- Local hunk assignments under the current worktree's Git metadata directory;
- user-defined worktree display names under the repository's shared Git metadata directory;
- the selected view mode in VS Code extension state.

## Data not collected

The extension contains no telemetry, analytics, advertising, account system, or application-level network client. It does not transmit repository contents, file paths, Git diffs, classifications, or usage information to Oxara or another service.

VS Code, Git, the operating system, remote-development environments, and extension distribution platforms may have their own data practices. Those products are outside this extension's control.

## Deletion

Uninstalling the extension removes its installed code but does not automatically delete repository metadata. This is intentional to prevent loss of classifications. Users may remove `local-change-guard` directories from the applicable Git metadata locations after confirming they no longer need the saved assignments or workspace names.

When a user explicitly deletes an eligible branch workspace through the extension, its display-name metadata is removed only after Git successfully removes the linked worktree. The associated Git branch is preserved. Dirty worktree deletion requires a separate typed confirmation because its staged, working-tree and untracked changes are permanently removed with that checkout.

Privacy questions can be sent to `oxara.dev@gmail.com`.
