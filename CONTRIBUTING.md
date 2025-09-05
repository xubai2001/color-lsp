# Contributing

Contributing are welcome!

## color-lsp

The `color-lsp` is a Language Server Protocol (LSP) server that provides color.

### Release new version

1. Run `cargo set-version -p color-lsp` to update version in `color-lsp/Cargo.toml`.
2. Git commit with `git commit -m "Version ${VERSION}"`
3. Create new tag and push it to GitHub

Then the GitHub Action will automatically publish the release.

## zed-color-highlight

The `zed-color-highlight` is a Zed editor extension that highlights color codes.

You must install [zed-extension](https://github.com/zed-industries/zed/tree/main/crates/extension_cli) cli first.

### Release new version

1. Run `cargo set-version -p zed-color-highlight` to update version in `zed-color-highlight/Cargo.toml`.
2. Modify `zed-color-highlight/extension.toml` to update the version.
3. Git commit with `git commit -m "Version ${VERSION}"`
4. Visit [GitHub Action](https://github.com/huacnlee/color-lsp/actions/workflows/release-extension.yml)
   page to trigger **Run Workflow**, and select a tag to trigger the workflow.

Then the GitHub Action will automatically publish the extension update PR
to [zed-extensions](https://github.com/zed-industries/extensions/pulls).
