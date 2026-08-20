---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vekia.fr
  spf: true
hosts:
- cert_expires: Oct 23 21:36:25 2026 GMT
  host: www.vekia.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vekia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vekia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vekia
provider_slug: vekia
slug: vekia-domain-security
source_filename: vekia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vekia.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 21:36:25 2026 GMT\n  hsts: false\ndomains:\n- domain: vekia.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vekia/refs/heads/main/security/vekia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Supply Chain
- Demand Forecasting
- Inventory Optimization
- Replenishment
- Retail
- Machine-Learning
- Artificial Intelligence
- Logistics
- France
---
