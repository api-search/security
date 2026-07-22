---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runreveal.com
  spf: true
hosts:
- cert_expires: Sep 10 03:52:46 2026 GMT
  host: runreveal.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runreveal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RunReveal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RunReveal
provider_slug: runreveal
slug: runreveal-domain-security
source_filename: runreveal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runreveal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: runreveal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runreveal/refs/heads/main/security/runreveal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- SIEM
- Security Log Management
- Detection Engineering
- Threat Detection
- Incident Response
- Observability
- SQL
- MCP
- AI
---
