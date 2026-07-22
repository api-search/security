---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: materialbank.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: materialbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Materialbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Materialbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Materialbank
provider_slug: materialbank
slug: materialbank-domain-security
source_filename: materialbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: materialbank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: materialbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materialbank/refs/heads/main/security/materialbank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Marketplace
- Architecture
- Design
- Building Materials
- Samples
- Adobe Commerce
---
