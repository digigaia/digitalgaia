# Infrastructure

Research for which internal tools to use should be made as [RFC/decision style document](#sop-ref)

- password manager (bitwarden)
- communication (matrix, element, zulip)
- file sharing (tresorit, syncthing?)
- bug tracking (linear)
- source code hosting (github)
- CI (?)
- sysadmin/devops (pyinfra) (see also network topologies (tailscale etc.) in hacking.org > netsec)

```{tip}
investigate [Radicle](https://radicle.xyz/blog/towards-decentralized-code-collaboration.html) for source code hosting and bug-tracking
- <https://radicle.xyz/2024/09/10/radicle-1.0.html>
- <https://radicle.xyz/guides/user>
```

## Security

Security needs to be enforced all the time, we want to have proper access to resources. Nothing "shared all" or public by default. Take care of access with (potentially old) SSH keys on servers.


## Infrastructure maintenance

Upgrade of critical infrastructure should be done in a meeting with everyone watching.

This shares information about what is done, how it is done, and ensures no one is working during that time.

We should also redeploy most of our servers regularly to make sure the install/backup scripts include everything -> even better, we should ensure that we are always able to redeploy the entire infrastructure by just having access to the `servers` repo.


## Infrastructure as code

see: [Infrastructure as code](https://en.wikipedia.org/wiki/Infrastructure_as_code)

in general, we want to store and work only on install scripts (a la ansible or pyinfra) instead of artifacts (docker, etc.). Even though it seems like containers/artifacts give us reproducibility, it introduces a lot of complexity in managing how artifacts are stored, how much they weigh, etc. Having only install scripts keeps only the high-level logic of the infrastructure and is much more nimble.

see also: [Why not Docker for SourceHut?](https://paste.sr.ht/~sircmpwn/78cc21e1661d5a9d8038f47e532d286807ac89ad)

another important aspect is that we need to ensure the idempotence of each operation in the scripts, this allows
to rapidly fix a broken deployment step-by-step by fixing on the go the operations that are failing and relaunching
the entire deploy repeatedly
