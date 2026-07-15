# SSH Access & Logging

In some cases, a developer or user may wish to obtain SSH access to run additional tasks, change configuration settings, or see full logs from the Escape Pod for diagnostic purposes.

---

## SSH Access

If you need to access the Pi via SSH, please use the credentials below.

**Note**: You will be prompted to change these defaults on first login. The connection will automatically exit when you have completed the password change. SSH back into the Pi with your new credentials.

Default Credentials:

Username: ubuntu

 Password: ubuntu

---

## Tailing Escape Pod Logs:

To tail Escape Pod service logs to diagnose and report issues, use the following shell command when logged in via SSH:

`journalctl -u escape_pod.service -f`

To see only the logs that pertain to words that are understood by the Escape Pod (useful for maintaining your own speech interpretation logs), use the following command:

`journalctl -u escape_pod.service -f | grep incoming_text`
