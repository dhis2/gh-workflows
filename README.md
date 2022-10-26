# gh-workflows

Create the file `.github/workflows/verify_commits.yml`. Example of contents:

```
name: 'dhis2: verify (commits)'

on:
    pull_request:
        types: ['opened', 'edited', 'reopened', 'synchronize']

jobs:
    reusable_verify_commit_workflow_job:
        uses: dhis2/gh-workflows/.github/workflows/dhis2-verify-commits.yml@main
```
