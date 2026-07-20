---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onarchipelago.com
  spf: true
hosts:
- cert_expires: Sep  9 21:32:41 2026 GMT
  host: www.onarchipelago.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 08:15:35 2026 GMT
  host: docs.onarchipelago.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.onarchipelago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archipelago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archipelago, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Archipelago
provider_slug: archipelago
slug: archipelago-domain-security
source_filename: archipelago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onarchipelago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:32:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.onarchipelago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:15:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.onarchipelago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: onarchipelago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archipelago/refs/heads/main/security/archipelago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Property Risk
- Underwriting
- Risk Management
- Commercial Property
- GraphQL
- Data
- AI Agent
---
