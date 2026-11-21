Lab 3b-1

Reflection Questions:
Why absolute paths matter in cron: 
cron runs with a minimal default PATH (often only /usr/bin:/bin) and a different working directory than an interactive terminal, so relative paths or unpathed commands can fail or write files to unexpected places.

Benefits of cloud exporting for backups: 
Off-site cloud copies protect against local hardware failure, accidental deletion, or localized outages, and allow recovery even if the source machine is lost.

How cron differs from manual execution: 
Manual runs execute in your live user session with your environment variables, interactive prompts, and immediate terminal output; cron runs non-interactively in the background on a schedule with a stripped-down environment and no attached terminal.

If SSH keys/fingerprints are not accepted ahead of time: 
An unverified host key causes SSH/scp to prompt interactively for yes/no (which hangs or fails in non-interactive cron jobs), while a missing or unauthenticated SSH key fails with Permission denied (publickey).

How login messages help engagement and operations: 
Clear banners and system summaries (figlet, neofetch, or custom MOTD notices) immediately orient administrators to which host they logged into, highlight maintenance notes or environment status, and make routine logins more informative.
