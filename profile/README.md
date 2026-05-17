<p align="center">
  <img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/q-git-square.png" alt="GoodQ mark" width="140" />
</p>

# GoodQ

If you can't own your tools, you don't own your future.

GoodQ builds local-first systems for memory, automation, and creative intelligence. The work is practical, inspectable, and meant to stay in the hands of the person running it.

## Welcome Aboard GoodQ4All

GoodQ4All is the public local-first memory project: a Windows-first multimodal system that turns video, audio, and text into scene-level memory with visible proof paths.

Start with the two-minute onboarding film if you want to see the install and first ingestion loop before reading the deeper docs.

<p align="center">
  <a href="https://github.com/GoodQ02/.github/releases/download/welcome-aboard-goodq4all-2026-05-17/GOODQ4ALL_DEMO_FINAL.mp4">
    <img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/goodq4all-demo-poster.jpg" alt="Watch Welcome Aboard GoodQ4All" width="760" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/GoodQ02/.github/releases/download/welcome-aboard-goodq4all-2026-05-17/GOODQ4ALL_DEMO_FINAL.mp4">Watch the 2-minute guided demo</a>
  ·
  <a href="https://github.com/GoodQ02/goodq4all">Open the repo</a>
  ·
  <a href="https://github.com/GoodQ02/goodq4all/blob/main/docs/guides/DEMO.md">Read the demo guide</a>
</p>

## Visual First Run

Each frame below is pulled from the final onboarding film and paired with the action it narrates. Click any frame to enlarge it.

| Step | Type or do this | Demo frame |
| --- | --- | --- |
| 1 | Clone the official source:<br>`git clone https://github.com/GoodQ02/goodq4all.git` | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/01-clone-official-source.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/01-clone-official-source.jpg" alt="Clone the GoodQ4All repository" width="300" /></a> |
| 2 | Enter the project cabin:<br>`cd goodq4all` | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/02-enter-project-cabin.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/02-enter-project-cabin.jpg" alt="Enter the GoodQ4All project folder" width="300" /></a> |
| 3 | Run the bootstrap installer:<br>`python scripts/bootstrap_install.py`<br><sub>CPU-safe first-run variant: `python scripts/bootstrap_install.py --disable-gpu --disable-wsl-audio --skip-model-prefetch`.</sub> | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/03-bootstrap-installer.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/03-bootstrap-installer.jpg" alt="Run the bootstrap installer" width="300" /></a> |
| 4 | Optional local config:<br>copy `.env.local.template` to `.env.local` when using local model, cache, or provider settings. | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/04-env-local-root.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/04-env-local-root.jpg" alt="Place env local configuration in the repo root" width="300" /></a> |
| 5 | Validate the bootstrap:<br>`.\scripts\bootstrap_validate.bat` | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/05-bootstrap-validator.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/05-bootstrap-validator.jpg" alt="Run the bootstrap validator" width="300" /></a> |
| 6 | Run the launcher/readiness check:<br>`.\LAUNCH_GOODQ.ps1` | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/06-launch-goodq.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/06-launch-goodq.jpg" alt="Launch GoodQ4All readiness checks" width="300" /></a> |
| 7 | Start Watchdog, then drop one small media file into `import_inbox`:<br>`conda run --no-capture-output -n goodq_core python -m cli.watchdog` | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/07-watchdog-observes.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/07-watchdog-observes.jpg" alt="Watchdog observes the imported media file" width="300" /></a> |
| 8 | Start the API and inspect proof:<br>`conda run --no-capture-output -n goodq_core python -m api.server` | <a href="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/08-proof-recorded.jpg"><img src="https://raw.githubusercontent.com/GoodQ02/.github/main/image/terminal-steps/08-proof-recorded.jpg" alt="Ingestion completes and proof is recorded" width="300" /></a> |

## What GoodQ4All Proves

- **Local-first memory**: the supported runtime works without a required cloud dependency.
- **Scene-centric ingestion**: scenes are the atomic unit for video, audio, and text intelligence.
- **Visible proof paths**: runtime artifacts, manifests, logs, and API routes are part of the product surface.
- **Operator-friendly flow**: bootstrap, validate, launch readiness, start Watchdog, drop media, inspect proof.

## Start Here

Supported first-run host: Windows 11 with Git, Conda, Python 3.10+, and local
disk space for the selected install path.

```powershell
git clone https://github.com/GoodQ02/goodq4all.git
cd goodq4all
python scripts/bootstrap_install.py
.\scripts\bootstrap_validate.bat
.\LAUNCH_GOODQ.ps1
```

Then leave Watchdog running in one terminal:

```powershell
conda run --no-capture-output -n goodq_core python -m cli.watchdog
```

Drop one small media file into the configured `import_inbox`, then start the API in another terminal:

```powershell
conda run --no-capture-output -n goodq_core python -m api.server
```

Open:

- `http://127.0.0.1:30000/api/health/summary`
- `http://127.0.0.1:30000/docs`

## Ethos

- Your data, your rules.
- Automate to liberate, not to surveil.
- Local truth beats cloud-shaped assumptions.
- Rigorous enough for production, friendly enough to invite curiosity.

## Links

- [GoodQ4All repo](https://github.com/GoodQ02/goodq4all)
- [Guided demo release](https://github.com/GoodQ02/.github/releases/tag/welcome-aboard-goodq4all-2026-05-17)
- [askgoodq.com](https://askgoodq.com)
- Instagram: [@goodq02](https://instagram.com/goodq02)
