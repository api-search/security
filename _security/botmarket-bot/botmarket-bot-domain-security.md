---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:<redacted — a personal mailbox; the record exists, the address is withheld under the enrichment PII guardrail>"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: botmarket.bot
  spf: false
hosts:
- cert_expires: Oct 22 01:03:58 2026 GMT
  host: botmarket.bot
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botmarket Bot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KOA Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KOA Labs
provider_slug: botmarket-bot
slug: botmarket-bot-domain-security
source_filename: botmarket-bot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botmarket.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 01:03:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: botmarket.bot\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:<redacted — a personal mailbox; the record exists, the address is withheld under the enrichment PII guardrail>\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botmarket-bot/refs/heads/main/security/botmarket-bot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agents
- MCP
- A2A
- Agent Discovery
- Marketplace
- Directory
- Protocol
- x402
- Open Data
- agent-native
- Non-Profit
- Mexico
---
