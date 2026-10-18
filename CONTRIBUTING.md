# Contributing to Redfox OSS

Thanks for helping! These guidelines apply to every repository in the organisation unless a repository has its own `CONTRIBUTING.md`.

## Before you start

- **Bugs:** search the existing issues first, then open one using the *Bug report* form.
- **Features and larger changes:** open an issue to discuss the idea **before** writing code, so nobody's time is wasted.
- **Security problems:** do **not** open a public issue. Follow [SECURITY.md](SECURITY.md).

## Making a change

1. Fork the repository and create a branch from `main` (for example `fix/mms-retry`).
2. Keep each pull request focused on one change. Small PRs get reviewed faster.
3. Follow the existing code style. Kotlin code follows the [Kotlin coding conventions](https://kotlinlang.org/docs/coding-conventions.html); UI uses the Obsidian components and tokens rather than hard-coded colours or sizes.
4. Build and test locally before pushing:
   ```bash
   ./gradlew build
   ```
5. Write commit messages in the imperative mood, with a short summary line (for example `MMS: retry temporary download failures`).
6. Open a pull request against `main` and fill in the template. CI must pass and review conversations must be resolved before merging.

`main` is protected: changes land only through pull requests, which are squash-merged.

## Licensing of contributions

Each repository has its own license (see its `LICENSE` file). By submitting a contribution you agree that it is licensed under that repository's license, and that you have the right to submit it.

## Never commit secrets

Do not commit signing keys, keystores, `keystore.properties`, `local.properties`, API keys or tokens. Secret scanning with push protection is enabled and will block such pushes.

## Code of Conduct

Everyone taking part must follow our [Code of Conduct](CODE_OF_CONDUCT.md).
