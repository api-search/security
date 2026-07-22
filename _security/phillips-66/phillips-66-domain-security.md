---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: phillips66.com
  spf: true
hosts:
- cert_expires: Aug  7 23:59:59 2026 GMT
  host: www.phillips66.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phillips 66 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phillips 66, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Phillips 66
provider_slug: phillips-66
slug: phillips-66-domain-security
source_filename: phillips-66-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phillips66.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phillips66.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phillips-66/refs/heads/main/security/phillips-66-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Fortune 500
- Refining
- Chemicals
- Logistics
---
