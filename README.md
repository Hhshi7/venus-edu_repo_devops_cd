# 📋 Twitch Live Bot – DevOps Platform

Production-like DevOps setup for a self-hosted Twitch monitoring bot running on ARM-based Linux (Raspberry Pi).
This repository serves as **operational and architectural documentation** for a real-world DevOps use case, focused on reliability, automation, and observability.


> [!NOTE]
> This repository does not contain the application source code.
> The bot itself is maintained in a separate repository and is intentionally decoupled from platform concerns.

---

## 💻 Environment

The application is designed to run continuously (24/7) with minimal downtime and fast recovery from failures.

It is hosted on a small-scale self-managed Linux server:

- **Hardware:** Raspberry Pi (ARM)
- **Operating System:** Raspberry Pi OS Lite (Debian-based)
- **Deployment model:** Manual self-hosting

## :x: Problem

The system relies entirely on home infrastructure, which introduces several reliability risks:
- Unstable home network
- Power outages
- Physical hardware limitations

### Current limitations
- Application stops silently when failures occur
- No automatic recovery after crashes or power loss
- Manual deployments required for every change
- SSH access needed to update code from different workstations

As a result, the service requires constant manual monitoring and maintenance.

---


