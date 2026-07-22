---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dupe.com
  spf: true
hosts:
- cert_expires: Oct  8 12:41:46 2026 GMT
  host: dupe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dupe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dupe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dupe
provider_slug: dupe
slug: dupe-domain-security
source_filename: dupe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dupe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:41:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dupe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dupe/refs/heads/main/security/dupe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shopping
- E-commerce
- Retail
- Visual Search
- Product Discovery
- Artificial Intelligence
- Affiliate
- MCP
---
