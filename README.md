# GitHub Actions

### Workflows, Jobs & Steps

- Workflows
  - Are defined at the repository level.
  - Define which triggers actually start the workflow.
  - Are composed of one or more jobs.
- Jobs
  - Are defined at the workflow level.
  - Define in which execution environment they are run.
  - Are composed of one or more steps.
  - Run in parallel by default.
- Steps
  - Are defined on the job level.
  - Define the actual script or GitHub Action that will be executed.
  - Run sequentially by default.



### Workflow Events

There are many ways we can trigger GitHub workflows:
- Repository Event:
  - Push (Triggered when someone pushes to the repo)
  - Issues (Triggered by variety of events related to issues)
  - Pull request (Triggered by a variety of events related to PRs)
  - Pull Request Review (Triggered by a variety of events related to PR reviews (submitting, editing, deleting))
  - Fork (Triggered when your repository is forked)
- Manual trigger:
  - Triggered via the UI 
  - Triggered via an API call (triggered via GitHub's REST API)
  - Triggered from another workflow (Triggered from within another workflow)
- Schedule:
  - Runs as a cron job