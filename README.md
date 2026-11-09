# template-test

[![security](https://github.com/niazhussain/template-test/actions/workflows/ci-security.yml/badge.svg?branch=main)](https://github.com/niazhussain/template-test/actions/workflows/ci-security.yml)

One or two sentences on what **template-test** does and who uses it.

## Getting started

How to install, configure and run template-test locally.

## Security checks

Every pull request and every push to `main` of `niazhussain/template-test` runs the shared security gate, through [`.github/workflows/ci-security.yml`](.github/workflows/ci-security.yml). It looks for leaked secrets, vulnerable or malicious dependencies, insecure code, risky workflow and Dockerfile settings, and, when there is a Dockerfile, problems in the built image and the running app. It then decides **PASS** or **FAIL**.

- **See a result:** open a run in [Actions → security](https://github.com/niazhussain/template-test/actions/workflows/ci-security.yml), then the **Security gate** job, and click **Open the full HTML report**.
- **Settings for this repository** (app port, health path, Dockerfile path) are in the `with:` block of `ci-security.yml`.
- **How the gate works, and what to do when it fails:** [niazhussain/template](https://github.com/niazhussain/template#readme).
- **Accepting a false positive** (`nosemgrep`, `.trivyignore`, …) needs a review from the code owners in [`.github/CODEOWNERS`](.github/CODEOWNERS).
