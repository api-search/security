---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spoileralert.com
  spf: true
hosts:
- cert_expires: Sep 10 06:29:16 2026 GMT
  host: spoileralert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spoiler Alert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spoiler Alert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spoiler Alert
provider_slug: spoiler-alert
slug: spoiler-alert-domain-security
source_filename: spoiler-alert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spoileralert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spoileralert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoiler-alert/refs/heads/main/security/spoiler-alert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Food Waste
- Inventory Management
- Supply Chain
- Retail
- Marketplace
- Sustainability
---
