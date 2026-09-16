# clusdr

A runtime for the cluster. An SDK for the app.

Distributed coordination without turning the application into a cluster member. The app talks to a **local daemon**; the daemons form the cluster.

Not a database, queue, or Kubernetes. API is **v1alpha1**. TLS is on by default.

```text
Application → local SDK → clusdr daemon → cluster
```

[clusdr.io](https://clusdr.io) · [Install](https://clusdr.io/docs/guide/install) · [Docs](https://clusdr.io/docs/)

## Repositories

| Repo | What it is |
|---|---|
| [clusdr](https://github.com/clusdr/clusdr) | Daemon, protocol, docs, Go SDK |
| [clusdr-python](https://github.com/clusdr/clusdr-python) | Python SDK — `pip install clusdr` |

## Install

```bash
curl -fsSL https://clusdr.io/install.sh | sh
```

Linux amd64/arm64. Image: `durguto/clusdr` on Docker Hub (`ghcr.io/clusdr/clusdr` is the same image).

```bash
go get github.com/durguto/clusdr/sdk
pip install clusdr
```

Go module path stays `github.com/durguto/clusdr`. Apache-2.0.
