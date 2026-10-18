# render

Personal video render jobs on GitHub Actions (one video, a few parallel chunks).

- `scene.bin` is an AES-256 encrypted bundle (the key lives in a repository secret and on the owner's PC). Nothing readable is stored here besides the workflow.
- Every result comes back sealed the same way (`sealed-*.enc`, artifacts kept 2 days). The logs show timings only.
- Triggered by hand (`workflow_dispatch`) by the owner. Forks cannot read the secret.

This is a personal media project, not a software product; the jobs are kept small (a handful of parallel runs, a few times a month).
