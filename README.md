# Codegy status

Uptime monitor and public status page for Codegy's services, built on
[Upptime](https://upptime.js.org): GitHub Actions checks each site every
5 minutes, opens an issue in this repo when one is down and closes it on
recovery (HQ is to read those issues). The page is meant to live at
`status.codegy.in`.

What it watches (`.upptimerc.yml`):

- **HQ**: Codegy's admin panel login page.
- **Platform**: the institute portal's login page. The address is kept in
  the `PLATFORM_HEALTH_URL` repository secret, not in this file. It shows
  the portal is being served, not that its database answers.
- **Codegy website**: https://www.codegy.in

This repository is public. Client monitors are named by an opaque id and
their addresses live in repository secrets; see [OPERATIONS.md](OPERATIONS.md).

## Turning it on

Actions are switched off on purpose until the secrets are set. The steps
(a token, two secrets, "Setup CI", Pages and DNS) are in
[OPERATIONS.md](OPERATIONS.md#turning-it-on). Once it runs, Upptime writes
the live table between the markers below.

<!--start: status pages-->
<!--end: status pages-->
