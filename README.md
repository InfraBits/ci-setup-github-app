# Setup GitHub app access key

Generate a valid access key for a given repo based on a GitHub app

## Example Usage

```
  setup:
    uses: infrabits/ci-setup-github-app/.github/workflows/setup.yml@main
    with:
      app_id: 1234
      app_key: "${{ secrets.SOME_BASE64_ENCODED_KEY }}"
      repo: some-org/some-repo
```

or

```
    steps:
      - uses: infrabits/ci-setup-github-app@main
        with:
          app_id: 1234
          app_key: "${{ secrets.SOME_BASE64_ENCODED_KEY }}"
          repo: some-org/some-repo
```
