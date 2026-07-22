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
hosts:
- cert_expires: Oct 14 19:18:50 2026 GMT
  host: scratchpad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scratchpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scratchpad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scratchpad
provider_slug: scratchpad
slug: scratchpad-domain-security
source_filename: scratchpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scratchpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:18:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scratchpad.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
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
- SaaS
---
