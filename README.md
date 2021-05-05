
This repository is used to track agreement for the Splunk Code of Conduct and the Splunk Contributor License Agreement.

Splunk developers may opt into this solution by adding `workflows/agreements.yaml` to their github repo in `.github/workflows`

After adding the workflow to the main branch. Enable branch protection for main,develop and any other merge targets with the requirement of passing the agreements status check

Add a repository secret PAT_TOKEN with a github PAT for a service account to your repo.
Add the service account to cla-agreement-svc
