# Agent1

Instructions and CSS specifications for the L4 Process Map Copilot Agent.

## L4 Process Map CSS — Public Gist

The file [`l4-css.txt`](./l4-css.txt) contains the full CSS specification used by the L4 Process Map Generator Copilot Agent.

### Automated Gist Publishing

A GitHub Actions workflow ([`.github/workflows/create-gist.yml`](./.github/workflows/create-gist.yml)) automatically creates or updates a **public GitHub Gist** with the contents of `l4-css.txt` whenever that file is pushed to `main`.

The raw Gist URL is printed in the workflow run log in the format:

```
https://gist.githubusercontent.com/<username>/<gist-id>/raw/l4-css.txt
```

Paste that URL into **M365 Copilot Agent Builder → Knowledge → Add website URL**.

### One-time Setup

Before the workflow can create Gists, add a Personal Access Token (PAT) as a repository secret:

1. Create a PAT at <https://github.com/settings/tokens> with the **`gist`** scope.
2. In this repository go to **Settings → Secrets and variables → Actions → New repository secret**.
3. Name the secret **`GIST_TOKEN`** and paste your PAT as the value.
4. Push any change to `l4-css.txt` on `main` (or run the workflow manually via **Actions → Publish L4 CSS as Public Gist → Run workflow**).
5. Open the workflow run log and copy the **Raw URL** printed at the end.
