# Matrix Build Demo (build-4ad9098)

This repository demonstrates a GitHub Actions matrix build with artifact management.

## What this workflow does

- Runs a matrix build with 3 variants (Node 14, 16, 18).
- Each matrix job runs in parallel.
- Each job generates a build artifact file and uploads it using `actions/upload-artifact@v4`.
- Artifacts use the name prefix `build-4ad9098-<variant>`.

## How to trigger

1. Push to `main` (or open a PR) and GitHub Actions will run the workflow.
2. Or manually run the workflow from the Actions tab using **Run workflow** (for `workflow_dispatch`).

## Validation checklist

- At least 3 successful matrix jobs in the latest run.
- At least 3 artifacts uploaded with names like:
  - `build-4ad9098-node14`
  - `build-4ad9098-node16`
  - `build-4ad9098-node18`
- Each artifact must be non-empty. Check the artifact contents in the Actions run.

## Contact

If you need help, contact: **23f3002144@ds.study.iitm.ac.in**
