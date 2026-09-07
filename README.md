# Production Workflow Automation (n8n)

## 📋 Overview

A custom automation system built on n8n for an e-commerce client to eliminate the manual coordination bottleneck in their advertisement production process. The previous workflow had the business owner acting as a "mailman" — manually transferring files and updates between the Research → Voice Over → Video (Montage) stages, making task tracking nearly impossible.

The system connects the whole team on autopilot and removes the owner from the middle of the process.

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Automation | n8n (self-hosted workflows) |
| Messaging | WhatsApp (notifications + interactive Approve/Reject buttons) |
| Storage | Google Drive (automated folder & file organization) |
| Tracking | Custom dashboard for stage-by-stage timing |

## ✨ How It Works

- **Instant Notifications** — As soon as the Research stage is done, the owner receives a WhatsApp notification with all product details and Approve / Reject buttons.
- **Automated Handoff** — On "Accept," the workflow automatically creates Google Drive folders, organizes the product data, and dispatches the task to the Voice Over artist — no manual handover.
- **Seamless Delivery** — When the recording is ready, the system grabs it and sends it directly to the Editor. No more playing "mailman."

## 📊 Results

- Massive time savings for the owner by removing manual coordination from the daily cycle
- Clear visibility — a dashboard that tracks exactly how long each stage takes, enabling real process analytics
- End-to-end visibility across the three production stages with structured, organized data (Google Drive + automated notifications)

## 📐 Impact

This project transformed the client from being a "bottleneck" into an observer — the automation handles the routing, organization, and communication, while the owner gets real time metrics to make better decisions.

---

## Repo Notes

This repo contains an exported n8n workflow (`My workflow.json`) plus a few helper scripts used for cleaning/verifying phone numbers.

- n8n workflow exports typically reference credentials by **name/id** (not secret values). Still, review the JSON before sharing publicly.
- CSV exports are intentionally ignored via `.gitignore`.