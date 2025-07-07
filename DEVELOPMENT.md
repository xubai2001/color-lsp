# Development

## Release new version for color-lsp

1. Run `cargo set-version` to update version in `color-lsp/Cargo.toml`.
2. Git commit with `git commit -m "Version ${VERSION}"`
3. Create new tag and push it to GitHub

Then the GitHub Action will automatically publish the release.

## Release new version for zed-color-highlight

1. Run `cargo set-version` to update version in `zed-color-highlight/Cargo.toml`.
2. Git commit with `git commit -m "Version ${VERSION}"`
3. Visit [GitHub Action](https://github.com/huacnlee/color-lsp/actions/workflows/release-extension.yml)
   page to trigger **Run Workflow**, and select a tag to trigger the workflow.

Then the GitHub Action will automatically publish the extension update PR
to [zed-extensions](https://github.com/zed-industries/extensions/pulls).
