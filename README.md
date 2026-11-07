# site (Labs)

The LinuxServer Labs website: every image in this organisation, its builds and the Labs fleet board, plus what Labs
is and how to get an application in. It is the main website's code ([linuxserver-playground/site](https://github.com/linuxserver-playground/site))
built in Labs mode (`PUBLIC_SITE_MODE=labs`) from the [Labs hub](https://github.com/linuxserverlabs-playground/hub),
and served on this repository's GitHub Pages.

- `.github/workflows/deploy.yml` builds it and publishes it from the `gh-pages` branch. Only the Labs control plane
  starts it, on its slots: when the Labs hub published new data or this repository's `main` moved, and once a day
  with `refresh_all`.
- The `data` branch holds this site's data snapshots in one commit, replaced on every deploy.

A change to the website belongs in the main site; this repository holds no code.
