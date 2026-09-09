# Security Policy

## Supported versions

This project is deployed as a single Cloudflare Worker without version branches. Only the code on `main` is supported.

## Reporting a vulnerability

Please **do not** open a public GitHub issue for security vulnerabilities.

Instead, use GitHub's [private vulnerability reporting](../../security/advisories/new) for this repository, if enabled, or open a draft security advisory. If that isn't available, contact the repository maintainer directly through GitHub.

Please include:
- A description of the vulnerability and its potential impact
- Steps to reproduce (proof of concept if possible)
- Any suggested fix, if you have one

We'll acknowledge reports as quickly as we can and work with you on a fix and disclosure timeline.

## Notes on this project's threat model

This Worker reads Halo PSA agent and client data and proxies images through Cloudflare. It is **not** intended to be exposed publicly without additional access control — see the [Security — Cloudflare Zero Trust](README.md#security--cloudflare-zero-trust) section of the README. Reports about the app being reachable without Zero Trust configured by a deployer are a deployment/configuration concern, not a vulnerability in the code itself, but we're still interested in hearing about ways the app could better guide safe deployment.
