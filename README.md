# googletest-action
GitHub Action for googletest

Runs GoogleTest C++ tests

# Usage

To use this action, create a `.github/workflows/googletest-checker.yml` in the target repository containing:

```
name: googletest-project
on:
  push:
    paths-ignore:
    - 'resources/**'
    - 'README.md'

jobs:
  test-project:
    name: Test Project
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2
    - name: Test project with googletest.
      uses: John-Hatton/googletest-action@main
```
