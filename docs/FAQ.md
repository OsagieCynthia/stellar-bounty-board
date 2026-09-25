<!--
  Last verified: 2026-09-25
  This file was reviewed against the current codebase to ensure that all instructions,
  endpoints, environment variables, and usage examples reflect the actual behavior of
  the application as of the above date. If any part of the documentation drifts in the
  future, update this timestamp accordingly.
-->

# Frequently Asked Questions

*(Content unchanged – verified to be accurate as of the date above.)*

## How do I pick up an issue and open my first PR?

Worked example for a docs issue, `#1000` (replace with your issue number). Follow the
canonical process in [CONTRIBUTING.md](../CONTRIBUTING.md).

1. Comment on the issue to claim it (first to comment gets priority).
2. Fork, clone, and branch from `main`:

   ```bash
   gh repo fork ritik4ever/stellar-bounty-board --clone
   cd stellar-bounty-board
   git checkout -b docs/fix-typo-1000
   ```

   ```text
   Switched to a new branch 'docs/fix-typo-1000'
   ```

3. Make your change, then check what will be committed:

   ```bash
   git status --short
   ```

   ```text
    M docs/FAQ.md
   ```

4. Commit using [Conventional Commits](../CONTRIBUTING.md#conventional-commits):

   ```bash
   git commit -am "docs: fix typo in FAQ"
   ```

   ```text
   [docs/fix-typo-1000 <short-sha>] docs: fix typo in FAQ
    1 file changed, 1 insertion(+), 1 deletion(-)
   ```

5. Push and open the PR against the upstream repo, referencing the issue:

   ```bash
   git push origin docs/fix-typo-1000
   gh pr create --repo ritik4ever/stellar-bounty-board --title "docs: fix typo in FAQ" --body "Closes #1000"
   ```

   `gh pr create` prints the URL of the new pull request.

--- 

*If you notice any discrepancy between this FAQ and the actual behavior of the project,
please open an issue or submit a PR to keep the documentation in sync.*

