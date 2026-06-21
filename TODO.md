# TODO

## Step 1 — Fix rejected push
- Fetch remote `main`
- Pull with rebase: `git pull --rebase origin main`
- Push again

## Step 2 — Fix GitHub Actions workflow syntax
- Update `.githubworkflow/build.yml`: change `cache: truecd` -> `cache: true` (remove stray `cd`).

## Step 3 — Validate
- Run `go test ./...`
- (Optional) run `go build ./...`
- Ensure workflow parses (push after Step 1/2)

