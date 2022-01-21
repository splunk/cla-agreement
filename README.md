
# CLA Agreement Tracker

## Overview

The “CLA” lite tool uses Github to track users who have agreed to the CLA for /splunk projects. Developers can rely on CI checks to determine if a PR from an outside source can be merged without manually consulting third-party systems like SFDC, which is error prone.
When properly used this fully automates the requirements of our contribution program.

> **Note:** Splunk employees should read the [internal version of this document](https://go.splunk.com/!create#:~:text=http%3A//go/claagreementtrackerdocs) instead.

## Intended Users

Splunk open-source project maintainers

## Get Started

Splunk developers may opt into this solution by doing the following:

1. Add workflows/agreements.yaml to their github repo in .github/workflows using the main branch. You can use [this premade agreements.yaml file](https://github.com/splunk/addonfactory-github-workflows/blob/55321beab6af7e2ebc81311af6baff529c6109b6/.github/workflows/agreements.yaml) if necessary.
1. Enable [branch protection](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/defining-the-mergeability-of-pull-requests/managing-a-branch-protection-rule) for main, develop, and any other merge targets with the requirement of passing the agreements status check.
Add a [repository secret PAT_TOKEN with a Github Personal Access Token (PAT)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) for a service account to your repo.  This token should include the repo scope, and you must manually add it in the repo’s secret.

## Acknowledgements

This CLA/COC tracker users https://github.com/marketplace/actions/cla-assistant-lite. Thank you SAP for your support of the OSS/Shared source Community.
