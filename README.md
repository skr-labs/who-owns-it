# who-owns-it

A GitHub Action designed to automatically generate, or suggest changes to, a repository's `CODEOWNERS` file.

## Methodology

This action analyzes the history of a repository and generates, or suggest changes to, a repository's `CODEOWNERS` file. It allows for various inputs to drive the behaviour of the action, including how much history to consider, how many owners to suggest based on contributions, and how many contributions to consider before suggesting a code owner.

The action will also implement the ability to review the current `CODEOWNERS` file and remove code owners who no longer exist in the organization, and check for group owners that have no members.

It is intended to be run either at the repository or organization level on a CRON job. It is suggested to run the CRON either weekly, or monthly.
