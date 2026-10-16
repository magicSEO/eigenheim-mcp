# ChatGPT App (Plugin) – submission guide

OpenAI retires custom GPTs on **11 December 2026** and replaces them with **apps in ChatGPT** (shown as “Plugins” in some accounts). Apps are built on MCP, so this server needs **no extra API** – ChatGPT connects directly to `https://eigenheim-invest.de/mcp/`.

## TL;DR
1. Verify your OpenAI platform account.
2. Test the server in ChatGPT (Developer mode / custom app).
3. Submit on the OpenAI platform → **Apps → Submit** with the data in [`app-submission.json`](./app-submission.json).
4. Wait for the review e-mail (Case ID). After approval click **Publish** – the app appears in the ChatGPT app directory.

## 1. Test before submitting
- ChatGPT → Settings → **Apps** (or **Plugins**) → Advanced → enable **Developer mode**.
- **Create app**: URL `https://eigenheim-invest.de/mcp/`, authentication **None**.
- Run every test prompt from `app-submission.json`; each answer must show source and date.

## 2. Submission form
| Field | Value |
|---|---|
| Name | Berlin Real Estate Market \| Eigenheim Invest |
| Short description | Live Berlin €/m² property prices, rental yields, land values and listings by Eigenheim Invest. |
| MCP server URL | `https://eigenheim-invest.de/mcp/` |
| Authentication | None |
| Tools | 8, all read-only (no write or destructive actions) |
| Website | https://eigenheim-invest.de/ |
| Privacy policy | https://eigenheim-invest.de/datenschutz/ |
| Support | info@eigenheim-invest.de |

## 3. Review checklist
- [ ] Server reachable, all 8 tools listed and annotated read-only
- [ ] No personal data: listings without street/house number, no leads
- [ ] Every answer names source (Rankimmo, IBB, Senate, Gutachterausschuss) and date
- [ ] Privacy policy URL works
- [ ] Logo / icon square PNG ready (min. 512×512)

## 4. After review
- **Approved:** publish from the OpenAI platform.
- **Rejected:** fix the reasons from the e-mail and resubmit; appeals by replying to the e-mail.
