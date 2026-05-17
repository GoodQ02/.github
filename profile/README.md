<p align="center">
  <img src="../image/q-git-square.png" alt="GoodQ mark" width="140" />
</p>

# GoodQ

If you can't own your tools, you don't own your future.

GoodQ builds local-first systems for memory, automation, and creative intelligence. The work is practical, inspectable, and meant to stay in the hands of the person running it.

## Welcome Aboard GoodQ4All

GoodQ4All is the public local-first memory project: a Windows-first multimodal system that turns video, audio, and text into scene-level memory with visible proof paths.

Start with the two-minute onboarding film if you want to see the install and first ingestion loop before reading the deeper docs.

<p align="center">
  <a href="https://github.com/GoodQ02/.github/releases/download/welcome-aboard-goodq4all-2026-05-17/GOODQ4ALL_DEMO_FINAL.mp4">
    <img src="../image/goodq4all-demo-poster.jpg" alt="Watch Welcome Aboard GoodQ4All" width="760" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/GoodQ02/.github/releases/download/welcome-aboard-goodq4all-2026-05-17/GOODQ4ALL_DEMO_FINAL.mp4">Watch the 2-minute guided demo</a>
  ·
  <a href="https://github.com/GoodQ02/goodq4all">Open the repo</a>
  ·
  <a href="https://github.com/GoodQ02/goodq4all/blob/main/docs/guides/DEMO.md">Read the demo guide</a>
</p>

## What GoodQ4All Proves

- **Local-first memory**: the supported runtime works without a required cloud dependency.
- **Scene-centric ingestion**: scenes are the atomic unit for video, audio, and text intelligence.
- **Visible proof paths**: runtime artifacts, manifests, logs, and API routes are part of the product surface.
- **Operator-friendly flow**: bootstrap, validate, launch readiness, start Watchdog, drop media, inspect proof.

## Start Here

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
