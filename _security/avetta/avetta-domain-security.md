---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avetta.com
  spf: true
hosts:
- cert_expires: Sep 11 12:34:33 2026 GMT
  host: avetta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 00:58:18 2026 GMT
  host: docs.api.avetta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:54:02 2026 GMT
  host: api.avetta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avetta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avetta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Avetta
provider_slug: avetta
slug: avetta-domain-security
source_filename: avetta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avetta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:34:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.avetta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:58:18 2026 GMT\n  hsts: false\n- host: api.avetta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:54:02 2026 GMT\n  hsts: null\ndomains:\n- domain: avetta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avetta/refs/heads/main/security/avetta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain
- Risk Management
- Compliance
- Contractor Management
- Safety
- ESG
- Supplier Management
---
