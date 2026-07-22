---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stockly.ai
  spf: true
hosts:
- cert_expires: Sep 26 16:57:35 2026 GMT
  host: stockly.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stockly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stockly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stockly
provider_slug: stockly
slug: stockly-domain-security
source_filename: stockly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stockly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:57:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stockly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockly/refs/heads/main/security/stockly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Retail
- Inventory
- Stock Management
- Fulfillment
- Marketplace
- Supply Chain
---
