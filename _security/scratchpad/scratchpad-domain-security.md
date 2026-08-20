---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scratchpad.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clearskies.cc
  spf: true
hosts:
- cert_expires: Nov  7 05:22:38 2026 GMT
  host: www.scratchpad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:31:32 2026 GMT
  host: clearskies.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:31:32 2026 GMT
  host: mcp.clearskies.cc
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scratchpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scratchpad, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scratchpad
provider_slug: scratchpad
slug: scratchpad-domain-security
source_filename: scratchpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scratchpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 05:22:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: clearskies.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:31:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.clearskies.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:31:32 2026 GMT\n  hsts: null\ndomains:\n- domain: scratchpad.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: clearskies.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scratchpad/refs/heads/main/security/scratchpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Sales
- CRM
- Salesforce
- Revenue Operations
- Artificial Intelligence
- Software-as-a-Service
- MCP
- Agents
- Sales Intelligence
---
