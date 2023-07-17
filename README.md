# Preevy Orb [![CircleCI Build Status](https://circleci.com/gh/livecycle/preevy-orb.svg?style=shield "CircleCI Build Status")](https://circleci.com/gh/livecycle/preevy-orb) [![CircleCI Orb Version](https://badges.circleci.com/orbs/livecycle/preevy.svg)](https://circleci.com/developer/orbs/orb/livecycle/preevy) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/livecycle/preevy/master/LICENSE) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)


Run Preevy from CircleCI 🤘

[What are orbs?](https://circleci.com/orbs/)


## About Preevy

Preevy is a powerful CLI tool designed to simplify the process of creating ephemeral preview environments.
Using Preevy, you can easily provision any Docker-Compose application on affordable [AWS](https://preevy.dev/drivers/aws-lightsail), [GCP](https://preevy.dev/drivers/gcp-gce), [Azure](https://azure.microsoft.com/en-us) or [k8s](https://preevy.dev/drivers/kube-pod) VMs.

Visit The full documentation here: https://preevy.dev/



## Resources

[CircleCI Orb Registry Page](https://circleci.com/developer/orbs/orb/livecycle/preevy) - The official registry page of this orb for all versions, executors, commands, and jobs described.

[CircleCI Orb Docs](https://circleci.com/docs/orb-intro/#section=configuration) - Docs for using, creating, and publishing CircleCI Orbs.

### How to Contribute

We welcome [issues](https://github.com/livecycle/preevy-orb/issues) to and [pull requests](https://github.com/livecycle/preevy-orb/pulls) against this repository!

### How to Publish An Update
1. Merge pull requests with desired changes to the main branch.
    - For the best experience, squash-and-merge and use [Conventional Commit Messages](https://conventionalcommits.org/).
2. Find the current version of the orb.
    - You can run `circleci orb info livecycle/preevy | grep "Latest"` to see the current version.
3. Create a [new Release](https://github.com/livecycle/preevy-orb/releases/new) on GitHub.
    - Click "Choose a tag" and _create_ a new [semantically versioned](http://semver.org/) tag. (ex: v1.0.0)
      - We will have an opportunity to change this before we publish if needed after the next step.
4.  Click _"+ Auto-generate release notes"_.
    - This will create a summary of all of the merged pull requests since the previous release.
    - If you have used _[Conventional Commit Messages](https://conventionalcommits.org/)_ it will be easy to determine what types of changes were made, allowing you to ensure the correct version tag is being published.
5. Now ensure the version tag selected is semantically accurate based on the changes included.
6. Click _"Publish Release"_.
    - This will push a new tag and trigger your publishing pipeline on CircleCI.    