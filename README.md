# vCard - Personal portfolio

vCard is a fully responsive personal portfolio website, responsive for all devices, built using HTML, CSS, and JavaScript.

## Demo

![vCard Desktop Demo](./website-demo-image/desktop.png "Desktop Demo")
![vCard Mobile Demo](./website-demo-image/mobile.png "Mobile Demo")

## Prerequisites

Before you begin, ensure you have met the following requirements:

* [Git](https://git-scm.com/downloads "Download Git") must be installed on your operating system.

## Installing vCard

To install **vCard**, follow these steps:

Linux and macOS:

```bash
sudo git clone https://github.com/doomslayer86/vcard-personal-portfolio.git
```

Windows:

```bash
git clone https://github.com/doomslayer86/vcard-personal-portfolio.git
```

## Deploy to Spaceship

Pushes to `master` trigger an automatic deploy. Two workflows:

- **`deploy-to-spaceship.yml`** — FTP (port 21). Use if your host supports FTP.
- **`deploy-to-spaceship-sftp.yml`** — SFTP (port 22). Use if you get **"Timeout (control socket)"** or your host only allows SFTP (common with cPanel/Spaceship). Same secrets; SFTP runs on push and can also be triggered manually (Actions → Deploy to Spaceship (SFTP) → Run workflow).

Only site files are uploaded; `.git`, `.github`, `node_modules`, and other dev/repo files are excluded.

### Where to set credentials

**GitHub → this repo → Settings → Secrets and variables → Actions**, or **Environments → prod** if you use the prod environment.

Add these secrets (repo or in **prod** environment):

| Secret             | Description |
|--------------------|-------------|
| `FTP_SERVER`       | FTP hostname (e.g. `ftp.example.com`) |
| `FTP_USERNAME`     | FTP username |
| `FTP_PASSWORD`     | FTP password |
| `FTP_REMOTE_PATH`  | Use `/` for site root, or e.g. `public_html` |

Then push to `main` or `master`; the **Actions** tab will show the deploy run.

---

## License

MIT
