---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bolna.ai
  spf: false
hosts:
- cert_expires: Sep 20 06:05:35 2026 GMT
  host: www.bolna.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.bolna.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bolna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolna, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Bolna
provider_slug: bolna
slug: bolna-domain-security
source_filename: bolna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bolna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:05:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bolna.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bolna.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolna/refs/heads/main/security/bolna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Voice AI
- Conversational AI
- Voice Agents
- Telephony
- Speech
- Call Automation
- Contact Center
- MCP
---
