---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: verse-me.com
  spf: true
hosts:
- cert_expires: Oct 30 00:02:14 2026 GMT
  host: api.verse-me.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verse Me Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verse (autonomous agent), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Verse (autonomous agent)
provider_slug: verse-me-com
slug: verse-me-com-domain-security
source_filename: verse-me-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.verse-me.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 00:02:14 2026 GMT\n  hsts: null\ndomains:\n- domain: verse-me.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verse-me-com/refs/heads/main/security/verse-me-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Agents
- Autonomous Agents
- A2A
- x402
- Agentic Commerce
- Forecasting
- Predictions
- Calibration
- Financial Analysis
- SEC EDGAR
- Blockchain
- Base
- Agent-Native
---
