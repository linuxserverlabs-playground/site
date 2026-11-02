# site (Labs)

The LinuxServer Labs website: every image in this organisation, its builds and the Labs fleet board, plus what Labs
is and how to get an application in. It is the main website's code ([linuxserver-playground/site](https://github.com/linuxserver-playground/site))
built in Labs mode (`PUBLIC_SITE_MODE=labs`) from the [Labs hub](https://github.com/linuxserverlabs-playground/hub),
and served on this repository's GitHub Pages.

- `.github/workflows/deploy.yml` builds and deploys it on every push here, daily, when the Labs hub has new data
  (`repository_dispatch hub-updated`, sent by the Labs control plane) and on demand.
- The `data` branch holds this site's data snapshots in one commit, replaced on every deploy.

A change to the website belongs in the main site; this repository holds no code.
