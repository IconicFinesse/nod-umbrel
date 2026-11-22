# nod-umbrel

Build pipeline for the **iconicfinesse-nod** Umbrel app. A GitHub Actions workflow checks out n8n-io/nod at the commit pinned in `UPSTREAM_SHA`, builds its three self-host images (server, browser, workspace), and pushes them to GHCR as ghcr.io/iconicfinesse/nod-server, ghcr.io/iconicfinesse/nod-browser, and ghcr.io/iconicfinesse/nod-workspace. The Umbrel app itself lives in the iconicfinesse-umbrel-app-store repo and only pulls these images.
