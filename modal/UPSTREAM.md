# Upstream and production baseline

This repository is a fork of `HorizonRobotics/EmbodiedGen`.

The repository root currently follows upstream `v2.1.0` (`f0124197888c2b733e4eaa65acd81ad9cfda3b79`).
The code under `modal/` was migrated from the previously validated `modal-build` production
integration and intentionally remains pinned to EmbodiedGen `v2.0.0`
(`cc3015ca5ccdacf94df3428d9e65f79375982216`) until a separate v2.1.0 compatibility validation is
completed.

The migration in this commit changes ownership and repository-relative paths only. It does not
silently upgrade the deployed Modal production runtime from v2.0.0 to v2.1.0.

Long term, Modal-specific deployment/build/orchestration code belongs under `modal/`. Changes that
are genuinely required in upstream EmbodiedGen source should be maintained as normal fork changes
with minimal divergence from upstream.
