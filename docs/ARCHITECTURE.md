# OpenWork Architecture Principles (Draft)

This document describes proposed requirements, **not an implemented architecture**. No final tech stack has been selected.

## OpenWork will focus on

- Proposing and moderating community project ideas.
- Discovering projects and contributor roles.
- Joining teams through safe, transparent workflows.
- Tracking high-level project lifecycle and linking to existing repositories and launched software.

## OpenWork should not rebuild

Git hosting, pull requests, general-purpose CI/CD, issue trackers, or full team chat platforms where suitable open-source tools already exist.

## Non-negotiable design criteria

1. **Self-hostable:** Runnable without mandatory accounts with proprietary vendors.
2. **Open source:** Compatible with Apache-2.0 and transparent development.
3. **Low cost:** No paid APIs required for core platform features; deployable on modest infrastructure.
4. **Portable:** Open formats and well-documented configuration where practical.
5. **Secure and private:** Minimal data collection, sensible access controls, safe authentication, secrets handling, and backups.
6. **Accessible:** Responsive layouts, keyboard support, screen-reader usability, and inclusive design.
7. **Maintainable:** Tests, migrations, documentation, and manageable operational complexity.

## Integrations

GitHub can be an **optional** integration for repository links and public contribution metadata. Core proposal and browsing functionality should not require GitHub sign-in for a self-hosted instance.

## Deployment

Reproducible local development and a documented self-hosted setup (possibly Docker Compose) are release requirements. Infrastructure outside the application can still incur costs.

## Open design questions

- Framework and language
- Database and migrations
- Login methods and optional GitHub OAuth
- Moderation and reporting channels
- Spam prevention and notifications
- Deployment, backups, upgrades, and testing

We will evaluate these publicly with founding contributors before committing to a stack.
