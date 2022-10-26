# workflow-app-verify-commits

Create the file `.github/workflows/verify_commits.yml` in your repo. Contents:

```
name: 'dhis2: verify (commits)'

on:
    pull_request:
        types: ['opened', 'edited', 'reopened', 'synchronize']

jobs:
    reusable_verify_commit_workflow_job:
        uses: dhis2/workflow-app-verify-commits/.github/workflows/app-verify-commits.yml@main
```
