# vibe-backend

**Define serverless APIs in natural-language markdown.**

You describe models, methods and API entry points in markdown. At deploy time
they are compiled into a human-reviewed, structured lock file. A Rust-core SDK
then runs them on demand, cold-starting like a serverless function, with
built-in best practices.

🌐 **Website:** [vibe-backend.github.io](https://vibe-backend.github.io/)
(English / 繁體中文)

## Repositories

| Repo | What it is |
| --- | --- |
| [sdk](https://github.com/vibe-backend/sdk) | Rust SDK, spec and docs. Ships the `vibe-sdk` (`vibe` CLI for build and dev) and `vibe-runtime` (deploy-only) binaries; latest pre-release [v1.0.0-rc.4](https://github.com/vibe-backend/sdk/releases/tag/v1.0.0-rc.4) |
| [sample-hello-world](https://github.com/vibe-backend/sample-hello-world) | Hello world and counter demo API with `backend/` (vibe project) and `frontend/` (React) folders; dev/demo image, not for production |
| [sample-shop](https://github.com/vibe-backend/sample-shop) | Sample shopping site: static `frontend/`, with a `backend/` built on the SDK planned ([live](https://vibe-backend.github.io/sample-shop/)) |
| [sample-envelope](https://github.com/vibe-backend/sample-envelope) | 信封產生器: frontend-only envelope layout and printing tool (React), `backend/` reserved for v2 ([live](https://vibe-backend.github.io/sample-envelope/)) |
| [vibe-backend.github.io](https://github.com/vibe-backend/vibe-backend.github.io) | Source for the organization website; docs are fetched from `sdk` at build time |
| [.github](https://github.com/vibe-backend/.github) | This organization profile |

## Get started

Read the [quick start](https://vibe-backend.github.io/) on the website, then browse
the [sample shop](https://github.com/vibe-backend/sample-shop) for a working
example.
