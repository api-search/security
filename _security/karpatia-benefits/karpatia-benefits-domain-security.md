---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: karpatia.tech
  spf: true
hosts:
- cert_expires: Aug 22 02:30:56 2026 GMT
  host: karpatia.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karpatia Benefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karpatia Benefits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Karpatia Benefits
provider_slug: karpatia-benefits
slug: karpatia-benefits-domain-security
source_filename: karpatia-benefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karpatia.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:30:56 2026 GMT\n  hsts: null\ndomains:\n- domain: karpatia.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karpatia-benefits/refs/heads/main/security/karpatia-benefits-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Employee Benefits
- Human Resources
- HR Tech
- Insurance
- Benefits Marketplace
- Reimbursement
- SaaS
---
