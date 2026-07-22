---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mhub.my
  spf: true
hosts:
- cert_expires: Oct  2 20:35:25 2026 GMT
  host: mhub.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MHub
provider_slug: mhub
slug: mhub-domain-security
source_filename: mhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mhub.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:35:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mhub.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mhub/refs/heads/main/security/mhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Property Technology
- PropTech
- Malaysia
- Sales
- CRM
- Accounting
- E-Invoicing
- SaaS
---
