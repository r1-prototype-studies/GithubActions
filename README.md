<h1> Github Actions <h1>

- [Notes](#notes)
- [Commands](#commands)
- [References](#references)

# Notes
* For troubleshooting purpose, add "ACTIONS_RUNNER_DEBUG" with value as "true" and "ACTIONS_STEP_DEBUG" with value as "true" in secrets in github settings.
* In `uses`, we can use any of the below 
  * Branch name (not preferred)
  * Release tag
  * commit id
* ``steps`` can be used to refer to other steps by their ids like
   ```
   {{ steps.greet.outputs.time}}
* Workflow can be triggered from github events.
* Use cron schedule to trigger the workflow at specified time.
* The minimum schedule of a workflow is every 5 mins.
* Branch matching
 ```
  - 'feature/*'    # matches feature/feature1 and doesn't match feature/a/fet
  - 'feature/**'   # matches feature/feature1 feature/a/fet
* We cannot have branches and branches ignore at the same time
* 

# Commands

| Commands | Example | Description                                            |
| -------- | ------- | ------------------------------------------------------ |
| >        |         | Long text in separate lines without new line character |
| \|       |         | Long text in separate lines with new line character    |

# References
* https://dev.to/pwd9000/github-actions-all-the-shells-581h
* https://github.com/actions/hello-world-javascript-action
* https://github.com/actions/checkout
* https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows
* https://crontab.guru/#*_*_*_*_*
* https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event
* https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet
* 

