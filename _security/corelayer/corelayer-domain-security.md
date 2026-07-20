---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corelayer.com
  spf: true
hosts:
- cert_expires: Oct  1 20:04:40 2026 GMT
  host: docs.corelayer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 08:48:48 2026 GMT
  host: api.corelayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corelayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corelayer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Corelayer
provider_slug: corelayer
slug: corelayer-domain-security
source_filename: corelayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.corelayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:04:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.corelayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 08:48:48 2026 GMT\n  hsts: null\ndomains:\n- domain: corelayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelayer/refs/heads/main/security/corelayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- SRE
- Incident Response
- Observability
- Production Support
- Root Cause Analysis
- Anomaly Detection
- DevOps
- Agent Native
- MCP
- Fintech
---
