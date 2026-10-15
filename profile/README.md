# vibe-backend

**Design serverless APIs in Markdown. Review the generated contract. Run them with a Rust-based runtime.**

vibe-backend is an early-stage toolkit for defining backend models, methods, migrations, and API entry points in structured Markdown. The `vibe` CLI compiles those definitions into reviewable lock files and a signed manifest; the runtime executes the manifest rather than interpreting natural language at request time.

> [!IMPORTANT]
> vibe-backend is under active development. Interfaces and workflows may change, and some documented capabilities remain design work. Review the [SDK status](https://github.com/vibe-backend/sdk#status) before using it in a project.

## How it works

1. **Define** your backend in Markdown.
2. **Compile** it into deterministic, structured lock files.
3. **Review and approve** the generated contract.
4. **Validate and build** a signed manifest.
5. **Serve** the manifest with the Rust runtime.

This separation keeps natural-language input out of the request path and gives teams an explicit artifact to review before deployment.

## Explore the project

| Repository | Purpose |
| --- | --- |
| [**sdk**](https://github.com/vibe-backend/sdk) | Rust runtime, `vibe` CLI, specifications, and technical documentation |
| [**sample-shop**](https://github.com/vibe-backend/sample-shop) | Example storefront and evolving reference integration |
| [**vibe-backend.github.io**](https://github.com/vibe-backend/vibe-backend.github.io) | Source for the project website |

## Get started

- Visit the [project website](https://vibe-backend.github.io/) in **English** or **繁體中文**.
- Read the [SDK overview and setup guide](https://github.com/vibe-backend/sdk#readme).
- Review the current [v1.7 specification](https://github.com/vibe-backend/sdk/blob/main/docs/spec-v1.7.md).
- Follow the [v1.8 draft](https://github.com/vibe-backend/sdk/blob/main/docs/spec-v1.8.md) to see work under review.

The SDK repository currently contains the runnable test fixture referenced by its setup guide. The sample shop is still evolving and should not yet be treated as a complete production example.

## Project principles

- **Review before execution** — generated contracts are explicit and human-reviewable.
- **Deterministic artifacts** — deployments are based on lock files and a signed manifest.
- **Runtime separation** — production requests execute approved structures, not natural-language prompts.
- **Secure defaults** — validation, authentication, authorization, rate controls, and tenant boundaries are treated as core platform concerns.

## Contributing and feedback

The project is evolving, and practical feedback is welcome. For bugs, documentation gaps, or feature proposals, open an issue in the most relevant repository:

- [SDK issues](https://github.com/vibe-backend/sdk/issues)
- [Sample shop issues](https://github.com/vibe-backend/sample-shop/issues)

When reporting a problem, include the affected version or commit, operating system, reproduction steps, and the expected and actual behavior.
