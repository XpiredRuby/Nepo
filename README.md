# Job Alert Watchdog

Free watchdog infrastructure for the recurring engineering-job alerts.

The ChatGPT scheduled searches write a small heartbeat file after a successful search + Gmail delivery. GitHub Actions independently checks those heartbeats. If one becomes stale, the workflow opens and assigns a GitHub issue; when the heartbeat recovers, the issue is closed automatically.

No OpenAI API key, paid scheduler, or email credential is stored in this repository.
