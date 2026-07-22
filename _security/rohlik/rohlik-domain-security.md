---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rohlik.cz
  spf: true
hosts:
- cert_expires: Oct  6 22:48:50 2026 GMT
  host: rohlik.cz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rohlik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rohlik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rohlik
provider_slug: rohlik
slug: rohlik-domain-security
source_filename: rohlik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rohlik.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:48:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rohlik.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rohlik/refs/heads/main/security/rohlik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- Grocery
- E-commerce
- Delivery
- Logistics
- MCP
- OAuth
- Europe
---
