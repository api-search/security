---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prediko.io
  spf: true
hosts:
- cert_expires: Sep 22 12:05:00 2026 GMT
  host: prediko.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prediko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prediko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prediko
provider_slug: prediko
slug: prediko-domain-security
source_filename: prediko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prediko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:05:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prediko.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prediko/refs/heads/main/security/prediko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Inventory Management
- Demand Forecasting
- Supply Chain
- Ecommerce
- Shopify
- Purchase Orders
- Retail
- AI
---
