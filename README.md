## Getting Started

This project is a template to be used to pull a given example from a folder/directory of another repository.

### Requirements

- Add descriptions to the example (mandatory)
- Check if the github action to perform the pull from another repository exists.
- Turn off issue/wikis/projects/discussions
- Disable Releases/Environments/Packages
- Change the github action workflow, `sync` accordingly to your needs

### Installation

```yaml
- name: Pull from another repository
  uses: ipfs-examples/actions-pull-directory-from-repo@main
  with:
    source-repo: # mandatory, ex: 'ipfs-examples/js-ipfs-examples'
    source-folder-path: # mandatory, ex: 'examples/your-example'
    source-branch: # optional, can be omitted, defaults to: 'main'
    target-branch: # optional, can be omitted, defaults to: 'main'
    git-username: # optional, can be omitted, defaults to: 'github-actions'
    git-email: # optional, can be omitted, defaults to: 'github-actions@github.com'
```

_For more information, please refer to the [Documentation](https://github.com/ipfs-examples/actions-pull-directory-from-repo)_

## Usage/Examples

This repository will sync automatically based on the timer of the workflow, you can trigger manually:

- Go to the repository on Github
- Go to the `Actions` section
- Select the `Sync` workflow
- Run the workflow

_For more information, please refer to the [Documentation](https://docs.github.com/en/actions/managing-workflow-runs/manually-running-a-workflow)_
