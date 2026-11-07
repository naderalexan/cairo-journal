# Ponytail

Use the full Ponytail workflow for implementation tasks. Follow a narrower level when the user requests one, and stop the workflow if they ask.

## Workflow

1. **Establish the task.** Read the applicable repository instructions and relevant domain or issue-tracker docs. Inspect the provided issue or spec, the affected code, and the current worktree. Identify existing edits that are outside this task and preserve them.
2. **Trace the behavior.** Follow the existing path from user-visible behavior to the relevant implementation and tests. Turn the request into concrete acceptance criteria; ask a focused question only if an unresolved choice would change the implementation.
3. **Choose the smallest complete change.** Prefer existing project patterns and public seams. Avoid speculative features, unrelated refactors, and new dependencies unless the task requires them.
4. **Implement and document.** Make the change and update relevant tests or documentation when behavior or contracts change. Keep the patch limited to the accepted scope.
5. **Verify and review.** Run the checks that cover the changed behavior when appropriate. Inspect the final diff and worktree to confirm the acceptance criteria are met, unrelated edits remain intact, and no generated or incidental files entered the change.
6. **Report the result.** Summarize what changed, the verification performed and its outcome, and any remaining limitation.

The workflow is complete when each acceptance criterion has evidence in the implementation or verification, the final diff has been reviewed, and the result report states any unchecked areas.
