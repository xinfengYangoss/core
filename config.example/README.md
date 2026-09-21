# Core configuration template

`config.example/` contains a minimal, non-sensitive example configuration for development handoff.

Create a new runtime directory named `config/` in the Core repository, then copy `configuration.yaml` into it. Do not copy another developer's `config/` directory: it can contain users, access tokens, device registrations, databases, and other local state.

The actual `config/` directory is intentionally ignored by Git. Keep secrets, certificates, and any environment-specific values only there or in a separately managed secret store.

`frontend.development_repo` is a path inside the development container, not a Windows path. The default assumes the Frontend repository is mounted at `/workspaces/frontend`.
