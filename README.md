# Fetch Latest Release Version

A Github Action to fetch the latest release version for the current repository.

## Usage

```
jobs:
  job-name:
    runs-on: ubuntu-latest
    steps:

      - uses: actions/checkout@v2

      - name: Fetch latest release version
        id: fetch-latest-release
        uses: Lukacs5/action-latest-release-version@v2.0.0

      - name: Test
        run: echo ${{ steps.fetch-latest-release.outputs.latest-release }}
``` 
