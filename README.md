# Run IntelliJ IDEA Inspections for Android Projects

This GitHub Action runs a set of IntelliJ IDEA Inspections against a PR, and comments on all violations. The image also has the Android tools installed, so this action can be used on Android projects.

## Inputs

### `gh_token`

The GitHub token used to authenticate with GitHub.

**Required**

### `inspections_file`

Path to inspections file relative to root of project directory.

**Required**

## Example Usage

```yml
- name: Run IntelliJ Inspections
  uses: gps/intellij-android-inspections@master
  with:
    GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    INSPECTIONS_FILE: Inspections.xml

```
