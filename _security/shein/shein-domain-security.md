---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shein.com
  spf: true
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: shein.com
  hsts: true
  hsts_max_age: 7776000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shein Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SHEIN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SHEIN
provider_slug: shein
slug: shein-domain-security
source_filename: shein-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shein.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000000\ndomains:\n- domain: shein.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shein/refs/heads/main/security/shein-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-commerce
- Retail
- Fashion
- Marketplace
- Fulfillment
- Logistics
- Open Platform
- Sellers
---
